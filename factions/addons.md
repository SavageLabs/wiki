---
title: FactionsX Addon Guide
description: How to build an addon
published: true
date: 2020-05-28T20:50:30.559Z
tags: 
---

<figure class="table"><table><thead><tr><th colspan="7"></th></tr></thead>
<tbody><tr><td><p style="text-align:center;"><b>FactionsX</b></p></td><td>
<p style="text-align:center;"><a href="https://wiki.savagelabs.net/en/factions/information">Information</a></p></td><td>
<p style="text-align:center;"><a href="https://wiki.savagelabs.net/en/factions/installation">Installation</a></p></td><td>
<p style="text-align:center;"><a href="https://wiki.savagelabs.net/en/factions/permissions">Permissions</a></p></td><td>
<p style="text-align:center;"><a href="https://wiki.savagelabs.net/en/factions/placeholders">Placeholders</a></p></td><td>
<p style="text-align:center;"><a href="https://wiki.savagelabs.net/en/factions/default-files">Deafult Files</a></p></td><td>
<p style="text-align:center;">Addons</p></td></tbody></table></figure>

<figure class="table"><table><thead><tr><th colspan="6"><p style="text-align:center;">
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Available Addons &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp;</p></th></tr></thead>
<tbody><tr><td><p style="text-align:center;"><a href="https://wiki.savagelabs.net/factions/addons/fwild">FWild</a></p></td><td>
<p style="text-align:center;"><a href="https://wiki.savagelabs.net/factions/addons/ftop">FTOP</a></p></td><td>
<p style="text-align:center;"><a href="https://wiki.savagelabs.net/factions/addons/fgrace">FGrace</a></p></td><td>
<p style="text-align:center;"><a href="https://wiki.savagelabs.net/factions/addons/ftnt">FTNT</a></p></td><td>
<p style="text-align:center;"><a href="https://wiki.savagelabs.net/factions/addons/fprinter">FPrinter</a></p></td></tr></tbody></table></figure>

# How to create an addon for FactionsX
*FactionsX allows 'addons' to be loaded to dynamically add features to the plugin*

* This tutorial assumes basic maven & java knowledge.

I will be creating an example `/f wild` addon.

* Lets start off with an empty maven project.

Add and import the SavageLabs repository to access FactionsX & AddonFramework.
**These versions may be out of date - check the [SavageLabs Repo](https://nexus.savagelabs.net/#browse/browse:maven-releases:net%2Fprosavage%2Ffactionsx) to make sure.**
```xml
<repositories>
  <repository>
    <id>savagelabs</id>
    <url>https://nexus.savagelabs.net/repository/maven-public/</url>
  </repository>
</repositories>

<dependencies>
  <dependency>
    <groupId>net.prosavage.factionsx</groupId>
    <artifactId>FactionsX</artifactId>
    <version>0.3-PATREON</version>
    <scope>provided</scope>
	</dependency>
  
  <dependency>
    <groupId>net.prosavage.factionsx</groupId>
    <artifactId>AddonFramework</artifactId>
    <version>1.1</version>
		<scope>provided</scope>
	</dependency>
</dependencies>
```

You can add these to access the Spigot-API and use my [BasePlugin Framework](https://github.com/SavageLabs/SavageFramework) for providing configs for your addons
```xml
<dependency>
  <groupId>org.spigotmc</groupId>
  <artifactId>spigot-api</artifactId>
  <version>1.15.1-R0.1-SNAPSHOT</version>
  <scope>provided</scope>
</dependency>


<dependency>
  <groupId>net.prosavage</groupId>
  <artifactId>BasePlugin</artifactId>
  <version>1.7.3</version>
  <scope>provided</scope>
</dependency>
```

* Define addon properties.

Head into `/src/main/java/resources/` and create `addon.properties`
The content of my `addon.properties` file will be:
```properties
# Name of the addon, basically like a spigot plugin name.
name=FWild-Addon
# Main class of the addon, like a spigot plugin main class.
main=net.prosavage.factionsx.FWildAddon
```

* Create our main class.
So, following the `addon.properties` we defined above, our main class's path would be `/src/main/java/net/prosavage/factionsx/FWildAddon`.
```java
package net.prosavage.factionsx;

public class FWildAddon extends Addon {

    @Override
    protected void onEnable() {
        logColored("Enabling FWild-Addon!");
    }

    @Override
    protected void onDisable() {
        logColored("Disabling FWild-Addon!");
    }
}
```

* Test our addon.

Now, run `mvn install` and you should get a successful build. 
Copy the jar file generated in the `/target/` folder, put it in the `/plugins/FactionsX/addons` folder in your minecraft server.

Now start the server normally, and we should see a line in the FactionsX enable startup looking like `[FactionsX] Enabling FWild-Addon!`.

This means our addon loaded successfully, there should now also be a folder `/plugins/FactionsX/addons/FWild-Addon/`.

* Now, we can try injecting a command into FactionsX.

Lets create a class called `CmdWild`.
```java
package net.prosavage.factionsx;

import net.prosavage.factionsx.command.engine.CommandInfo;
import net.prosavage.factionsx.command.engine.CommandRequirementsBuilder;
import net.prosavage.factionsx.command.engine.FCommand;
import org.jetbrains.annotations.NotNull;

public class CmdWild extends FCommand {

    public CmdWild() {
        // Alias for the command, so this would do `/f wild`.
        getAliases().add("wild");
        // We can add multiple
        getAliases().add("wild-tp");
        
        // The commandRequirements pre-check common things for you, the official way.
        // For example we could add #asFactionMember(true) if we want to make sure they're a faction member.
        // Here we do not want this executed in console, as the console cannot be teleported.
        this.commandRequirements = new CommandRequirementsBuilder()
                .asPlayer(true)
                .build();
    }


    public void execute(@NotNull CommandInfo info) {
        info.message("Executing wild command, since you passed the command requirement check.");
    }


    /**
     * This is used by the command engine to tell a player what a command does in the help menu
     */
    @NotNull
    public String getHelpInfo() {
        return "teleport to a random chunk.";
    }
}
```

Now for our execute method, we want to load the random chunk async and THEN teleport.
[PaperLib](https://github.com/PaperMC/PaperLib) allows us to do this, however, its an external library. FactionsX's addon system also can load libraries, they simply need to be specified in the pom normally.

So we add the following to our `pom.xml`
```xml
<repository>
   <id>papermc</id>
   <url>https://papermc.io/repo/repository/maven-public/</url>
</repository>

<dependency>
  <groupId>io.papermc</groupId>
  <artifactId>paperlib</artifactId>
  <version>1.0.2</version>
  <scope>compile</scope>
</dependency>
```

Now we can access PaperLib, and load a random chunk.


Now we have to register the command into FactionsX.
We also need to remove it on disable.
```java
public class FWildAddon extends Addon {

    @Override
    protected void onEnable() {
        logColored("Enabling FWild-Addon!");
        FactionsX.baseCommand.addSubCommand(new CmdWild());
    }

    @Override
    protected void onDisable() {
        logColored("Disabling FWild-Addon!");
        FactionsX.baseCommand.removeSubCommand(new CmdWild());
    }
}
```
Our addon will now add the command on startup, and remove on shutdown.



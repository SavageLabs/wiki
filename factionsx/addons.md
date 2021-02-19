---
title: FactionsX Addon Guide
description: How to build an addon
published: true
date: 2021-02-19T23:11:33.797Z
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
<p style="text-align:center;"><a href="https://wiki.savagelabs.net/factions/addons/fshop">FShop</a></p></td><td>
  <p style="text-align:center;"><a href="https://wiki.savagelabs.net/factions/addons/fmobtweaks">FMobTweaks</a></p></td><td>
  <p style="text-align:center;"><a href="https://wiki.savagelabs.net/factions/addons/fdynmap">FDynmap</a></p></td><td>
  <p style="text-align:center;"><a href="https://wiki.savagelabs.net/factions/addons/fshop">FShop</a></p></td><td>
  <p style="text-align:center;"><a href="https://wiki.savagelabs.net/factions/addons/fchest">FChest</a></p></td><td>
  <p style="text-align:center;"><a href="https://wiki.savagelabs.net/factions/addons/fcropupgrades">FCropUpgrades</a></p></td><td>
<p style="text-align:center;"><a href="https://wiki.savagelabs.net/factions/addons/fprinter">FPrinter</a></p></td></tr></tbody></table></figure>

# How to create an addon for FactionsX
*FactionsX allows 'addons' to be loaded to dynamically add features to the plugin*

* The source code for the completed guide can be found below:
https://github.com/ProSavage/FWild-Addon-Example

* This tutorial assumes basic maven & java knowledge.

I will be creating an example `/f wild` addon.

* Lets start off with an empty maven project.

Add and import the SavageLabs repository to access FactionsX & AddonFramework.
The version for AddonFramework and FactionsX *should* match.
**These versions may be out of date - check the [SavageLabs Repo](https://nexus.savagelabs.net/#browse/browse:maven-releases:net%2Fprosavage%2Ffactionsx) to make sure.**
```xml
<repositories>
  <repository>
    <id>savagelabs</id>
    <url>https://nexus.savagelabs.net/repository/maven-releases/</url>
  </repository>
</repositories>

<dependencies>
  <dependency>
    <groupId>net.prosavage.factionsx</groupId>
    <artifactId>FactionsX</artifactId>
    <version>1.0.8-RC</version>
    <scope>provided</scope>
	</dependency>
  
  <dependency>
    <groupId>net.prosavage.factionsx.addonframework</groupId>
    <artifactId>AddonFramework</artifactId>
    <version>1.0.8-RC</version>
    <scope>provided</scope>
  </dependency>
</dependencies>
```

You can add these to access the Spigot-API and use my [BasePlugin Framework](https://github.com/SavageLabs/SavageFramework) for providing configs for your addons
```xml
  <repository>
    <id>spigot-repo</id>
    <url>https://hub.spigotmc.org/nexus/content/repositories/snapshots/</url>
</repository>


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
main=net.prosavage.fwildaddon.FWildAddon
```

* Create our main class.
So, following the `addon.properties` we defined above, our main class's path would be `/src/main/java/net/prosavage/factionsx/FWildAddon`.
```java
package net.prosavage.fwildaddon;

import net.prosavage.factionsx.addonframework.Addon;

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

Now, run `mvn package` and you should get a successful build. 
Copy the jar file generated in the `/target/` folder, put it in the `/plugins/FactionsX/addons` folder in your minecraft server.

Now start the server normally, and we should see a line in the FactionsX enable startup looking like `[FactionsX-FWild-Addon] Enabling FWild-Addon!`.

This means our addon loaded successfully, there should now also be a folder `/plugins/FactionsX/addons/FWild-Addon/`.

* Now, we can try injecting a command into FactionsX.

Lets create a class called `CmdWild`.
```java
package net.prosavage.fwildaddon;

import net.prosavage.factionsx.command.engine.CommandInfo;
import net.prosavage.factionsx.command.engine.CommandRequirementsBuilder;
import net.prosavage.factionsx.command.engine.FCommand;

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


    public boolean execute(CommandInfo info) {
        info.message("Executing wild command, since you passed the command requirement check.");
        return true;
    }


    /**
     * This is used by the command engine to tell a player what a command does in the help menu
     */
    public String getHelpInfo() {
        return "teleport to a random chunk.";
    }
}
```

* Register the command.

Now we have to register the command into FactionsX.
We also need to remove it on disable.
```java
package net.prosavage.fwildaddon;

import net.prosavage.factionsx.FactionsX;
import net.prosavage.factionsx.addonframework.Addon;

public class FWildAddon extends Addon {

    private static CmdWild cmdWild = new CmdWild();

    @Override
    protected void onEnable() {
        logColored("Enabling FWild-Addon!");
        FactionsX.baseCommand.addSubCommand(cmdWild);
    }

    @Override
    protected void onDisable() {
        logColored("Disabling FWild-Addon!");
        FactionsX.baseCommand.removeSubCommand(cmdWild);
    }
}
```
Our addon will now add the command on startup, and remove on shutdown.

* Creating a config file

Next, we are going to create a configuration file.

We are going to need an instance of our main class, so let's turn it into a singleton.

```java
package net.prosavage.fwildaddon;

import net.prosavage.factionsx.FactionsX;
import net.prosavage.factionsx.addonframework.Addon;

public class FWildAddon extends Addon {

    private static FWildAddon instance;

    public static FWildAddon getInstance() {
        return instance;
    }

    private static CmdWild cmdWild = new CmdWild();

    @Override
    protected void onEnable() {
        logColored("Enabling FWild-Addon!");
        instance = this;
        FactionsX.baseCommand.addSubCommand(cmdWild);
    }

    @Override
    protected void onDisable() {
        logColored("Disabling FWild-Addon!");
        FactionsX.baseCommand.removeSubCommand(cmdWild);
    }
}
```


Create a class called `WildConfig`.
```java
package net.prosavage.fwildaddon;

import net.prosavage.factionsx.FactionsX;
import net.prosavage.factionsx.addonframework.Addon;

import java.io.File;

public class WildConfig {

    public static transient WildConfig instance = new WildConfig();

    public static String coolConfigOption = "yeah boiii";


    public static void save(Addon addon) {
        addon.getConfigSerializer().save(instance,
                new File(FWildAddon.getInstance().getAddonDataFolder(), "config.json")
        );
    }

    public static void load(Addon addon) {
        FactionsX.baseCommand.getHelpInfo();
        addon.getConfigSerializer().load(instance,
                WildConfig.class,
                new File(FWildAddon.getInstance().getAddonDataFolder(), "config.json")
        );
    }

}
```

Next we want to load, and then save our config.
So our main class should look like this now:
```java
package net.prosavage.fwildaddon;

import net.prosavage.factionsx.FactionsX;
import net.prosavage.factionsx.addonframework.Addon;

public class FWildAddon extends Addon {

    private static FWildAddon instance;

    public static FWildAddon getInstance() {
        return instance;
    }

    private static CmdWild cmdWild = new CmdWild();

    @Override
    protected void onEnable() {
        logColored("Enabling FWild-Addon!");
				instance = this;
        FactionsX.baseCommand.addSubCommand(cmdWild);
        WildConfig.load(this);
    }

    @Override
    protected void onDisable() {
        logColored("Disabling FWild-Addon!");
        FactionsX.baseCommand.removeSubCommand(cmdWild);
        // Load first to read changes from file, then save.
        WildConfig.load(this);
        WildConfig.save(this);
    }
}
```

Lets test this, so run `mvn package` again, and see if we generate a config.

So once our server starts, we should see a file at the following location: `/plugins/FactionsX/addons/FWild-Addon/config.json`

With the following contents:
```json
{
  "coolConfigOption": "yeah boiii"
}
```

Since we had a field, it is now represented in our json configuration file, 
and the load function will read the value from file, and then sync it to the variable in memory.
```java
public static String coolConfigOption = "yeah boiii";
```

So you can add whatever fields you want and they will be automatically handled by the framework.

The same system can be used to create data files, but you won't have to call the `load` function on shutdown since the values do not need to be read.


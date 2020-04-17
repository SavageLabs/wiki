---
title: Addon Guide
description: How to build an addon
published: 1
date: 2020-04-17T22:01:37.701Z
tags: 
---

# How to create an addon for FactionsX
*FactionsX allows 'addons' to be loaded to dynamically add features to the plugin*

* This tutorial assumes basic maven & java knowledge.

I will be creating an example `/f wild` addon.

1. Lets start off with an empty maven project.

Add and import the SavageLabs repository to access FactionsX & AddonFramework.
**These versions may be out of date - check the [SavageLabs Repo](https://nexus.savagelabs.net/#browse/browse:maven-releases:net%2Fprosavage%2Ffactionsx) to make sure.**
```xml
<repositories>
  <!-- SavageLabs repository -->
  <repository>
    <id>savagelabs</id>
    <url>https://nexus.savagelabs.net/repository/maven-public/</url>
  </repository>
</repositories>

<dependencies>
  <!-- FactionsX Lib -->
  <dependency>
    <groupId>net.prosavage.factionsx</groupId>
    <artifactId>FactionsX</artifactId>
    <version>0.2-PATREON</version>
	</dependency>

  <!-- AddonFramework Lib -->
  <dependency>
    <groupId>net.prosavage.factionsx</groupId>
    <artifactId>AddonFramework</artifactId>
    <version>1.0</version>
	</dependency>
</dependencies>
```

2. Define addon properties.

Head into `/src/main/java/resources/` and create `addon.properties`
The content of my `addon.properties` file will be:
```properties
# Name of the addon, basically like a spigot plugin name.
name=FWild-Addon
# Main class of the addon, like a spigot plugin main class.
main=net.prosavage.factionsx.FWildAddon
```

3. Create our main class.

So, following the `addon.properties` we defined above, our main class's path would be `/src/main/java/net/prosavage/factionsx/FWildAddon`.
```java
package net.prosavage.factionsx;

public class FWildAddon extends Addon {

    @Override
    protected void onEnable() {
        getInstance().getLogger().info("Enabling FWild-Addon!");
    }

    @Override
    protected void onDisable() {
        getInstance().getLogger().info("Disabling FWild-Addon!");
    }
}
```

4. Test our addon.

Now, run `mvn install` and you should get a successful build. 
Copy the jar file generated in the `/target/` folder, put it in the `/plugins/FactionsX/addons` folder in your minecraft server.

Now start the server normally, and we should see a line in the FactionsX enable startup looking like `[FactionsX] Enabling FWild-Addon!`.

This means our addon loaded successfully, there should now also be a folder `/plugins/FactionsX/addons/FWild-Addon/`.

5. Now, we can try injecting a command into FactionsX.



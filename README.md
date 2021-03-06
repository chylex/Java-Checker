You can download latest versions of Java Checker on CurseForge:

http://minecraft.curseforge.com/projects/java-version-checker

The mod is in Public Domain, so do whatever you want with it! Hugs and mentions appreciated but not required. If you want to include Java Checker in your own mod, read the shading guide.

## Repository archived

Because Minecraft 1.12+ already requires Java 8 and mods cannot use Java 9+ yet, the repository has been archived. If modding starts moving towards a newer version of Java in the future, I might revisit the project.

## Shading Java Checker into your mod

You can insert Java Checker into your mod, so that it will alert the user if they are using outdated Java. You will need to use a special version designed for shading, you can use tterrag's Maven repository in your build.gradle or download it manually.

The shading library should work fine for all Minecraft versions since 1.6.2. It can currently check for Java 7 or 8, based on how you configure it.

In order to shade and configure Java Checker, you need to update your **build.gradle** file. Use the following links as a guide, make sure to update everything in the <> brackets.

[ForgeGradle 1.2 (Minecraft 1.7.10 and older)](https://github.com/chylex/Java-Checker/wiki/Shading-with-ForgeGradle-1.2)

[ForgeGradle 2.1 (Minecraft 1.8 and newer)](https://github.com/chylex/Java-Checker/wiki/Shading-with-ForgeGradle-2.1)

You can also use [Hardcore Ender Expansion's build.gradle](https://github.com/chylex/Hardcore-Ender-Expansion/blob/master/build.gradle) as a reference.

Now build the mod and run it to make sure nothing messed up. If the mod does not load, something might have changed in Forge which breaks a hack in the shading library. In that case, [create a new issue](https://github.com/chylex/Java-Checker/issues) and I will release an update.

# Minecraft Skin Converter

This project will convert pre-1.8 skins into 1.8 skins. You can choose to convert 1 skin to the new format, or you can combine 2 skins into one.

## Table of Contents

- [About](#about)
- [Building the Project](#building-the-project)
  - [Set Up Environment Variables](#set-up-environment-variables)
  - [Convert to Eclipse Project](#convert-to-eclipse-project)
  - [Export Project to JAR File](#export-project-to-jar-file)
  - [Execute the JAR File](#execute-the-jar-file)
- [Contribute](#contribute)
- [License](#license)

## About

In Minecraft [release 1.8][1], [skin cutomization][2] was improved.

The size of the skin file was increased from [64 x 32 pixels][3] to [64 x 64 pixels][4]. The additional 32 pixels adds support for a full body overlay with independent left and right arms and legs. Instead of just a hat (head) overlay, you also have a jacket (body), sleeves (arms) and pants (legs).

The right and left arms and legs can now be edited independently. Previously, you could only edit the right arm and leg and they would be mirrored to produce the left arm and leg. 

## Building the Project

In order to build this project, you will need to use [Eclipse][5] and [Gradle][6].

### Set Up Environment Variables

The following variables should point to their installation directory.

- `JAVA_HOME`
- `GRADLE_HOME`

### Convert to Eclipse Project

Before the project can be imported into Eclipse, you must convert it to an Eclipse project. This task will generate the `.settings/`, `.classpath`, and `.project` files.

    C:\Eclipse\workspace\MinecraftSkinConverter>gradle eclipse --daemon

### Export Project to JAR File

This project can be exported to a standalone JAR file, by executing the following task.

    C:\Eclipse\workspace\MinecraftSkinConverter>gradle jar --daemon

### Execute the JAR File

You can either navigate to the `build/libs/` directory in the project and double-click to launch the application, or you can launch it from the terminal with the command below.

    C:\Eclipse\workspace\MinecraftSkinConverter>java -jar build\libs\MinecraftSkinConverter-1.0.jar

## Contribute

If you would like to contribute to the project, have at it. [Fork this project][7] project, include your changes, and [submit a pull request][8] back to the main repository.

## License

[MIT License][9] - see the LICENSE.txt file in the source distribution.

  [1]: http://minecraft.gamepedia.com/1.8
  [2]: http://minecraft.gamepedia.com/Skin
  [3]: http://minecraft.gamepedia.com/File:Skintemplate.png
  [4]: http://minecraft.gamepedia.com/File:1.8_Skin_Template.png
  [5]: http://www.eclipse.org/
  [6]: https://gradle.org/
  [7]: https://help.github.com/articles/fork-a-repo
  [8]: https://help.github.com/articles/using-pull-requests
  [9]: http://opensource.org/licenses/mit-license.html

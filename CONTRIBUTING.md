
<p align="center">
  <a href="https://tcno.co/">
    <img src="https://raw.githubusercontent.com/TcNobo/TcNo-Acc-Switcher-Themes/master/other/img/Themes_Banner.png"></a>
</p>

# Contributing guidelines

These are the guidelines for contributing to this repository.

## Before contributing

To avoid similar themes with small changes, themes are merged only if they bring large/sensitive changes to the default TcNo Account Switcher UI, and are different to existing themes.

A theme's file name should be the same as the themes name (where possible - avoiding windows file name errors), with spaces replaced by underscores. Names are set in the `name:` parameter.

Example: `name: Dracula Cyan` should have the filename: `Dracula_Cyan.yaml`


## How to contribute

### To add your own theme
1. Fork this repository
2. Create a folder where you'll put your themes (Example: `Default_Themes` in `Themes`, or `Fire_Flavours` in `Themes`)
3. Either:
	- Follow theme creation steps below in: **Creating a theme**, or
	- Create subfolders for themes (eg. `Dracula_Cyan` and `Old_Default`) and a `README.md` for a catalogue. See: **Multiple themes**.
4. Add your theme to the master theme list. See: **Add your themes the Themes.md list**.
5. Finally, **Create a pull request**!

## Creating a theme
In the folder you just created: 
1. Create a `style.scss` file, where you can put your modifications. 
	Do include info at the top of your scss file as follows:
```markdown
/*
	<Theme name>
	- Created by <Username>
*/
... Theme scss
```
2. Create an `info.yaml` file (required) with the following required fields in it (Used by updater, etc). See the `Dracula Cyan` example below:
```yaml
# This theme's name (Shows in-app, can be different to folder name)
name: Dracula Cyan (Default)
accent: "#8BE9FD"

# Required colors for updater & main UI (not HTML/CSS):
# - Not including these will cause the updater to use default color scheme (Dracula Cyan)
linkColor: "#8BE9FD" # Accent color
headerbarBackground: "#253340"
mainBackground: "#0E1419"
modalInputBackground: "#070A0D"
borderedItemBorderColor: "#888888"
buttonBackground: "#274560"
buttonBackground-hover: "#28374E"
buttonBackground-active: "#28374E"
buttonColor: "#FFFFFF"
buttonBorder: "#274560"
buttonBorder-hover: "#274560"
buttonBorder-active: "#8BE9FD"
windowControlsBackground: "#253340"
windowControlsBackground-active: "#3B4853"
windowControlsCloseBackground: "#D51426"
windowControlsCloseBackground-active: "#D51426"
```
#### Now that you have your theme, you need to document it.

3. Create a `README.md` file using the template below:
```markdown
# <Theme name>

## Screenshots
[Followed by at least one image - Example:]
<![Tag](image.png)>

## Information
<Why your theme is unique>
Created by <username>.

[Specify any fonts needed, download links if not included in SCSS; (optionally) author name and/or any other info about the theme]
```

4. **Extra files?** In the future, extra `js`, `css` and other files are planned to be used by the program as well. Currently only `style.scss` is compiled and used by the TcNo Account Switcher. Images and other files in this folder will not link properly. FOR NOW user input is required (mentioned under *Installation* in the main `README.md`. You can create a `wwwroot` folder and place required files in there. Do see the actual [wwwroot folder](https://github.com/TcNobo/TcNo-Acc-Switcher/tree/master/TcNo-Acc-Switcher-Server/wwwroot) so you know what directory structure to follow. 
If your work applies or works well with the actual program, your user-content could be included in any way in the official repo. You will be credited in the software for all to see.

## Multiple themes

Create subfolders for each theme, as well as a catalogue `README.md` file. Continuing the aforementioned `Fire_Flavours` example. As an example, we'll make a new folder for `Purple` and `Green` in `Fire_Flavours`.

1. Create the catalogue `README.md` file, using the template below:
```markdown
# <Category name>

## Information

<Maybe some info on your themes, a logo image or anything else>

### [Name of theme 1](<relative/link>)

[1 image from theme]

### [Name of theme 2](<relative/link>)

[1 image from theme]

...
```

2. In each theme subfolder, place all your theme files. See **Creating a theme**.

## Add your themes the Themes.md list
For now just add themes following the format already used, and shown below. In the future when there are lots of themes this file may be restructured.

Edit the existing `Themes.md` file to add your work.

1. Create your theme/author heading. For multiple themes in a group, use that name, for single themes maybe use a username or your theme's name. The link should take them to the folder containing either your theme, or the category file containing all your themes.

**For a single theme:**
```markdown
## [<Theme group name>](Themes/<Themes folder>)

[A single image of the theme]
```

**For a theme group:**

```markdown
## [<Theme group name>](Themes/<Themes folder>)

### [<Theme name 1>](Themes/<Themes folder>/<Theme1>)

[A single image of the theme]

...
```

**Image guidelines:** 
Either include individual screenshots if you only have 1 or 2 themes, or create an image that shows more than a few themes in one (or a few images) - Whether just a mosaic, or an edited view with names for each theme\color palette. It's up to you. Just don't include 3,000 of these - 3 or so is fine. Anything more, please compile down into one or a few images.
 
 ## Create a pull request
 Open a Pull Request and you can include more details in the commit message.
 Try to keep it simple, and do a good job with explaining what your theme is, and/or what makes it different to already existing similar themes (if any).

**Finally....**
Thank you for taking the time to help out with this project. Extra help is always appreciated. Seeing the community grow this far has been awesome.

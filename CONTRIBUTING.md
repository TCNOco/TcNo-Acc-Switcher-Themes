
<p align="center">
  <a href="https://tcno.co/">
    <img src="https://raw.githubusercontent.com/TcNobo/TcNo-Acc-Switcher/master/other/img/Banner.png"></a>
</p>

# Contributing guidelines

These are the guidelines for contributing to this repository.

## Before contributing

To avoid similar themes with small changes, themes are merged only if they bring large/sensitive changes to the default TcNo Account Switcher UI, and are different to existing themes.

A theme's file name should be the same as the themes name (where possible - avoiding windows file name errors), with spaces replaced by underscores. Names are set in the `name:` parameter.

Example: `name: Dracula Cyan` should have the filename: `Dracula_Cyan.yaml`


## How to contribute

To add your own theme:
1. Fork this repository
2. Create another folder with the same name as your theme yaml
3. Create a `XYZ.yaml` file, where `XYZ` is the name of your theme, based off the default theme: `Default.yaml`.
4. Create a `README.md` with the following structure:
```markdown
# Theme name

## Screenshots

[Followed by at least one image]

## Information

[Specify any fonts needed; (optionally) author name and/or any other info about the theme]
```

If you're submitting more than 1 theme under a general category: Create a folder with subfolders for each theme. Follow the folder and README structure above for each theme. For example: `Dracula` can contain `Dracula Blue` and `Dracula Purple` folders, with a YAML file and README in each. If you do this, add another README in the category folder (containing all the themes) with screenshots and titles for each. The category README should follow this format:
```markdown
# Category name

## Screenshots

### Name of theme 1

[1 image from theme]

### Name of theme 2

[1 image from theme]

...
```
5. Add your theme, or theme category to the THEMES.md file using the following structure. The file is ordered alphabetically, keep it that way.

```markdown
## [Theme name](ThemeFolder)

[A single image of the theme]
```
or
```markdown
## [Category name](ThemeCategory)

### [Theme name 1](ThemeCategory/Theme1)

[A single image of the theme]

### [Theme name 2](ThemeCategory/Theme2)

[A single image of the theme]

...
```

6. Commit only once. 
7. Open a Pull Request and you can include more details in the commit message.
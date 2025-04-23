Myst Theme for Obsidian.

## Introduction
The CSS has been modified with reference to IntelliJ color schemes.  
Confirmed to work properly on Obsidian v1.8.9.

## Features
- Title Style Change: Added a pen icon at the beginning of titles to make it clear when editing is in progress, and used an animated background effect to keep things visually engaging.
- Added lines below H2 headings to help distinguish between sections more clearly.
- Used different colors to emphasize text and make it stand out.
- Change the default font to `S-CoreDream-3Light`.
- Added folder icons in the file explorer to make it easier to distinguish between folders and files.


## Theme deploy
If you have modified theme.css, manifest.json, create a new release in the following order.

### 1.Tag creation

```bash
git tag -a 1.0.1 -m "1.0.1"
git push origin 1.0.1
```

### 2.Performed by GitHub action

Github action is automatically executed.
Wait until the action ends normally.

### 3.Release creation
1. Select `Release` in the right sidebar.
2. Select `draft a new release`.
3. Input tag selection and title (explanation can be omitted)
4. attached `manifest.json` and `theme.css`
5. `Publish Release`

### References
- [Build a theme](https://docs.obsidian.md/Themes/App+themes/Build+a+theme)
- [Release your theme with GitHub Actions](https://docs.obsidian.md/Themes/App+themes/Release+your+theme+with+GitHub+Actions)
- [Submit your theme](https://docs.obsidian.md/Themes/App+themes/Submit+your+theme)
- [Embed fonts and images in your theme](https://docs.obsidian.md/Themes/App+themes/Embed+fonts+and+images+in+your+theme)


## License
MIT

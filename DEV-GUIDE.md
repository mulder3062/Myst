# Development Guide

# Apply it to Local First

First, launch Obsidian.

You can open developer tools to check styles:
- Windows: `Ctrl + Shift + i`
- MacOS: `Command + Option + i` 

Go to `Setting > Appearance` and click the folder icon next to Themes to check the path of your currently applied theme.

If your theme is `Myst`, the CSS path will be `obsidian/.obsidian/themes/Myst/theme.css`.

When you modify the `theme.css` file, you can immediately see the changes in Obsidian.

# Release theme 

## 1. `manifest.json` version update

example:
```json
{
	"name": "Myst",
	"version": "1.0.7",
	"minAppVersion": "1.9.12",
	"author": "mulder3062",
	"authorUrl": "https://github.com/mulder3062"
}
```

## 2. `version.json` version update

example:
```json
{
	"1.0.0": "1.8.9",
	"1.0.1": "1.8.9",
	"1.0.2": "1.8.9",
	"1.0.3": "1.8.9",
	"1.0.4": "1.8.9",
	"1.0.5": "1.8.9",
	"1.0.6": "1.8.10",
	"1.0.7": "1.9.12"
}
```



## 3. GitHub Actions
[Guide](https://docs.obsidian.md/Themes/App+themes/Release+your+theme+with+GitHub+Actions)

Note: If you already have a 'release obsidian theme' in the Github Action, run the following steps after modification.

1. Create a tag that matches the version in the `manifest.json` file.
```bash
git tag -a 1.0.7 -m "1.0.7"
git push origin 1.0.7
```

2. Browse to your repository on GitHub and select the Actions tab. Your workflow might still be running, or it might have finished already.
3. When the workflow finishes, go back to the main page for your repository and select Releases in the sidebar on the right side. The workflow has created a draft GitHub release and uploaded the required assets as binary attachments.
4. Select Edit (pencil icon) on the right side of the release name.
5. Add release notes to let users know what happened in this release, and then select Publish release.

## References
- [Build a theme](https://docs.obsidian.md/Themes/App+themes/Build+a+theme)
- [Release your theme with GitHub Actions](https://docs.obsidian.md/Themes/App+themes/Release+your+theme+with+GitHub+Actions)
- [Submit your theme](https://docs.obsidian.md/Themes/App+themes/Submit+your+theme)
- [Embed fonts and images in your theme](https://docs.obsidian.md/Themes/App+themes/Embed+fonts+and+images+in+your+theme)


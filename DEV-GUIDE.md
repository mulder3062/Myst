# Development Guide

# Apply it to Local First

First, launch Obsidian.

You can open developer tools to check styles:
- Windows: `Ctrl + Shift + i`
- MacOS: `Command + Option + i` 

Go to `Setting > Appearance` and click the folder icon next to Themes to check the path of your currently applied theme.

If your theme is `Myst`, the CSS path will be `obsidian/.obsidian/themes/Myst/theme.css`.

When you modify the `theme.css` file, you can immediately see the changes in Obsidian.

# Github Actions으로 테마 릴리즈하기
[가이드](https://docs.obsidian.md/Themes/App+themes/Release+your+theme+with+GitHub+Actions)

참고: 이미 github action에 `Release Obsidian theme`가 있다면 수정 후 아래 단계를 실행합니다.

1. Create a tag that matches the version in the `manifest.json` file.
```bash
git tag -a 1.0.1 -m "1.0.1"
git push origin 1.0.1
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


---
title: "My Minimal VSCode Setup"
date: 2024-05-18T19:37:25Z
author: "aefly"
slug: my-minimal-vscode-setup
tags: ["VSCode", "Development", "Programming"]
comments: true
draft: false
showToc: true
TocOpen: false
hidemeta: false
disableHLJS: false
hideSummary: false
searchHidden: false
ShowReadingTime: true
ShowBreadCrumbs: true
ShowCodeCopyButtons: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
---

## Introduction

VSCode has become the go-to code editor for many developers due to its versatility, performance, and extensive ecosystem of plugins. However, setting up the perfect environment can sometimes feel overwhelming with the sheer number of options available. In this post, I'll share my minimal VSCode setup, including configurations and essential plugins that enhance my workflow without overwhelming it.

## Theme

Choosing a theme that is easy on the eyes and enhances readability is crucial. I use the [CodeSandbox Theme](https://marketplace.visualstudio.com/items?itemName=ngryman.codesandbox-theme) with the "Legacy" color scheme. This theme offers a clean and visually appealing interface, making long coding sessions more comfortable.

## Font

For the font, I prefer [Cascadia Code](https://github.com/microsoft/cascadia-code) by Microsoft, along with [Caskaydia Nerd Font](https://www.nerdfonts.com/font-downloads) from NerdFont for terminal icons. This combination provides a clear and modern look with support for programming ligatures and icons.

## Extensions

To maximize productivity and maintain a clutter-free workspace, I rely on a few key extensions. Here are my top picks:

- **[emojisense](https://marketplace.visualstudio.com/items?itemName=bierner.emojisense)**: Adds emoji suggestions to your autocomplete menu, making it easy to insert emojis into your code or comments.
- **[Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)**: Helps you create more human-friendly comments in your code. This extension allows you to categorize comments using different colors, which makes your annotations more readable and organized.
- **[Discord Presence](https://marketplace.visualstudio.com/items?itemName=icrawl.discord-vscode)**: Shows your coding activity on your Discord profile. It's a fun way to let your friends and colleagues see what you're working on in real-time.
- **[Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)**: Replaces the default file icons with material design icons. It enhances the visual appeal and makes it easier to identify different file types at a glance.
- **[Output Colorizer](https://marketplace.visualstudio.com/items?itemName=IBM.output-colorizer)**: Adds syntax highlighting to the VSCode Output Panel. It makes reading logs and debugging output much easier by adding color coding to different types of messages.
- **[Project Manager](https://marketplace.visualstudio.com/items?itemName=alefragnani.project-manager)**: Simplifies switching between projects. This extension allows you to save your workspace configurations and quickly switch between them, which is especially useful if you work on multiple projects simultaneously.
- **[Remote - SSH](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-ssh)**: Allows you to open a remote folder on any remote machine using SSH and take advantage of VSCode’s full feature set. This is invaluable for working on servers or remote environments.
- **[Conventional Commits](https://marketplace.visualstudio.com/items?itemName=vivaxy.vscode-conventional-commits)**: Assists you in writing conventional commits messages, which is essential for maintaining a consistent commit history and automating the release process.
- **[GitHub Actions](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-github-actions)**: Provides an interface to view and manage GitHub Actions workflows directly from VSCode. This extension helps you monitor your CI/CD pipelines without leaving your editor.
- **[GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)**: Enhances the built-in Git capabilities of VSCode. It allows you to visualize code authorship, seamlessly navigate through your repository’s history, and much more.
- **[Live Preview](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server)**: Provides a live preview of your web application. It's particularly useful for front-end developers as it shows changes in real-time as you code.
- **[Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)**: A comprehensive Markdown editing experience. This extension includes shortcuts, a preview pane, and many other features to streamline Markdown editing.
- **[Markdown Emoji](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-emoji)**: Adds emoji support to Markdown files, enabling you to easily include emojis in your documentation and notes.
- **[markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint)**: Ensures your Markdown files follow best practices. It highlights issues and provides fixes, which is great for maintaining consistent and clean documentation.
- **[Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)**: An opinionated code formatter that supports many languages. It enforces a consistent style by parsing your code and re-printing it with its own rules.

## Settings

Here is my global `settings.json`, optimized for a clean and efficient coding experience:

```json
{
  "editor.acceptSuggestionOnCommitCharacter": false,
  "editor.fontFamily": "'CaskaydiaMono Nerd Font Mono', Cascadia Code, Consolas, 'Courier New', monospace",
  "editor.fontLigatures": true,
  "editor.fontSize": 13,
  "editor.linkedEditing": true,
  "editor.lineHeight": 22,
  "editor.minimap.enabled": false,
  "editor.occurrencesHighlight": "off",
  "editor.renderWhitespace": "trailing",
  "editor.suggest.insertMode": "replace",
  "editor.guides.indentation": false,
  "editor.cursorBlinking": "smooth",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.smoothScrolling": true,
  "explorer.autoReveal": false,
  "explorer.confirmDelete": false,
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmPasteNative": false,
  "files.autoSave": "onWindowChange",
  "git.autofetch": true,
  "git.confirmSync": false,
  "git.enableSmartCommit": true,
  "git.ignoreRebaseWarning": true,
  "gitlens.telemetry.enabled": false,
  "gitlens.graph.minimap.enabled": false,
  "json.schemaDownload.enable": true,
  "workbench.editor.enablePreview": false,
  "workbench.tree.indent": 20,
  "workbench.tree.renderIndentGuides": "always",
  "workbench.layoutControl.enabled": false,
  "terminal.integrated.smoothScrolling": true,
  "editor.mouseWheelScrollSensitivity": 1.3,
  "workbench.iconTheme": "material-icon-theme",
  "security.workspace.trust.untrustedFiles": "open",
  "window.titleBarStyle": "custom",
  "window.commandCenter": false,
  "window.menuBarVisibility": "compact",
  "telemetry.telemetryLevel": "off",
  "discord.removeDetails": true,
  "workbench.startupEditor": "none",
  "workbench.colorTheme": "CodeSandbox Legacy",
  "remote-explorer.foldersSortOrder": "alphabetical"
}
```

## Preview

With the settings listed above, my VSCode environment looks like this:

![VSCode](https://cdn.aefly.gg/cache/v1/blog/my-minimal-vscode-setup/1.webp)

## Conclusion

With this minimal VSCode setup, I strike a balance between functionality and simplicity. By customizing basic configurations and carefully selecting essential plugins, I create an environment tailored to my needs without overwhelming clutter. Remember, the key is to adapt these settings to your workflow and preferences.

Feel free to share your own setups or any extensions you find indispensable in the comments below.

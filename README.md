<p align="center">
<img src="Sources/icon.png" height="130" width="130"/>
</p>
<h1 align="center">Productive VS Code</h1>

# Table Of Contents

- [Customizing VS Code](#customizing-vs-code)
  - [Change UI Theme](#change-ui-theme)
  - [Change Icon Theme](#change-icon-theme)
  - [Change Font Family](#change-font-family)
  - [Change Font Size](#change-font-size)
  - [Turn On Ligatures](#turn-on-ligatures)
  - [Word Wrap](#word-wrap)
  - [Editor Split](#editor-split)
- [Editor](#editor)
  - [Editor Preview Mode](#editor-preview-mode)
  - [Trigger Intellisense](#trigger-intellisense)
  - [Go To Definition](#go-to-definition)
  - [Find](#find)
  - [Multi Cursor Editing](#multi-cursor-editing)
  - [Rename Symbol](#rename-symbol)
  - [Setting Sync](#setting-sync)
  - [Snippets](#snippets)
    - [Extension Based Snippets](#extension-based-snippets)
    - [User Defined Snippets](#user-defined-snippets)
  - [Open VS Code In A Folder](#open-vs-code-in-a-folder)
  - [Multi Cursor](#multi-cursor)
- [Extensions](#extensions)
  - [Settings](#settings)
    - [Disable Extensions](#disable-extensions)
    - [Recommended Extensions For Workspace](#recommended-extensions-for-workspace)
  - [Useful Extensions](#useful-extensions)
    - [`Debug Visualizer`](#debug-visualizer)
    - [`Import Cost`](#import-cost)
    - [`Markdown All In One`](#markdown-all-in-one)
    - [`markdownlint`](#markdownlint)
    - [`Dendron` Note-Taking](#dendron-note-taking)
    - [`REST Client`](#rest-client)
    - [`Thunder Client`](#thunder-client)
    - [`Tabnine AI`](#tabnine-ai)
    - [`GitHub Copilot`](#github-copilot)
    - [`Blockman - Highlight Nested Code Blocks`](#blockman---highlight-nested-code-blocks)
    - [`Error Lens`](#error-lens)
    - [`indent-rainbow`](#indent-rainbow)
    - [`Live Server`](#live-server)
    - [`Live Preview`](#live-preview)
    - [`Path Intellisense`](#path-intellisense)
  - [Git Extensions](#git-extensions)
    - [`gitignore`](#gitignore)
    - [`Version Lens`](#version-lens)
    - [`gitlink`](#gitlink)
    - [`Git Indicators`](#git-indicators)
    - [`GitLens`](#gitlens)
    - [`GitHub Pull Requests And Issues`](#github-pull-requests-and-issues)
    - [`Remote Repositories`](#remote-repositories)
  - [Multiple Projects Workflow](#multiple-projects-workflow)
    - [`Project Manager`](#project-manager)
    - [`Peacock`](#peacock)
- [Autosave \& Autoformat Workflow](#autosave--autoformat-workflow)
  - [Auto Save](#auto-save)
  - [Auto Format: `Prettier`](#auto-format-prettier)
- [Keyboard Shortcuts](#keyboard-shortcuts)
  - [Tab Management](#tab-management)
  - [Line Management](#line-management)
  - [Navigation](#navigation)

---

# Customizing VS Code

## Change UI Theme

```html
https://marketplace.visualstudio.com/items?itemName=ThePsychoCoder.psyco-coder-dark
```

> ⭐ This is my personal preference.

## Change Icon Theme

```html
https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme
```

> ⭐ This is my personal preference.

## Change Font Family

```html
https://www.jetbrains.com/lp/mono/
```

> ⭐ This is my personal preference.

- Preview fonts online

```html
https://coding-fonts.netlify.app/fonts/codelia/
```

## Change Font Size

1. Press `Ctrl` + `Shift` + `P`, then search for `setting (UI)`.
2. Search `Font Size` and change according to your preference.

## Turn On Ligatures

1. Press `Ctrl` + `Shift` + `P`, then search for `setting (json)`.
2. Add this line.

```json
    "editor.fontLigatures": true
```

> ⚠️ **Language must support font Ligatures**.

## Word Wrap

When any text runs off the side of the screen, the Word Wrap feature of VS Code consolidates it within the window and formats it perfectly.

1. Press `Ctrl` + `Shift` + `P`, then search for `setting (UI)`.
2. Search `Editor Word Wrap` and turn it `ON`.

## Editor Split

- Press `Ctrl` + `\`.

- Press `Ctrl` + `Shift` + `P`, then search for `split editor`.

# Editor

## Editor Preview Mode

When ever we single press to open a file in `VS Code`, it just shows us the `preview` of file until we type something in it.

One way to get rid out of this issue by opening file by double click.

Another way is to turn it `off` in settings.

- How we check the file is in `preview mode` or not?

> If the tab name is in `Italics`, then it is in `preview mode`, otherwise not.

## Trigger Intellisense

- Press `Ctrl` + `Space`

## Go To Definition

- Press `F12` or `right click` on mouse.
- Press `Ctrl` and click the `function`.

## Find

We can use regular expression `(regex)` to find something. Just press `alt` + `r` and press `ctrl` + `f` and write your expression.

## Multi Cursor Editing

Suppose, you are changing some repeated text one option you use is `find and replace`. Other option is, press `Ctrl` + `F` and write that text and then press `alt` + `enter`, now you have multi-line cursor and every keystroke you did can reflect to all cursor positions.

Alternatively, you can use `alt` + `mouse pointer` to the desired location to create multi-line cursor.

## Rename Symbol

Now, we are in a condition where we have to change the name of a function, one thing we can do is find and replace all but changes reflects to all the matching strings.

To solve this issue, there is an option in `VS Code`. Select the function name you want to change, press `right mouse key` and then select `Rename Symbol`. In this option, VS Code replaces all the function name everywhere it is called across the file system.

One more alternative way of doing this, we can select text and press `right mouse key` and select `Find All References`.

## Setting Sync

Having multiple devices can be clutter when we have to modify setting in all the devices one-by-one. With the `sync setting` we can use `GitHub` or `Microsoft` account to sync setting across the devices.

- Press `Account` icon present in the _bottom-left_ corner. Add your account.

## Snippets

### Extension Based Snippets

1. Press `Ctrl` + `Shift` + `X` to open extension marketplace.
2. Write `@category:"snippets"` and this will show you all the available snippets extension.
3. Press `Ctrl` + `Shift` + `P` to open `Command Palette`.
4. Search `Insert Snippet` and select it.
5. It will show you all snippets and you can insert which one you want.

### User Defined Snippets

1. Press `Ctrl` + `Shift` + `P` to open `Command Palette`.
2. Search and select `Snippets: Configure User Snippets`.
3. Now, you have option to create snippet for any language, workspace or globally. Select any of these.
4. Enter the name of snippet.
5. Now, a new file created with the name of your snippet.
6. Here is an example:

```javascript
	"Print ctrl": {
		"scope": "markdown",
		"prefix": "ctrl",
		"body": [
			"`Ctrl` + $0"
		],
		"description": "Print the Ctrl Button in Markdown"
	}
```

7. Now, when ever you type the `{prefix}`, it will shows the option to select the snippet.

> Snippet guide available in the starting of your snippet file with an example.

## Open VS Code In A Folder

- Using Terminal

```bash
code folderName
```

- Using Context Menu

**One time setup**:

1. Press `Ctrl` + `Shift` + `P` to open the Command Palette.
2. Type `shell command` and select `Shell Command: Install 'code' command in PATH`.

This will add the code command to your system PATH, so that you can launch VS Code from anywhere on your computer by typing code in a terminal window.

Now, open desired folder you want to open in VS Code and press `right mouse` key, you will see `Open With Code` option there.

## Multi Cursor

One way is to hold `Alt` + `Right click` on mouse where every you want to create another cursor. Or like this:

<center>
<img src="https://raw.githubusercontent.com/DhananjayPorwal/productive-vs-code/main/Sources/auto-cursor.gif" alt="auto-cursor">
</center>

- Press `Shift` + `Alt` + `Mouse Selection`.

Another and more efficient way of creating multi cursor is:

1. Select the word you want.
2. Press `Ctrl` + `D` you create multi cursors.

**OR**

1. Press `Ctrl` + `Shift` + `Alt` + `Up\Down Arrow` to create multi-cursor in same columns.

> Press `Esc` to exit multi-cursor.

# Extensions

## Settings

### Disable Extensions

> **More extensions -> slower the IDE**

Some project doesn't required all the extension we installed. So, we can disable them for particular workspace or project.

1. Press `Ctrl` + `Shift` + `X`.
2. Navigate to the plugin you want to disable.
3. Press the `gear` or `setting` icon.
4. Select `Disable For Workspace`.

### Recommended Extensions For Workspace

While working on a project, you installed some extensions. You want to recommended list of extension whoever use this project. One way is to list down all the extension and that use install them one by one.

Now, `VS Code` provides use a functionality by which, we can add recommended extension to the user using the project.

1. Press `Ctrl` + `Shift` + `P`.
2. Type `Recommended Extension` and select it.
3. Now, it will open a new file named `extension.json`.
4. In the `extension.json` file, you will find `recommendations` array.
5. After that, we just have to copy extension id from the extension page and paste in the array with double quotes.

Now, when ever someone open your project in `VS Code`, it will show a **pop-up** for _recommending extension_, which can be installed using one click.

## Useful Extensions

### `Debug Visualizer`

A visual watch window that lets you visualize your data structures while debugging.

<center>
<img src="https://raw.githubusercontent.com/DhananjayPorwal/productive-vs-code/main/Sources/debug-visualizer.gif" alt="import-cost">
</center>

### `Import Cost`

Display import/require package size in the editor.

<center>
<img src="https://raw.githubusercontent.com/DhananjayPorwal/productive-vs-code/main/Sources/import%20cost.gif" alt="import-cost">
</center>

### `Markdown All In One`

All you need to write Markdown (keyboard shortcuts, table of contents, auto preview and more).

### `markdownlint`

Markdown/CommonMark linting and style checking for Visual Studio Code.

### `Dendron` Note-Taking

Dendron is an open-source, local-first, markdown-based, note-taking tool. It's a personal knowledge management solution (PKM) built specifically for developers and integrates natively with IDEs like VSCode.

### `REST Client`

REST Client allows you to send HTTP request and view the response in Visual Studio Code directly.

### `Thunder Client`

Thunder Client is a lightweight Rest API Client Extension for Visual Studio Code with simple and clean design.

### `Tabnine AI`

AI coding assistant with AI code completions and AI code chat right in the IDE, helping developers by generating code, writing unit tests and documentation, explaining legacy code, and much more. Tabnine supports all major languages including JavaScript, Python, Java, Typescript c/c++ and more.

### `GitHub Copilot`

Your AI pair programmer.

### `Blockman - Highlight Nested Code Blocks`

VS Code Extension For Nested Block Highlighting

### `Error Lens`

Improve highlighting of errors, warnings and other language diagnostics.

### `indent-rainbow`

A simple extension to make indentation more readable

### `Live Server`

Launch a development local Server with live reload feature for static & dynamic pages.

### `Live Preview`

An extension that hosts a local server for you to preview your web projects on. This extension is most useful for projects where a server is not already created (e.g. not for apps using React, Angular, etc.). To work with these, feel free to run the Simple Browser: Show command that is already built-in with VS Code.

### `Path Intellisense`

Visual Studio Code plugin that autocompletes filenames.

## Git Extensions

### `gitignore`

This extension lets you pull `.gitignore` templates from `github/gitignore`.

1. Install extension `gitignore` from the marketplace .
2. Press `Ctrl` + `Shift` + `P`.
3. Search for `add gitignore`.
4. Now, you have to select the technology of your project.

### `Version Lens`

Shows the latest version for each package using code lens.

<center>
<img src="https://raw.githubusercontent.com/DhananjayPorwal/productive-vs-code/main/Sources/version%20lens.gif" alt="version-lens">
</center>

### `gitlink`

Goto/Copy current file's online link, supports multiple remote sources in GitHub/GitLab/BitBucket/VSTS/DevOps.

### `Git Indicators`

Git indicator in the status bar.

### `GitLens`

Supercharge Git and unlock untapped knowledge within your repository to better understand, write, and review code. Focus, collaborate, accelerate.

### `GitHub Pull Requests And Issues`

Review and manage your GitHub pull requests and issues directly in VS Code

### `Remote Repositories`

The Remote Repositories extension integrates with the GitHub Repositories and Azure Repos extensions, allowing you to quickly browse, search, edit, and commit to remote git repositories directly from within Visual Studio Code.

## Multiple Projects Workflow

### `Project Manager`

It helps you to easily access your projects, no matter where they are located. Don't miss those important projects anymore. You can define your own Projects (also called Favorites), or choose for auto-detect Git, Mercurial or SVN repositories, VSCode folders, or any other folder.

### `Peacock`

Subtly change the workspace color of your workspace. Ideal when you have multiple VS Code instances and you want to quickly identify which is which.

# Autosave & Autoformat Workflow

## Auto Save

- Why?
  - Remove time to format.
  - Remove milliseconds of thought.
  - Focus on code.
  - Enforce styles across team.

1. Open `Settings (UI)`.
2. Search `Auto Save`.
3. Change `Files: Auto Save` to `afterDelay`.

<center>
<img src= "https://raw.githubusercontent.com/DhananjayPorwal/productive-vs-code/main/Sources/autosave.png" alt = "auto-save">
</center>

Now, whenever you stop typing, `VS Code` will automatically save your file after `1000` milliseconds.

## Auto Format: `Prettier`

Prettier is an opinionated code formatter. It enforces a consistent style by parsing your code and re-printing it with its own rules that take the maximum line length into account, wrapping code when necessary.

Now, after installing this extension we have to manually select this extension to `Format Document` once.

1. Open `Setting UI`.
2. Search `Default Formatter`.
3. Select `Prettier`.

<center>

<img src = "https://raw.githubusercontent.com/DhananjayPorwal/productive-vs-code/main/Sources/Prettier.png" alt="prettier"></center>

After this, we can automate auto formatting using `Setting (UI)`.

1. Open `Setting UI`.
2. Search `Format On Save`.
3. Check the box with title `Editor: Format On Save`.

<center>

<img src="https://raw.githubusercontent.com/DhananjayPorwal/productive-vs-code/main/Sources/autoformat.png" alt = auto-format></center>

# Keyboard Shortcuts

> **Official Documentation**: https://code.visualstudio.com/docs/getstarted/keybindings

1. Open Command Palette.
2. Search `Keyboard Shortcut Reference`.
3. Select `Help: Keyboard Shortcut Reference`.

It will navigate you to the [VS Code shortcut keys pdf](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf).

> Next **Sub-Sections** are specifically for **Windows** based `VS Code Installation`. You can follow above method to find shortcut key for your **operating system**.

## Tab Management

| Key                    | Work                       |
| ---------------------- | -------------------------- |
| `Ctrl` + `N`           | Open New File              |
| `Ctrl` + `P`           | Open a File                |
| `Ctrl` + `W`           | Close File                 |
| `Ctrl` + `\`           | Split Editor               |
| `Ctrl` + `1`           | Jump into 1st Editor Group |
| `Ctrl` + `2`           | Jump into 2nd Editor Group |
| `Ctrl` + `Tab`         | Cycle Tabs                 |
| `Ctrl` + `Shift` + `T` | Reopens Closed Tabs        |

## Line Management

| Key                            | Work               |
| ------------------------------ | ------------------ |
| `Ctrl` + `Up Arrow`            | Moves Line Up      |
| `Ctrl` + `Down Arrow`          | Moves Line Down    |
| `Shift` + `Alt` + `Up Arrow`   | Copy Line Up       |
| `Shift` + `Alt` + `Down Arrow` | Copy Line Down     |
| `Ctrl` + `Shift` + `Enter`     | Insert Line Above  |
| `Ctrl` + `Enter`               | Insert Line Below  |
| `Ctrl` + `]`                   | Insert Indentation |
| `Ctrl` + `/`                   | Insert Comments    |

## Navigation

| Key                    | Work                   |
| ---------------------- | ---------------------- |
| `Ctrl` + `G`           | Go To Line             |
| `Ctrl` + `T`           | Go To Symbol           |
| `F12`                  | Go To Definition       |
| `F12`                  | Go To Definition       |
| `Ctrl` + `Shift` + `\` | Go To Matching Bracket |
| `Ctrl` + `Shift` + `P` | Go To Command Palette  |
| `Ctrl` + `Shift` + `P` | Go To Command Palette  |
| `Ctrl` + $`$           | Open/Close Terminal    |

---

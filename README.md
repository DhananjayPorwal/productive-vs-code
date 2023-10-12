<p align="center">
<img src="Sources/icon.png" height="130" width="130"/>
</p>
<h1 align="center">Productive VS Code</h1>

# Customizing VS Code

## Change UI Theme

```html
https://marketplace.visualstudio.com/items?itemName=ThePsychoCoder.psyco-coder-dark
```

## Change Icon Theme

```html
https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme
```

## Change Font Family

```html
https://www.jetbrains.com/lp/mono/
```

+ Preview fonts online

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

## Word Wrap

1. Press `Ctrl` + `Shift` + `P`, then search for `setting (UI)`.
2. Search `editor word wrap` and turn it `on`.

## Editor Split

+ Press `Ctrl` + `\`.

+ Press `Ctrl` + `Shift` + `P`, then search for `split editor`.

# Editor

## Editor Preview Mode

When ever we single press to open a file in `VS Code`, it just shows us the `preview` of file until we type something in it. 

One way to get rid out of this issue by opening file by double click.

Another way is to turn it `off` in settings. 

+ How we check the file is in `preview mode` or not?

> If the tab name is in `Italics`, then it is in `preview mode`, otherwise not.


## Trigger Intellisense

+ Press `Ctrl` + `Space`

## Go To Definition

+ Press `F12` or `right click` on mouse.
+ Press `Ctrl` and click the `function`.

## Find

We can use regular expression `(regex)` to find something. Just press `alt` + `r` and press `ctrl` + `f` and write your expression.

## Multi Cursor Editing

Suppose, you are changing some repeated text one option you use is `find and replace`. Other option is, press `Ctrl` + `F` and write that text and then press `alt` + `enter`, now you have multi-line cursor and every keystroke you did can reflect to all cursor positions.

Alternatively, you can use `alt` + `mouse pointer` to the desired location to create multi-line cursor.

## Rename Symbol

Now, we are in a condition where we have to change the name of a function, one thing we can do is find and replace all but changes reflects to all the matching strings.

To solve this issue, there is an option in `VS Code`. Select the function name you want to change, press `right mouse key` and then select `Rename Symbol`. In this option, VS Code replaces all the function name everywhere it is called across the file system.

One more alternative way of doing this, we can select text and press `right mouse key` and select `Find All References`.

# Extensions

## Disable Extensions

> More extensions -> slower the IDE.

Some project doesn't required all the extension we installed. So, we can disable them for particular workspace or project.

1. Press `Ctrl` + `Shift` + `X`.
2. Navigate to the plugin you want to disable.
3. Press the `gear` or `setting` icon.
4. Select `Disable For Workspace`.

## Recommended Extensions For Workspace

While working on a project, you installed some extensions. You want to recommended list of extension whoever use this project. One way is to list down all the extension and that use install them one by one.

Now, `VS Code` provides use a functionality by which, we can add recommended extension to the user using the project.

1. Press `Ctrl` + `Shift` + `P`. 
2. Type `Recommended Extension` and select it.
3. Now, it will open a new file named `extension.json`.
4. In the `extension.json` file, you will find `recommendations` array. 
5. After that, we just have to copy extension id from the extension page and paste in the array with double quotes.

Now, when ever someone open your project in `VS Code`, it will show a **pop-up** for *recommending extension*, which can be installed using one click.

## Setting Sync

Having multiple devices can be clutter when we have to modify setting in all the devices one-by-one. With the `sync setting` we can use `GitHub` or `Microsoft` account to sync setting across the devices.

+  Press `Account` icon present in the *bottom-left* corner. Add your account.

## Snippets

### Extension Based Snippets

1. Press `Ctrl` + `Shift` + `X` to open extension marketplace.
2. Write `@category:"snippets"` and this will show you all the available snippets extension.
3. Press `Ctrl` + `Shift` + `P` to open `Command Palette`.
4. Search `Insert Snippet` and select it.
5. It will show you all snippets and you can insert which one you want.

### User Defined Snippets


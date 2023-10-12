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

+ Press `Ctrl` + `Shift` + `P`, then search for `setting (UI)`.
+ Search `Font Size` and change according to your preference.

## Turn On Ligatures

+ Press `Ctrl` + `Shift` + `P`, then search for `setting (json)`.
+ Add this line.

```json
    "editor.fontLigatures": true
```

## Word Wrap

+ Press `Ctrl` + `Shift` + `P`, then search for `setting (UI)`.
+ Search `editor word wrap` and turn it `on`.

## Editor Split

+ Press `Ctrl` + `\`.

**OR**

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

To solve this issue, there is an option in `VS Code`. Select the function name you want to change, press `right mouse key` and then select `Rename Symbol`. In this option, VS Code replaces all the function name everywhere it is called.

One more alternative way of doing this, we can select text and press `right mouse key` and select `Find All References
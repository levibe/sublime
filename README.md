# Sublime settings and snippets 

Boxy Ocean theme with customized preferences.

Javascript, Node, and Vue snippets with no semicolons and tab indenting.

See [Setup How to](#setup)

# Snippets

## CSS

**com**  
`/* $1 */ $0`

**dib**  
`display: inline-block; `

**hs**  
`$1 h1, $1 h2, $1 h3, $1 h4, $1 h5, $1 h6 { $2 } `

**pabs**  
`position: absolute; `

**pafull**  
`position: absolute; top: 0; right: 0; bottom: 0; left: 0; `

**pfix**  
`position: fixed; `

**prel**  
`position: relative; `

**rgb**   
`rgb(${1:255}, ${2:255}, ${3:255}); $0`

**rgba**  
`rgba(${1:255}, ${2:255}, ${3:255}, ${4:1}); $0`

**tac**  
`text-align: center; `

**tra**  
`transition: ${1:all} ${2:0.15}s ${3:ease}; `

**vat**  
`vertical-align: top; `

**:aft**  
`:after { $1 content: ''; } `

**:bef**  
`:before { $1 content: ''; } `


### Chunks

**cols**  
```
.${1:class} { $2 }
    .${1:class} li { width: ${3:33%}; display: inline-block; }
$0
```

**fbase**
```
form { $1 }
    input[type='text'], textarea { $2 }
    input[type='submit'] { $3 }
```


### Partials

**base**  
```
/* General & Resets */

* { box-sizing: border-box; }
html, body { height: 100%; width: 100%; margin: 0; padding: 0; color: #444; }
body, input, select, textarea, button { font-family: "Helvetica Neue", Helvetica, Arial, sans-serif; }

p { line-height: 120%; }
ul { margin-bottom: 0; }

a, button { outline: none; transition: all 0.15s ease; }

$1
```

**responsive**  
```
/* Responsive */

@media handheld and (max-width: 1200px), screen and (max-device-width: 1200px), screen and (max-width: 1200px)  {
	.wrapper { width: 960px; }
}

@media handheld and (max-width: 960px), screen and (max-device-width: 960px), screen and (max-width: 960px)  {
	.wrapper { width: auto; min-width: 0; margin-left: 20px; margin-right: 20px; }
	$1
}

@media handheld and (max-width: 740px), screen and (max-device-width: 740px), screen and (max-width: 740px)  {
	$2
}
```

## HTML






<a name="setup">
## Setup

### Set up theme
- Download Roboto from Google Fonts (for Terminal)

- Install Package Control:
`Cmd + Shift + P` -> `Install Package Manager`

- Install Boxy Ocean theme through Package Manager

- Set up a symlink between repo preferences and sublime preferences, e.g. `ln -s ~/Projects/sublime/Preferences.sublime-settings ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User/Preferences.sublime-settings`

### Link snippets
- Set up a symlink between this repo's snippets folder and Sublime's User Settings folder, e.g. `ln -s ~/Projects/sublime/Snippets/ ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User/`


## Why use Sublime?

It's simple and fast:  
https://pavelfatin.com/typing-with-pleasure/  
https://blog.xinhong.me/post/sublime-text-vs-vscode-vs-atom-performance-dec-2016/

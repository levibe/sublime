# Sublime settings and snippets 

Boxy Ocean theme with customized preferences. See [Setup](#setup)


# Snippets

Javascript style is no semicolons and tab indenting.

* [CSS](#css)
* [HTML](#html)
* [Javascript](#js)
* [Node](#node)
* [Vue](#vue)


<a name="css">
# CSS

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
*Base CSS file with some simple defaults*

**responsive**  
*Responsive media query template*



<a name="html">
# HTML

**a**  
`<a href="$1">$2</a>$0`

**base**  
Base HTML template

**c**  
`<${1:component}$2></${1:component}>$0`

**cr**  
`Copyright &copy; $1. $0`

**ga**  
*Google Analytics snippet*



<a name="js">
# Javascript

**cl**  
`console.log($1)$0`

**si**  
```
setInterval(function() {
	${2}
}, ${1:1000})$0
```

**st**  
```
setTimeout(function() {
	${2}
}, ${1:1000})$0
```


<a name="node">
# Node

**me**  
`module.exports = ${1:name}`

**pe**  
`process.exit(${1:0})$0`

**re**  
`var ${1:module} = require('${1:module}')$0`




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

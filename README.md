# Sublime settings and snippets 

Boxy Ocean theme with customized preferences. See [Setup](#setup) for info on how to set up your Sublime Text for these snippets.

* [CSS](#css)
* [HTML](#html)
* [Javascript](#js)
* [Node](#node)
* [Vue](#vue)


# Snippets

<a name="css"></a>
## CSS

**anim**  
``animation: ${1:name} 0.5s linear 0s forwards; ``

**bsh**  
`box-shadow: ${1:0} ${2:1px} ${3:5px} rgba(0,0,0,${4:0.15}); $0`

**com**  
*Add a comment, useful for headings*  
`/* $1 */ $0`  

**cd**  
`cursor: default; `

**cp**  
`cursor: pointer; `

**db**  
`display: block; `

**df**  
`display: flex; `

**di**  
`display: inline; `

**dib**  
`display: inline-block; `

**dn**  
`display: none; `

**fs**  
`font-size: $1;$0`

**fw**  
`font-weight: ${1:400};$0`

**key**  
```
@keyframes $1 {
	0% { $2 }
	100% { $3 }
}
```

**hs**  
`$1 h1, $1 h2, $1 h3, $1 h4, $1 h5, $1 h6 { $2 } `

**mau**  
`margin: ${1:0} auto; $0`

**noselect**  
`user-select: none;`

**oh**  
`overflow: hidden;`

**op**  
`opacity: ${1:1}; $0`

**pabs**  
`position: absolute; `

**pafill**  
`position: absolute; top: 0; right: 0; bottom: 0; left: 0; `

**pr**  
`padding-right: $1; $0`

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

**tal**  
`text-align: left; `

**tar**  
`text-align: right; `

**tra**  
`transition: ${1:all} ${2:0.15}s ${3:ease}; `

**tsh**  
`text-shadow: ${1:0} ${2:1px} ${3:5px} rgba(0,0,0,${4:0.15}); $0`

**vat**  
`vertical-align: top; `

**:aft**  
`:after { $1 content: ''; } `

**:bef**  
`:before { $1 content: ''; }` 

**:fc**  
`:first-child { $1 } `

**:lc**  
`:last-child { $1 } `


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
*[Base CSS file](https://github.com/levibe/sublime/blob/master/Snippets/css/base.sublime-snippet) (with simple common settings)*

**responsive**  
*[Responsive media query](https://github.com/levibe/sublime/blob/master/Snippets/css/responsive.sublime-snippet) (with simple common settings)*



<a name="html"></a>
# HTML

**a**  
`<a href="$1">$2</a>$0`

**base**  
*[Base HTML template](https://github.com/levibe/sublime/blob/master/Snippets/html/base.sublime-snippet)*

**c**  
`<${1:component}$2></${1:component}>$0`

**com**  
*Add a comment*  
`<!-- $1 -->$0`

**ga**  
*[Google Analytics snippet](https://github.com/levibe/sublime/blob/master/Snippets/html/google-analytics.sublime-snippet)*



<a name="js"></a>
# Javascript

Javascript style is no semicolons and tab indenting.

**cl**  
`console.log($1)$0`

**com**  
*Add a comment*  
`/* $1 */ $0`  

**method**
```
${1:name}: function ($2) {
		$3
},
```

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

**vst**  
`var self = this`



<a name="node"></a>
# Node

**me**  
`module.exports = ${1:name}`

**pe**  
`process.exit(${1:0})$0`

**re**  
`var ${1:module} = require('${1:module}')$0`



<a name="vue"></a>
# Vue

**import**  
`import ${1:module} from './${1:module}'$0`

**vcdata**  
```
data () {
	return {
		${1:name}: ${2:data}
	}
},$0
```

**vcomponent**  
*[Base Vue component](https://github.com/levibe/sublime/blob/master/Snippets/vue/vue-component.sublime-snippet)*

**vdirective**  
*[Base Vue directive](https://github.com/levibe/sublime/blob/master/Snippets/vue/vue-directive.sublime-snippet)*

---

<a name="setup"></a>
# Setup

### Set up theme
- Install Package Control:
`Cmd + Shift + P` -> `Install Package Manager`

- Install Boxy Ocean theme through Package Manager

- Set up a symlink between repo preferences and sublime preferences, e.g. `ln -s ~/Projects/sublime/Preferences.sublime-settings ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User/Preferences.sublime-settings`

  
### Link snippets
- Set up a symlink between this repo's snippets folder and Sublime's User Settings folder, e.g. `ln -s ~/Projects/sublime/Snippets/ ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User/`


## Why Sublime?

It's simple and fast:  
https://pavelfatin.com/typing-with-pleasure/  
https://blog.xinhong.me/post/sublime-text-vs-vscode-vs-atom-performance-dec-2016/

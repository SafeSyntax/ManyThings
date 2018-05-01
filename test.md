
#### Test <br> 
# Another <br>
<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> <mark>| command prompt |</mark>

Hellow **World!**  
*What's about you?*

```
#include <isotream>  
using namespace std;  
  int mian() {
  sdfs
  }
 ```

> Just a qoute 

This site was built using [Safe Syntax](https://safesyntax.com/).

* Item 1
* Item 2
* Item 3

- List 
  - Another
  
  - [x] Finish my changes
- [ ] Push my commits to GitHub
- [ ] Open a pull request


| Command | Description |
| --- | --- |
| git status | List all new or modified files |
| git diff | Show file differences that haven't been staged |
| git status | List all new or modified files |
| git status | List all new or modified files |


| Shortcut | Description |
| ---------| ----------- |
| <kbd>Ctrl</kbd>+<kbd>P</kbd> | go to file |
| <kbd>Ctrl</kbd>+<kbd>G</kbd> | go to line |
| <kbd>Ctrl</kbd>+<kbd>R</kbd> | go to methods |
| <kbd>Ctrl</kbd>+<kbd>K</kbd><kbd>B</kbd> | toggle side bar |
| <kbd>Ctrl</kbd>+<kbd>N</kbd> | new window |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>N</kbd> | new window |


## Quick way to code at Sublime Text

#### Child: >

div>ul>li
```
<div>
    <ul>
        <li></li>
    </ul>
</div>
```

#### Sibling: +

div+p+bq

<div></div>
<p></p>
<blockquote></blockquote>

div+div>p>span+em 
```
<div></div>
<div>
    <p><span></span><em></em></p>
</div>
```


#### Climb-up: ^

With ^ operator, you can climb one level up the tree and change context where following elements should appear:

div+div>p>span+em^bq
```
<div></div>
<div>
    <p><span></span><em></em></p>
    <blockquote></blockquote>
</div>
```

You can use as many ^ operators as you like, each operator will move one level up:

div+div>p>span+em^^^bq
```
<div></div>
<div>
    <p><span></span><em></em></p>
</div>
<blockquote></blockquote>
```

#### Multiplication: *

ul>li*5
...outputs to
```
<ul>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
</ul>
```

#### Grouping: ()

div>(header>ul>li*2>a)+footer>p
```
<div>
    <header>
        <ul>
            <li><a href=""></a></li>
            <li><a href=""></a></li>
        </ul>
    </header>
    <footer>
        <p></p>
    </footer>
</div>
```

(div>dl>(dt+dd)*3)+footer>p
```
<div>
    <dl>
        <dt></dt>
        <dd></dd>
        <dt></dt>
        <dd></dd>
        <dt></dt>
        <dd></dd>
    </dl>
</div>
<footer>
    <p></p>
</footer>
```

#### ID and CLASS

div#header+div.page+div#footer.class1.class2.class3
```
<div id="header"></div>
<div class="page"></div>
<div id="footer" class="class1 class2 class3"></div>
```
Custom attributes

td[title="Hello world!" colspan=3]
```
<td title="Hello world!" colspan="3"></td>
```
Note:  
You can use single or double quotes for quoting attribute values.
You don’t need to quote values if they don’t contain spaces: td[title=hello colspan=3] will work.

#### Item numbering: $

ul>li.item$*5
```
<ul>
    <li class="item1"></li>
    <li class="item2"></li>
    <li class="item3"></li>
    <li class="item4"></li>
    <li class="item5"></li>
</ul>
```
You can use multiple $ in a row to pad number with zeroes:

ul>li.item$$$*5
```
<ul>
    <li class="item001"></li>
    <li class="item002"></li>
    <li class="item003"></li>
    <li class="item004"></li>
    <li class="item005"></li>
</ul>
```
Changing numbering base and direction
With @ modifier, you can change numbering direction (ascending or descending) and base (e.g. start value).

For example, to change direction, add @- after $:

ul>li.item$@-*5
```
<ul>
    <li class="item5"></li>
    <li class="item4"></li>
    <li class="item3"></li>
    <li class="item2"></li>
    <li class="item1"></li>
</ul>
```
To change counter base value, add @N modifier to $:

ul>li.item$@3*5
…transforms to
```
<ul>
    <li class="item3"></li>
    <li class="item4"></li>
    <li class="item5"></li>
    <li class="item6"></li>
    <li class="item7"></li>
</ul>
```
You can use these modifiers together:

ul>li.item$@-3*5
…is transformed to
```
<ul>
    <li class="item7"></li>
    <li class="item6"></li>
    <li class="item5"></li>
    <li class="item4"></li>
    <li class="item3"></li>
</ul>
```

#### Text: {}

a{Click me}
```
<a href="">Click me</a>
```
Note that {text} is used and parsed as a separate element (like, div, p etc.) but has a special meaning when written right after element. For example, a{click} and a>{click} will produce the same output, but a{click}+b{here} and a>{click}+b{here} won’t:

<!-- a{click}+b{here} -->
````
<a href="">click</a><b>here</b>
````
<!-- a>{click}+b{here} -->
````
<a href="">click<b>here</b></a>
````
In second example the <b> element is placed inside <a> element. And that’s the difference: when {text} is written right after element, it doesn’t change parent context. Here’s more complex example showing why it is important:

p>{Click }+a{here}+{ to continue}
````
<p>Click <a href="">here</a> to continue</p>
````

p{Click }+a{here}+{ to continue}
...produces

<p>Click </p>
```
<a href="">here</a> to continue
````




## bootstrap autocomple how to
Preferences > Package Control > Package Control : Install Package > write Bootstrap 4 Autocomplete


## Bootstrap 3 Snippet
- [Bootstrap 3 Snippet](https://github.com/JasonMortonNZ/bs3-sublime-plugin)  
- [Bootstrap 4 Snippet](https://github.com/degouville/sublime-bootstrap4)


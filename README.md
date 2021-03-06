SmartDuplicate
==============

SmartDuplicate is a Sublime Text 2 and 3 plug-in that allows duplicating lines while changing certain keywords.

Installation
------------

* Using [Package Controller](http://wbond.net/sublime_packages/package_control) (recommended):
Call _Install Package_ and look for __SmartDuplicate__.

* Manually:
Clone repo into your packages folder (in Subime: _Preferences_ > _Browse Packages..._ menu item to open this folder).


Command
-------

**[CTRL+SHIFT+d]** (or **[CMD+SHIFT+d]** for OSX) duplicates line using smart duplicate

_Note: This overwrites the default duplicate line shortcut._


Examples
--------

I wrote the first line of the pairs and hit **[CTRL+SHIFT+d]**.

```
Grid.WIDTH = window.innerWidth();
Grid.HEIGHT = window.innerHeight();

element.x = other.width + 20 + element.width;
element.y = other.height + 20 + element.height;

target.x = stage.mouseX;
target.y = stage.mouseY;

marginTop: "30px"
marginBottom: "30px"

padding-left: 20px;
padding-right: 20px;
```


Supported keywords
------------------

* `width` <-> `height` (case insensitive)
* `left` <-> `right` (case insensitive)
* `top` <-> `bottom` (case insensitive)
* `.x` <-> `.y`
* `.[word]X` <-> `.[word]Y`  (any word ending in a capital X or Y)

__Once again: work in progress. Constantly expanding and fine tuning the keywords__


Motivation
----------

I'm a front-end developer. It's been too many times that I duplicate a line and then go through and change all the
`.height` to `.width` etc.. In the manner of __automate all the things__ I thought I write a little plugin for the editor
of my choice.

Let me know what you think. No _you suck_-emails please.
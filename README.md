Middleman Template: Famous
==========================
This is Middleman with Foundation 5, Haml, Sass and Bower; Middleman
Famous.

It's aim is to be minimal and provide quick scaffolding to web projects.
It also uses some goodies like Livereload and a Google Analytics
snippet.

There is no content by default, so you have no fluff to remove.

You're all set!

## (The same, in readable) Bullet points!
* Middleman 3.3
* Foundation 5
* HAML
* Bower
* Livereload
* No content, just the frame
* Google Analytics

## Goodies
### Two-tier Layouts
In the layout folder, I put two layouts: `base`, and `layout`.
Basically, `layout` is `base` plus a frame to support stand-alone text.

That means you can drop in Markdown files which will layout correctly
in the grid without any more markup; while allowing you to customize
how your crafted HAML views look.

So for example, we can drop in `about.md` which will work as a
stand-alone document and use `layout`; as well as have `home.html.haml`
that will use `base` and configure rows in `home` rather than being in
the layout.

For this to work, you only have to add `layout: base` in the
front-matter.

## Usage
### Install

    $ git clone git://github.com/joallard/middleman-famous ~/.middleman/famous

### Create

    $ middleman init [foo] --template=famous
    $ cd [foo]
    $ rm README.md    # because it's annoying
    $ bower install   # provided Bower is installed

### Upgrade once in a while

    $ cd ~/.middleman/famous
    $ git pull [--rebase]   # rebase if you've made committed changes

## To do

* Make a branch for those who don't need the JS
* Make Analytics adaptable?
* Clean up CSS

Corrections welcome. Enjoy!

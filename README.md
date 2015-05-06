# swarm-graphics
Reskin Swarm Simulator with CSS. No changes to the Swarmsim code required! Create and share your own Swarmsim skin!

edit css: https://github.com/erosson/swarm-graphics/tree/gh-pages

view css: https://erosson.github.io/swarm-graphics/graphics.css

after v1.0.37, to use custom styling:
* with one click: [Standalone](https://swarmsim.github.io/#/cleartheme?themeExtra=@import url%28'https://test.swarmsim.com/swarm-graphics/graphics.css'%29;) , [Kongregate](https://www.swarmsim.com?kongregate=1/#/cleartheme?themeExtra=@import url%28'https://test.swarmsim.com/swarm-graphics/graphics.css'%29;)
* or [options > theme > `Additional styling (advanced)`](http://i.imgur.com/cB5oMiH.png?1) > paste `@import url('https://test.swarmsim.com/swarm-graphics/graphics.css');`
  * The CSS import must be _http**s**://_, not _http://_!

git will host your css files for free. steps:
* create github account
* create a repository
* switch to your repository's gh-pages branch: http://github.com/{{your-account-name}}/{{your-repository-name}}/tree/gh-pages
* edit and commit your css file there. the "+" at the top adds a file.
* go to https://{{your-account-name}}.github.io/{{your-repository-name}}/graphics.css

relevant css classes:

* `icon-{{name}}` to insert graphics. `tab-icon`, `desc-icon`, `list-icon`, `unselectedlist-icon` to control style for the icon in different locations. use with background-url to insert images into tabs/descriptions/lists. Replace `{{name}}` with a unit name from [the spreadsheet](https://docs.google.com/a/swarmsim.com/spreadsheets/d/1ughCy983eK-SPIcDYPsjOitVZzY10WdI2MGGrmxzxF4/pubhtml), or see kittens.css for many examples of inserting images.
* unit names: `label-{{name}}`, with different locations controlled by `.tab-label`, `.selected-label`, `.list-label`, `.unselectedlist-label`. Each of those has children broken into two parts, `.label-label`, and `.label-suffix`. Look in kittens.css for "mewtagen" for an example of changing a unit name.
* unit descriptions: `desc-{{name}}`. For an example of changing a unit description, see kittens.css: `.desc-meat`.

Kitten Klicker, the Swarmsim 2015 April Fools joke, is a good example of what CSS skins are capable of changing. No code changes; it was all CSS. [Standalone](https://swarmsim.github.io/#/cleartheme?themeExtra=@import url%28'https://test.swarmsim.com/swarm-graphics/kittens.css'%29;), [Kongregate](https://www.swarmsim.com?kongregate=1/#/cleartheme?themeExtra=@import url%28'https://test.swarmsim.com/swarm-graphics/kittens.css'%29;)

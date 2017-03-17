# Spirits

![screenshot](http://i.imgur.com/qbS29GT.jpg)
First version : DON'T LOSE YOUR WAY

![screenshot](http://i.imgur.com/fmR7mr6.jpg)
Second version : A BELIEVING HEART IS YOUR MAGIC

![screenshot](http://i.imgur.com/siiXX9p.jpg)
Third version : ROW ROW FIGHT THE POWER 

What's a startpage/homepage ?
-------------------------------

It's a local website, namely you'll be able to access it thanks to files present on your computer (in general, it'll be a .htm file), and some browser like Firefox Mozilla and Google Chrome will allow you to set a custom homepage. What's more, thanks to some add-ons/extensions such as 'New Tab Homepage' for FF or 'New Tab Redirect' for Chrome, you'll be able to set this said startpage as you new tab page (amazing isn't it ?). There are a lot of custom startpage on the net, you can check this list of startpage http://startpages.github.io/ or search some of them on github/deviantart. 

What's the structure of 'Spirits' ?
-------------------------------

There are 4 differents folders and two files (.htm and .css) : 
- the first folder 'background' contains, well, the background I used, there are three ones, if you want to change them or add some more, rename them like 'background04.jpg', it'll be easier to edit it in the others files.
- in the second folder 'banner' you'll find, surprise, the three differents banners I made for the startpage featuring Mako Mankanshoku from Kill La Kill, Sucy Manbavaran from Little Witch Academia and Nia Teppelin from Tengen Toppa Gurren Lagann (I really like these shows). Like the background, if you want to change the banner or add others ones, add the files in this folder and name them 'banner4.jpg'.
- the icons folder has the icons I used, there are only three : the favicon (ie the icon in the tab), the search and enter icons.
- the js folder is very important since you'll have to edit some files to add banner/background or modify some functionalities.
- the .htm file is the most important file since you'll need it to open the startpage on your browser, if you want to change the structure of the startpage you'll have to edit it.
- the .css file will be needed if you want to change the aspect of the startpage, namely the background, the font-family, the size of a picture, etc.

How can I customize 'Spirits' ?
-------------------------------

### LINKS :
- open the .htm file in a text editor (personally I use Sublime), search for 'LINK1' and replace it by the name of a website you visit frequently (for exemple Facebook). 
- after that, change the 'http://link1.com/' with the URL of the said site (if we take Facebook, it'll be https://www.facebook.com/).
- if you want to add a link,                                         

``` htm 
<a href="http://link1.com/">
    <li> LINK1 </li>
</a> 
```

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
- the first folder `background` contains, well, the background I used, there are three ones, if you want to change them or add some more, rename them like `background04.jpg`, it'll be easier to edit it in the others files.
- in the second folder `banner` you'll find, surprise, the three differents banners I made for the startpage featuring Mako Mankanshoku from Kill La Kill, Sucy Manbavaran from Little Witch Academia and Nia Teppelin from Tengen Toppa Gurren Lagann (I really like these shows). Like the background, if you want to change the banner or add others ones, add the files in this folder and name them `banner4.jpg`.
- the `icons` folder has the icons I used, there are only three : the favicon (ie the icon in the tab), the search and enter icons.
- the `js` folder is very important since you'll have to edit some files to add banner/background or modify some functionalities.
- the `.htm` file is the most important file since you'll need it to open the startpage on your browser, if you want to change the structure of the startpage you'll have to edit it.
- the `.css` file will be needed if you want to change the aspect of the startpage, namely the background, the font-family, the size of a picture, etc.

Features of 'Spirits'
-------------------------------

There are two main features :
- first, the button `SHUFFLE`, by clicking it you'll be able change the banner/background of the startpage, it'll be at random, otherwise it won't be fun !
- second, in the search bar, by entering some special keys, such as `-y jazz music`, you'll be able to search directly on youtube and not on Google. Another exemple with `-w moe`, it'll search 'moe' on wikipedia. I took the code from a startpage called 'Gokouri', can't seem to find it anymore on github tho.

How can I customize 'Spirits' ?
-------------------------------

### LINKS :

- open the `.htm` file in a text editor (personally I use Sublime), search for `LINK1` and replace it by the name of a website you visit frequently (for exemple Facebook). 
- after that, change the `http://link1.com/` with the URL of the said site (if we take Facebook, it'll be `https://www.facebook.com/`).
- if you want to add a link, copy paste this code (you'll have to change the `ANOTHER LINK` and the href link of course) after the LINK6 (around line 67) :                                       

``` htm 
<a href="http://anotherlink.com/">
    <li> ANOTHER LINK </li>
</a> 
```

### DATES & MONTS :
- open the `.htm` file in a text editor, search for 'var days' (it'll be at the beginning of the document, around line 19), and change the days (instead of 'dimanche' you can write 'sunday' or 'domingo').
- search for 'var months' (under the var days) and change the months (instead of janvier, you can write january or enero). 

``` javascript
/* DAYS AND MONTHS IN ENGLISH */
var days = ['sunday','monday','tuesday','wenesday','thursday.','friday','saturday'];
var months=['january', 'february', 'march', 'april', 'may', 'june', 'july', 'august', 'september', 'october', 'november', 'december'];
```
- if you want to change the structure of the date, you'll have to edit the following code : the `("0" + m.getDate()).slice(-2)` is the dats, the `(months[m.getMonth() ])` is the month and the `m.getFullYear()` is the year,

``` javascript
var dateString = (days[ m.getDay() ])  + " " +  ("0" + m.getDate()).slice(-2) + " " + (months[ m.getMonth() ])   + " " + m.getFullYear()            
```

### BANNER & BACKGROUND
- first of all, like I said previously, change/add the banner in the banner folder and the background in the background folder and renamed them `background[insert a number].jpg` and `banner[insert a number].jpg` (you'll have to change the '[insert a number]' of course.
- open the js folder, and edit `banner.js` in a text editor : if you one to add others banners/background, you'll have to copy paste this code, you'll have to change the number of course (if you want a fifth banner/background, replace the `4` by `5` : 

``` javascript
/* ADDING A FOURTH BANNER AND BACKGROUND */
4: {
    image: "banner/banner4.jpg",
    landscape:"background/background04.jpg",

}, 
```
- you'll have to change the value in the following code, for example if you have 6 banner/background, you'll have to copy paste this code 
``` javascript
var randomNumber = Math.floor((Math.random() * 6) + 1);
```

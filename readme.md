# Valerie
Valerie is an atmospheric homepage that was inspired by multiple designs that featured full front page wallpapers and underlines used on specific letters. The startpage features an easily customizable greeting, search bar, music player and links. 

![alt text](https://github.com/chloechantelle/valerie/blob/master/preview/valerie.gif "Valerie Preview")

# Instructions
<h3>Firefox</h3>

*Homepage*
    
Ctrl+L > about:preferences > Home Page > Enter the HTML file location.
        
*New tab*
    
Install the <a href="https://addons.mozilla.org/en-US/firefox/addon/new-tab-override" target="_blank">New Tab Override</a> extension > Ctrl+Shift+A > Extensions > New Tab Options > Enter the HTML file location.

<h3>Chrome</h3>

*Homepage*

Settings > Show Home Button > Change New Tab > Enter the HTML file location.

*New tab*

Install the <a target="_blank" href="https://chrome.google.com/webstore/detail/new-tab-redirect/icpgjfneehieebagbmdbhnlpiopdcmna?hl=en">New Tab Redirect</a> extension > Settings > More Tools > Options for New Tab Redirect > Enter the HTML file location.

# Customizing

<h3>Greeting</h3>

The greeting is time based, but can be changed to whatever you like.

Change the greeting variables to your liking:

`var user = ('Your Name');
  var morning = ('morning, ') + user;
  var afternoon = ('good afternoon, ') + user;
  var evening = ('evenin!, ') + user;`

<h3>Search</h3>

You can change the search text that appears by changing the placeholder value:

`<input class="searchbox" name="q" title="Search Google" placeholder="بحث">`

You can also change search engine, for example if you wanted DuckDuckGo instead of Google you adjust the action URL to:

`<form class="search" method="get" action="https://duckduckgo.com/?q=">`

<h3>Cover Image</h3>

To change the cover image move your preferred image to the `img` folder.

Then in the `style.css` file refer to the image:

`#cover { background: url("../img/sky.jpg") }`

<h3>Music</h3>

To change the music that plays move a MP3 file to the `mp3`folder and then change the source for the song:

`<audio id="music" src="mp3/SongName.mp3" preload="auto">`

You can also adjust the song so it autoplays when you load the tab:

`<audio autoplay id="music" src="mp3/Zone.mp3" preload="auto">`	

<h3>Colors</h3>

Colors are set in the `:root` variables at the top of the `style.css` file.

# Issues
<a href="https://github.com/chloechantelle/valerie/issues/new">Submit an issue</a> if you have any problems.

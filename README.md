# Scenes of FFXIV #
Scenes of FFXIV is a site intended to showcase a number of locations from the critically acclaimed MMORPG Final Fantasy XIV (FFXIV).
It will contain a number of in-game screenshots from these locations as well as some descriptive text detailing the history or some key features of the landscape shown.
<br>
This site is intended for any who may be interested in FFXIV, whether it is existing players, those who cannot play, who used to and wish for a feeling of nostalgia, or those who are on the fence and may want a closer look at some of the vistas that are on offer.

## Features ##

## Design ##
### Wireframe ###
Home page
<br><br>
![Desktop Home page](docs/readme_images/Desktop_homepage_wireframe.PNG)
![Mobile Home page](docs/readme_images/mobile_homepage_wireframe.PNG)
<br>
Mobile Home page with Burger Icon selected
<br>
![Mobile Home page burger](docs/readme_images/Mobile_homepage_wireframe_menu.PNG)
<br><br>

Content pages
<br><br>
![Desktop Content page](docs/readme_images/Desktop_content_wireframe.PNG)
![Mobile Content page](docs/readme_images/Mobile_content_wireframe.PNG)
<br>
Two images per block of information. On mobile, text is followed by both images.
<br><br>

Coming Soon page
<br><br>
![Desktop Coming Soon page](docs/readme_images/Desktop_soon_wireframe.PNG)
![Mobile Coming Soon page](docs/readme_images/Mobile_soon_wireframe.PNG)

## Technologies ##
- HTML
  <br> Used as the main language for the site.
- CSS
  <br> Used to style the website via an external stylesheet.
- GitHub
  <br> Used as a repository to store site information and act as a hosting platform.
- Git
  <br> Used to commit and push information to GitHub.
- FontAwesome
  <br> Used to display symbols such as the burger icon, socials, and store pages icons.
- balsamiq
  <br> Used to create wireframe designs for website.
- cloudconvert.com
  <br> Used to convert hero and content images from .png to .webp.

## Testing ##

### Bugs ###
When styling the Store Page icons from Font Awesome (Steam and Meteor), using the 'i' attribute did not allow the colour to change as it did with the Socials icons. I had to use the 'a' attribute. This will not be looked into as it works as is.
<br>
When creating wireframes, copying the mobile homepage facebook image changed it to a different facebook image on paste. Did not change as it does not affect functionality.
<br>
When attempting to add a second font to the site via import from Google Fonts, the formatting broke, causing either the original font I had download and added via @font-face to break and revert to serif, or for the header style to break. This was corrected by instead downloading the font pack, uploading to the repo and applying via @font-face.
<br>
I was unable to utilise the Instagram page for FFXIV without being signed into Instagram. Testing this with my girlfriend's instagram allowed the link to work without issue (https://www.instagram.com/ffxiv?igsh=dmJrcmNoNDM4cmJ0) as such, the Instagram homepage will be used to avoid a 404 error for those that do not have Instagram accounts.
<br>
Upon testing with other people (Discord server full of friends) the Chrome users identified an issue with the images not showing next to each other as intended, and as Firefox did. Upon some testing, a float attribute was needed for the images on Chrome and Edge to stop them from wrapping around each other. Image was rectified and re-tested with those same users and the images were showing as intended.

### Feedback ###
When testing mobile, feedback received was that the nav menu opened on the left where the burger icon was on the right. As such, this was changed for a better UX. Upon re-testing, several user reported this feature was much improved.
<br>

## Credits ##
### Content ###
- Font family downloaded from [FontMeme](https://fontmeme.com/fonts/enge-etienne-font/), created by OPTIFONT.
- Font families Imbue and Bitter downloaded from [Google Fonts](https://fonts.google.com/).
- [W3Schools](https://www.w3schools.com) for information on various HTML and CSS tips.
- [Stack Overflow](https://stackoverflow.com/) for information on various HTML and CSS tips.
- [Final Fantasy XIV Fan Kit site](https://na.finalfantasyxiv.com/lodestone/special/fankit/icon/) for various icons used as favicons and README title accompaniment.
- [Final Fantasy XIV Materials Usage License](https://support.na.square-enix.com/rule.php?id=5382&tag=authc) confirming the feasibility of the project and what concessions are required.
- Information regarding locations was taken either from in-game or from the [Final Fantasy Wiki](https://finalfantasy.fandom.com/wiki/Final_Fantasy_Wiki).

### Media ###
- Content images were taken by myself using my own FFXIV account and the in-game screenshot function. Due to weather conditions and a day night cycle, this proved somewhat taxing.
- The Coming Soon image is the public base game render of a Lalafellan Alchemist. The image itself was taken from the [Final Fantasy Wiki](https://finalfantasy.fandom.com/wiki/Alchemist_(Final_Fantasy_XIV)).
- Hero image taken from the [Final Fantasy XIV Fan Kit](https://na.finalfantasyxiv.com/lodestone/special/fankit/desktop_wallpaper/2_0/#nav_fankit).
- 404 image of my character was taken and edited by Royal Jelly, a friend in Final Fantasy XIV who made this into a Discord sticker. 
  
FINAL FANTASY is a registered trademark of Square Enix Holdings Co., Ltd.
© SQUARE ENIX CO., LTD. All rights reserved. 
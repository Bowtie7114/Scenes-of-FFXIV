# Scenes of FFXIV #
Scenes of FFXIV is a gallery site intended to showcase a number of locations from the critically acclaimed MMORPG Final Fantasy XIV (FFXIV).
It will contain a number of in-game screenshots from these locations as well as some descriptive text detailing the history or some key features of the landscape shown.
<br><br>
This site is intended for any who may be interested in FFXIV, whether it is existing players, those who cannot play, who used to and wish for a feeling of nostalgia, or those who are on the fence and may want a closer look at some of the vistas that are on offer. The live site can be accessed via this link: [Scenes of FFXIV](https://bowtie7114.github.io/Scenes-of-FFXIV/).
<br><br>

![Website Mock-up](docs/readme_images/Mock_up.png)

## Features ##
### Site wide features: ###
The Navigation bar contains the page header as a central element, "Scenes of FFXIV". It also acts as a link to the Homepage. On larger screens the navigation menu is below the title in a row, with an underline denoting which page the user is currently visiting. <br>

![Desktop Nav Bar](docs/readme_images/Nav_desktop.png)
<br>
For mobile devices and small screens the navigation bar is a hidden element until the burger icon is selected. The nav menu then opens below the icon and works as similarly to the larger screen version. The nav menu can then be closed by selecting the icon again.
<br>
![Mobile Nav Bar closed](docs/readme_images/Nav_mobile_closed.png)
![Mobile Nav Bar open](docs/readme_images/Nav_mobile_open.png)
<br>

The footer contains six links; four to social pages, and two to store pages for the game.
They are split into distinct groups, with the socials leading to Facebook, Instagram, Discord, and Reddit. The store pages lead to the Steam Store and the FFXIV homepage respectively.
<br>
![Footer](docs/readme_images/Footer.png)
<br>
As this is a gallery page, and the goal is to allow the User to see the screenshots, the header and footer are glued to the top and bottom of the page respectively.
<br>

### Homepage: ###
The Hero image on the Homepage is responsive and changes size, starting from the middle of the image, on larger screens by design. <br>

![Hero Image Mobile](docs/readme_images/Hero_Mobile.png)
![Hero Image Desktop](docs/readme_images/Hero_PC.png)
<br>

For the main content of the Homepage, there is an introduction on the site, the game it is based on, and instructions on using the site. There are also additional links to the various pages available with the crests of those area's ruling parties/armies. On Mobile, these are in one line, but on larger screens this is spread into two columns to save space and be more visually appealing.
<br>

![Homepage Mobile](docs/readme_images/Main_mobile.png)
![Homepage PC](docs/readme_images/Main_PC.png)

<br><br>

### Content pages: ###
The content pages contain a sub-heading, and introduction to the area, and then the main focus: A description of a region, and two images from said region, repeated three times.
<br>

![Mobile Content 1](docs/readme_images/Content_mobile_1.png)
![Mobile Content 2](docs/readme_images/Content_mobile_2.png)
![Desktop Content](docs/readme_images/Content_PC.png)

<br><br>

### Coming Soon page: ###
There is a Coming Soon page with a small section of text explaining that more content is on the way, and a Lalafell Alchemist performing experiments, for visual flair. Next to this there is a basic form allowing the user to sign up to a newsletter containing updates on the site. This will send the user to the Thank You page upon successful submission.

<br>

![Coming Soon content](docs/readme_images/Coming_soon_desktop.PNG)
![Coming Soon mobile](docs/readme_images/Coming_soon_mobile.PNG)

<br><br>

### Thank You page: ###
Once the form is submitted, the User is taken to the Thank You page, containing some large text thanking the User, and asking them to "look forward to monthly updates" with a smiling Au'Ra greeting them.
<br>

![Thank you content](docs/readme_images/Thank_you.PNG)

### 404 page: ###

The 404 page, which redirects at broken or missing URLs, features a Lalafell performing the "This is fine" meme. The paragraph containing the 'click here' passage was removed for accessibility reasons but urges the user to either check that their URL is correct, or find the creator on GitHub in order to let them know that something is broken.

<br>

![404 Content](docs/readme_images/404.png)

<br>

### Favicon ###
The favicon is set to the icon for the Sightseeing Log in game, which I thought was appropriate, and the title changes depending on the page the user is on, preceeded by "FFXIV Scenes - ".

![Favicon and Title](docs/readme_images/Favtitle.png)

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
- tinypng.com
  <br> Used to compress image files before upload to increase web loading performance.

## Testing ##

### Accessibility ###
The [Wave Accessibility] tool was used for testing at the end of development. The testing found one critical error in that there was no label for the "burger icon" to open the navigation menu on Mobile. This label was added to all pages and the error resolved.

The following were all Alerts that were received by the tool, but will not be changed as they are intentional in some manner:
- Possible headings for main page secondary links. They are p elements whereas the system think they would be better as h elements.
- Possible headings for footer Socials and Store pages paragraphs.
- Redundant link. Home Nav element directly next to Title, both containing the index.html redirect.
- Underlined text on nav menu items. Kept for visual representation of what page the user is on.
- Long alternative text for images: as this is a gallery site, I feel the images being more descriptive here is a boon, rather than a bane.

The following Alert was changed:
- Suspicious link text on Coming Soon and 404 pages. Link to homepage removed and text changed/removed.

The following criteria was met following testing with the Wave Accessibility tool:
- Colour contrasts passed both the WCAG AA and AAA, with a contrast ratio of 8.59:1.
- The order of the page flows correctly from header to text without skipping sections.
- All non-text based content contains alt text descriptions for screen readers.
- HTML page lang attribute has been set correctly.
- Aria properties implemented correctly.

After manual testing, the site was navigable using only keyboard and only mouse, respectively, on Mozilla Firefox, Google Chrome, Microsoft Edge, and Safari.

### Lighthouse Testing ###
Initial Lighthouse testing was performed using Google Chrome, and showed low performance (between 65 and 89) due to image sizes. Accessibility was also at 94 across the board. Lighthouse testing was done again upon in the UK and accessiblity was 100 without additional changes. It could be related to language differences in the browser/systems used at the time. <br><br>
Content images were made smaller in terms of resolution (1600px by 900px), converted to webp, and then run through tinypng.com to improve performance. Significant increases were observed. <br><br>
Previous values:<br>
![Lighthouse Homepage](docs/readme_images/Lighthouse_Homepage.png)
![Lighthouse Thanalan page](docs/readme_images/Lighthouse_Thanalan.png)
![Lighthouse La Noscea page](docs/readme_images/Lighthouse_Noscea.png)
![Lighthouse Black Shroud page](docs/readme_images/Lighthouse_Shroud.png)
![Lighthouse Coming Soon page](docs/readme_images/Lighthouse_Soon.png)
<br><br>
New values:<br>
![Lighthouse Homepage](docs/readme_images/Lighthouse_Homepage2.PNG)
![Lighthouse Thanalan page](docs/readme_images/Lighthouse_Thanalan2.PNG)
![Lighthouse La Noscea page](docs/readme_images/Lighthouse_Noscea2.PNG)
![Lighthouse Black Shroud page](docs/readme_images/Lighthouse_Shroud2.PNG)
![Lighthouse Coming Soon page](docs/readme_images/Lighthouse_Soon.PNG)
![Lighthouse Thank You page](docs/readme_images/Lighthouse_Thanks.PNG)
![Lighthouse 404 page](docs/readme_images/Lighthouse_404.PNG)
<br><br>
### Functional Testing ###
#### Navigational Links ####
All page links were tested thoroughly throughout development, and again by multiple test users by selecting each link on each page individually. All links routed to the correct pages as expected throughout.

| Navigation Link  | Page to Load     |
| ---------------- | ---------------- |
| Scenes of FFXIV  | index.html       |
| Home             | index.html       |
| Thanalan         | thanalan.html    |
| La Noscea        | la-noscea.html   |
| The Black Shroud | shroud.html      |
| Coming Soon!     | coming-soon.html |

The various footer icons obtained from FontAwesome were all tested on each webpage to ensure that they functioned correctly. The expected behaviour is that they are to open a new tab and open to the following pages in order from left to right:
- [Facebook](https://www.facebook.com/) Login page/Homepage if logged in
- [Instagram](https://www.instagram.com/) Login page/Homepage if logged in
- Reddit FFXIV Subreddit: [r/FFXIV](https://www.reddit.com/r/ffxiv/)
- [Discord](https://www.discord.com/) Homepage
- [Steam FFXIV Store Page](https://store.steampowered.com/app/39210/FINAL_FANTASY_XIV_Online/)
- [Final Fantasy XIV Homepage](https://www.finalfantasyxiv.com/)

Upon testing each icon on each page individually, these are all working as expected.

#### Form Testing ####

The form on the Coming soon page is very basic due to intended features only being available through JavaScript, namely attaching a pop-up to the required fields in the form of red asterisks and an optional telephone number field that would become required should a radio button for both Email and Text news selected. As such, Name and Email are both requried fields.

It was tested to ensure it functioned as expected when correct data was input and when incorrect data was input. The following test scenarios were covered:

_Scenario One - Correct Inputs_

Steps:

1. Navigate to [Coming Soon page](https://bowtie7114.github.io/Scenes-of-FFXIV/coming-soon.html)
2. Scroll down to the form and input the following data:
   - Name: Jordan
   - Email Address: jordan.cook@fake.com
3. Click Submit

Expected:

The form submits without any errors and successfully redirects to thanks.html.

Actual:

Website behaved as expected.

_Scenario Two - Missing Required Field Name_

Steps:

1. Navigate to [Coming Soon page](https://bowtie7114.github.io/Scenes-of-FFXIV/coming-soon.html)
2. Scroll down to the form and input the following data:
   - Name:
   - Email Address: jordan.cook@fake.com
3. Click Submit

Expected Result:

An Error is displayed informing the user that the Name field is required, and it does not submit.

Result:

Error message was displayed to fill out the Name field and the form did not submit.

_Scenario Three - Missing Required Field Email_

Steps:

1. Navigate to [Coming Soon page](https://bowtie7114.github.io/Scenes-of-FFXIV/coming-soon.html)
2. Scroll down to the form and input the following data:
   - Name: Jordan
   - Email Address:
3. Click Submit

Expected:

An Error is displayed informing the user that the Email field is required, and it does not submit.

Actual:

Error message was displayed to fill out the Email field and the form did not submit.

_Scenario Four - Incorrect email format_

Steps to test:

1. Navigate to [Coming Soon page](https://bowtie7114.github.io/Scenes-of-FFXIV/coming-soon.html)
2. Scroll down to the form and input the following data:
   - Name: Jordan
   - Email Address: jordan.
3. Click Submit

Expected:

An Error is displayed informing the user that they need to enter a valid email address, and the form fails to submit.

Actual:

Error message was displayed to enter a valid email address and the form did not submit.

### Validator Testing ###
Initial validation with the [W3C Validator](https://validator.w3.org/#validate_by_uri) found a number of errors and warnings to resolve in the HTML relating to stray end tags for the i attributes from font-awesome. Upon correct these, no further errors were noted:

![Validator Homepage](docs/readme_images/Validator_home.png)
![Validator Thanalan](docs/readme_images/Validator_thanalan.png)
![Validator La Noscea](docs/readme_images/Validator_noscea.png)
![Validator Shroud](docs/readme_images/Validator_shroud.png)
![Validator Coming Soon](docs/readme_images/Validator_soon.png)
![Validator Thank You](docs/readme_images/Validator_thanks.PNG)
![Validator 404](docs/readme_images/Validator_404.png)

Initial validation with the [Jigsaw Validator](https://jigsaw.w3.org/css-validator/) flagged a number of mistakes seen below. These were corrected and validator passed on second run.
<br>

![CSS Validator fail](docs/readme_images/CSS_validator_errors.png)
![CSS Validator pass](docs/readme_images/CSS_validator_fixed.png)

### Bugs ###
- When styling the Store Page icons from Font Awesome (Steam and Meteor), using the 'i' attribute did not allow the colour to change as it did with the Socials icons. I had to use the 'a' attribute. This will not be looked into as it works as is.
<br><br>
- When creating wireframes, copying the mobile homepage facebook image changed it to a different facebook image on paste. Did not change as it does not affect functionality.
<br><br>
- When attempting to add a second font to the site via import from Google Fonts, the formatting broke, causing either the original font I had download and added via @font-face to break and revert to serif, or for the header style to break. This was corrected by instead downloading the font pack, uploading to the repo and applying via @font-face.
<br><br>
- I was unable to utilise the official Instagram page for FFXIV without being signed into Instagram. Testing this with my girlfriend's Instagram account allowed the link to work without issue (https://www.instagram.com/ffxiv?igsh=dmJrcmNoNDM4cmJ0) as such, the Instagram homepage will be used to avoid a 404 error for those that do not have Instagram accounts.
<br><br>
- Upon testing with other people (Discord server full of friends) the Chrome users identified an issue with the images not showing next to each other as intended, and as Firefox did. Upon some testing, a float declaration was needed for the images on Chrome and Edge to stop them from wrapping around each other. Image was rectified and re-tested with those same users and the images were showing as intended.

### Feedback ###
When testing mobile, feedback received was that the nav menu opened on the left where the burger icon was on the right. As such, this was changed for a better UX. Upon re-testing, several user reported this feature was much improved.
<br><br>

## Deployment ##
### Version Control ###

This website was made using Replit as the IDE which was linked to GitHub, allowing it to be saved as a remote repository named "Scenes-of-FFXIV" using git commands.

Said commands used to push to the repository are:

```git add <file>``` which adds the file (or all changes if you use . ) to the staging area to be committed.

```git commit -m "commit message"``` then commits the changes that were added previously, along with a message indicating what was changed. These commits are then queued together before being pushed.

```git push``` will then update the repository with all of the previously committed code, including their messages and timestamps, to the GitHub repository linked to the IDE.

### Deployment to GitHub Pages ###
The site was deployed using Github Pages. The live link to the site is: https://bowtie7114.github.io/Scenes-of-FFXIV/
<br>
A site can be deployed to GitHub Pages by:
- Selecting the 'Settings' in your GitHub repository.
- Selecting the 'Pages' tab from the left-hand menu.
- From the 'source' drop-down selecting 'Branch: Main'.
- Click Save.
- After a few moments, refresh the page and link to the live site will be available at the top of the page.

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
- 404 image of my character and thank you image of another FC member were taken and edited by Royal Jelly, a friend in Final Fantasy XIV who made these into Discord stickers. Permission was provided before use. 
  
FINAL FANTASY is a registered trademark of Square Enix Holdings Co., Ltd.
© SQUARE ENIX CO., LTD. All rights reserved. 
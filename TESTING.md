# **TESTING DOCUMENT**

## **Wet Paws** | Dog Walking and Sitting Services

[View live project here](https://maialenz.github.io/WetPaws/)

## OVERVIEW

This being my first ever project in Web Development, at the beginning, I encountered quite a few obstacles that made me start the project from the start again (as seen in the commit history).

As my project started taking form and I could visualize it on a browser as I went along, I felt more and more confident on what I was doing, even trying new things like adding music tracks and trying different hover styles.

Towards the end I had to redo a few things that did not quite work as I planned, like loading libraries, JS, jQuery...

From the very beginning I used Google Chrome Dev Tools to style and fix my code, so thanks to that I found it much easier to see real time changes and copy that css/code to my workspace.

Once finished, I tested my site on a few different phones, laptop, tablet and desktop as well as DevTools and different browsers manually.

## Table of Content

1. [USER STORIES](#user-stories-testing)
2. [FAVICON TEST](#favicon-test)
3. [VALIDATOR CHECKS](#validator)
   - [HTML](#html-validator)
     - Index.html
     - Services.html
     - Contact.html
   - [CSS](#css-validator)
4. [LIGHTHOUSE TESTING](#lighthouse-testing)
   - Mobile
   - Web
5. [DEVICE RESPONSIVENESS](#device-responsiveness)
6. [BROWSER COMPATIBILITY](#browser-compatibility)
7. [BUGS](#bugs)
8. [KNOWN BUGS](#known-bugs)
9. [BACK TO README.md](README.md)

## USER STORIES TESTING

- As a visiting user I want to:

  - _"Find out what the company is about."_

    - When the user lands on any of the pages, the first thing they see it's the logo representing a paw and the name of the company (Wet Paws), followed by a summed up version of the company's nature to be (Dog walking and sitting). Just by seeing the logo once, the user will get a clear idea of the intention of the business.
    - The hero image hints that the business is related to dogs. All hero images represent dogs, but they are all different so the user knows there has been some change when they have clicked on one of the navigation links. All dog pictures have been chosen to have some relation to the outdoors or the sea.

      ![screenshot of logo and company name](docs/testing/user-stories/test-userstory1.png)

    - For users who want to learn more about the business and the owner, there is an informative section called About Us where the owner explains what the company is about. The section also has a picture of the owner's dog as an introduction to the company's owner and to create a feeling of trust and showing the users that the owner has knowledge of dog care.
    This section also tells the user Who the owner is, Where the company is located, Why to hire them and the name of their own dog to make it more personal.

      ![screenshot of about us section explaining the company's reason to be](docs/testing/user-stories/test-userstory1.2.png)

    - For the comfort of the user, the navbar has a section called About Us that can be reached from any of the other pages. The link is highlighted on a darker color to suggest that the user is seeing the page with the company's information

      ![screenshot of the navbar highlighting the About us section](docs/testing/user-stories/test-user-story1-about-us-navbar.png)

  - _"Easily visualize and understand what services the company offers."_

    - On the navbar, there is a tab called Services so the user can jump directly to that page and see the services the company offers.

      ![screenshot of the navbar pointing the services section](docs/testing/user-stories/test-userstory2.services-navbar.png)

    - When the user scrolls down from the hero image, there is a header that lets the user know that they are seeing the services section, and this contains 4 cards each with a highlighted heading with the title of the service and a short but concise explanation about each service.

      ![screenshot of the header for services section](docs/testing/user-stories/test-userstory2-service-header.png)
      ![screenshot of the service cards and their explanation](docs/testing/user-stories/test-userstory2-services.png)

  - _"Be able to use and book one or more services the company has to offer."_

    - Under each service card there is an area saying "Ask more about this service" which the user can click to be redirected to the contact form and be able to ask more questions to the owner.

      ![screenshot of the ask about this service button under each service](docs/testing/user-stories/test-userstory3-ask-about-button.png)

    - The "Ask more about this service" button will redirect the user to the contact form where the user can select an option to be booked or enquired about. This section is not required so the user can write their own requirements on personal needs on the "Tell us more" textarea, located just below the radio button service choices:

      ![screenshot of the form showing radiobuttons to choose service the user to know more about](docs/testing/user-stories/test-userstory3-know-more-about.png)

  - _"Be able to use the contact form for the business and service enquiries."_

    - To be able to quickly access the contact form from any part of the website, the words "form/contact form/Ask about this form (button)" have been linked to the form section. The first two words have been underlined and the font weight increased to hint the user that the word is clickable. "Ask about this service" button glows and changes the background color when hovered over, to entice the user to click on it.

      ![screenshot of the form links](docs/testing/user-stories/test-userstory4-form-link.png)
      ![screenshot of the form links](docs/testing/user-stories/test-userstory4-contact-form-link.png)
      ![screenshot of the ask about this service button hovered](docs/testing/user-stories/test-userstory4-link-hovered.png)

    - The navbar has a direct link to the contact form called "Contact Us!" to make the user feel confortable to contact the company with any question/needs the user might have:

      ![screenshot of the navbar highlighting Contact Us section](docs/testing/user-stories/test-userstory4-contact.us-navbar.png)

    - The contact form is minimal with no pictures to make sure the user doesn't get overwhelmed with information and fields to be filled. For users who need help with the information required on each field, there is a placeholder text to hint the user with the response needed on each box.
    - [EDIT]: at the end of the testing I added an asterisk to the required fields to hint the users that those forms are mandatory to be able to send the form.

      ![screenshot of the contact form first part](docs/testing/user-stories/test-userstory4-contactform1.png)
      ![screenshot of the contact form second part](docs/testing/user-stories/test-userstory4-contactform2.png)
      ![screenshot of mandatory fields pointed with an asterisk](docs/testing/user-stories/asterisk.png)

  - _"Have the option to personalize the services offered."_

    - Within the services section, the user can find a card called "Personalised", refering to a personalization of the services offered or the posibility of asking for a service not listed on the other cards. The user is informed to make an inquire in the contact form inside the "Tell us more" section, asking for the posibility and conditions of their personal request.

      ![screenshot of the personalised service card](docs/testing/user-stories/test-userstory5-personalised-service.png)

  - _"Feel that the company cares and I can trust them caring for my loved dog by seeing other people's reviews."_

    - The user can find reviews by customers on a section located below the services. They can find a review for each one of the services offered, and for more realism each one of the reviews has a picture of a real dog at the top, representing the actual dog that the company looked after personally.

      ![screenshot of the reviews under services](docs/testing/user-stories/test-userstory6-reviews.png)

    - The user can also find a small gallery with pictures taken of dogs under the owner's care while they are with her. The users can see what other dogs look like and they can also see their own dog's picture, giving the user feeling of company transparency and relieve seeing their dogs well when they are not around.

      ![screenshot of the small gallery with dog pictures](docs/testing/user-stories/test-userstory6-gallery.png)

  - _"Be able to know more about the owner by having the option to personally meet them."_

    - For those users who want to meet the owner personally before deciding if they want to book any of the services, there is a section called "Meet Us" where the user can find information about meeting times, location and if they prefer, a link to the contact form to book a private walk with the owner and see the compatibility between the owner's dog and the user's dog.

      ![screenshot of meet us section](docs/testing/user-stories/test-userstory7-meetus.png)

  - _"Know the location of the business and know where those services are offered."_

    - Just above the footer there is a location map where the user can see the specific loaction of the company on the map.

      ![screenshot of the map for location](docs/testing/user-stories/test-userstory8-map.png)

    - On the footer the user can find information about the location, county and country of the business, as well as the name of the owner and their dog's.

      ![screenshot of the footer information about company location](docs/testing/user-stories/test-userstory8-name-town.png)

  - _"Get in touch with the business easily by having contact details clearly available."_

    - In the navbar the user can find a direct link that will bring them to the contact form.

      ![screenshot of the navbar with contact us link](docs/testing/user-stories/test-userstory4-contact.us-navbar.png)

    - The navbar is sticky so the user can access any of the pages links at any moment without the need of scrolling up. The sticky navbar is responsive on small screens too, as the user needs to scroll more on a mobile device to go to the top.

      ![screenshot of the navbar with contact us link](docs/testing/user-stories/test-userstory9-sticky-navbar.png)
      ![screenshot of the navbar with contact us link](docs/testing/user-stories/test-userstory9-sticky-navbar-mobile.png)

    - The user has also the posibility of contacting the company by phone or email using the information found at the footer.

      ![screenshot of the contact information at footer](docs/testing/user-stories/test-userstory9-reachus.png)

    - For those users that submit the form but they require faster contact, on the feedback form they can find a note encouraging the user to call the owner anytime at the phone provided.

      ![screenshot of the feedback page with contact number](docs/testing/user-stories/test-userstory9-feedback-number.png)

  - _"Find social links to be able to follow the business in social media platforms."_

    - For those users who want to follow the company on different social media platforms, there are links on the footer under the header called "follow our adventures". These links open on separate tabs for better user experience.

      ![screenshot of the social media links](docs/testing/user-stories/test-userstory10-socials.png)

    - For users that have a premium spotify account, there is a section where there is three playlists, so the users can enjoy playlists chosen by the owner while they are walking their own dogs.

      ![screenshot of the spotify playlists](docs/testing/user-stories/test-userstory10-playlist.png)

---
## FAVICON TEST

When I introduced the first and second favicon, I noticed I could not see the shape on the brower tab as they were very
blurry and unidentifyable. Therefore, I created a new favicon with a bold black color and simpler shape, so it can be easily identified
in between the rest of the opened tabs. This change has improved the user experience as I can identify the site's tab in one
fast single look.

- [Favicon 1](docs/testing/favicon_test/test-favicon1.png)
- [Favicon 2](docs/testing/favicon_test/test-favicon2.png)
- [Chosen Favicon](docs/testing/favicon_test/test-favicon3.png)

As seen in the examples above, the new favicon is visually more appealing than the first two.

---

## VALIDATOR:

During the whole project, I continuously checked my code using [W3 Validator](https://validator.w3.org/#validate_by_uri) to make sure I fixed my code as I wrote it. At the end, I ran all the finished pages and made sure all the errors were fixed (see identified and fixed error list below).

As a css validator, I also used [w3 Validator](https://jigsaw.w3.org/css-validator/) to make sure it checked my style.css file to CSS level 3 + SVG standards.

(See passed validator results at the end of HTML and [CSS](#css-validator) sections.

### HTML VALIDATOR:

List of errors found by the validator to be fixed (after the first run):

- The type attribute is unnecessary for JavaScript resources.

  - I removed the type attribute fromm them.

- Some of the images are not loading and the path seems to be broken

  - I checked with dev-tools on google chrome.
  - I fixed this fixing the source path where I made a mistake (my assets directory is called static, but I wrote assets/images)
  - It's fixed. All pictures are showing as they are meant to and they are responsive.

- missuse of Aria attribute (Aria-label) on line 65 (span aria-label="image of an ...").
  - To make it accessible and have an image description I added a role="img" to be able make a relevant description of the purpose of the parent element.

INDEX.html

- line 152: text-center not allowed on div

  - fixed error adding class="text-center"

- line 155: Attribute target not allowed on element iframe at this point.

  - removed all target attributes from iframe elements.

- line 155: Attribute autoplay not allowed on element iframe at this point.

  - removed autoplay from iframe elements

- line 158: The frameborder and allowtransparency attribute on the iframe element are obsolete.

  - to comply with the w3 validator, I added inline styles to the iframes (style="border:none;") and removed allowtransparency="true as I didn't need it.

- line 172: Bad value 100% for attribute width on element iframe: Expected a digit but saw % instead.

  - I removed width="100%" and added class="w-100" to the map's iframe

- line 170: section is missing a header
  - added h2 to map section for better accessibility and organization of information.

SERVICES.html

- line 148: No p element in scope but a p end tag seen.

  - error: a ul element was inside the p element. To fix this i closed the p element in line 138 and put the ul as a child of div (card-body)

- line 170: Attribute heigh not allowed on element img at this point.

  - Fixed by removing height and width from the img element and added them using css under .img-responsive (style.css line 350, 351)

- line 170: An img element must have an alt attribute

  - added alt attribute to all img elements within the article element on lines 170, 191, 214, 235.

- line 162: Article lacks heading. Consider using h2-h6 elements to add identifying headings to all articles.

  - moved h2 from line 164 to line 163 over the div-reviews element.

CONTACT.html

- line 169: Element h5 not allowed as child of element label in this context.
  - removed h5 element from label. I added the id="tell-more" to the label and styled the same way as h5 (style.css line 397)

---

HTML VALIDATOR RESULTS

- [Index.html Validator result](docs/testing/validator/index.html-w3-pass.png)

- [Services.html Validator result](docs/testing/validator/services.html-w3-pass.png)

- [Contact.html Validator result](docs/testing/validator/contact.html-w3-pass.png)

- [Feedback.html Validator result](docs/testing/validator/feedback.html-w3-pass.png)

---

### CSS VALIDATOR

Results for CSS validator check

- [CSS Validator result](docs/testing/validator/CSS-validator-pass.png)

---

## LIGHTHOUSE TESTING

Using DevTool's Lighthouse tool, I checked all pages on mobile and desktop to make sure the scores were as high as I posibly could. Below you can find the results and scores of first time tests and after implementing suggestions that the tool offered:

(All tests were carried out the same way: I cleared cache data, opened new incognito page (Chrome and Edge), and reloaded and tested each page twice. Same procedure was used for mobile and web assessment)

- **Mobile**

  - Index.html Lighthouse test:

    - [Before](docs/testing/lighthouse/index-phone-before) implementing changes:
      - The performance score was very low and in red. This was due to very big images and unused javascript libraries. To fix that I compressed all images with Tinypng and cropped them to make equal squares. I also changed the gallery images as it was impossible to make them any lower on weight without pixelating them and they ended up not looking too good. I also changed the grid system so all pictures show on top of each other in mobile view.
    - [After](docs/testing/lighthouse/index-phone-after) following lighthouse suggestions:
      - I managed to increase the very low performance score to 82%. Although this is not ideal, I found it very difficult to implement any more changes as this meant to add attributes to elements that made the validator fail. So I decided to leave the index at this level until I have more time and skills for further changes and improvements.

  - Services page Lighthouse test:

    - [Before](docs/testing/lighthouse/services.html-phone-before.png) implementing changes
      - as in the index page, the performance score was quite low because of the weight of the images
    - [After](docs/testing/lighthouse/services-phone-after.png) following lighthouse suggestions:
      - once I implemented the suggestions given by the lighthouse tool, the score increased to 86%. I decreased the size of the images and added meta data to the head for better SEO (%100)

  - Contact page Lighthouse test:

    - [Before](docs/testing/lighthouse/contact.html-before-phone.png) implementing changes
    - [After](docs/testing/lighthouse/contact.html-phone-after.png) following lighthouse suggestions:
      - although the performance before was quite low, implementing lighthouse suggested changes increased the performance of the mobile test quite significantly, but we can see the biggest improvement in Best practices, where the score went up to 93%.

  - Feedback page Lighthouse test:
    - Before: This feature was added at the very end of the project, when I noticed some issues as I was testing all the pages (see bugs for more info on error 501). Because of this, I forgot to take any screenshots of the lighthouse testing before.
    - [After](docs/testing/lighthouse/lighthouse-feedback-after.png)

- **Web**

Because I focused on mobile first approach for the testing part, all the improvements made to increase the performance on the mobile view, has greatly benefited the web performance too. This changes included compression of images, removal of unused code and css, reload of better sources for bootstrap/fontawesome libraries...

- Index web page Lighthouse test:

  - [Before](docs/testing/lighthouse/index.html-before-web.png) implementing changes
  - [After](docs/testing/lighthouse/index.html-after-web.png) following lighthouse suggestions:
    - in the results we can see that the best practices did not increase too much. This was due to the ratio of the image I chose to display on the grid of "About us" section within Index.html. Whilst lighthouse was advicing to change this ratio to it's original size, I decided not to change it, as I found this to be much bigger than I intended it to be, and this would consequently affect the performance on the mobile view.

- Services web page Lighthouse test:

  - [Before](docs/testing/lighthouse/services.html-before-web.png) implementing changes
  - [After](docs/testing/lighthouse/services.html-after-web.png) following lighthouse suggestions:
    - We can clearly see in these results that eventhough the performance of the services page was already high enough, making changes after the mobile lighthouse test increased all the parameters even higher.

- Contact web page Lighthouse test:

  - [Before](docs/testing/lighthouse/contact.html-before-web.png) implementing changes
  - [After](docs/testing/lighthouse/contact.html-after-web.png) following lighthouse suggestions:
    - This has been the best results out of all the pages. This is due to the simplicity of the page, minimal structure and no heavy imagery to be loaded. Still, we can see an improvement after the changes lighthouse suggested.

- Feedback web page Lighthouse test:
  - Before: This feature was added at the very end of the project, when I noticed some issues as I was testing all the pages (see bugs for more info on error 501). Because of this, I forgot to take any screenshots of the lighthouse testing before.
  - [After](docs/testing/lighthouse/feedback-after-lighthouse.png)

---

## DEVICE RESPONSIVENESS

I continuously tested the project on various devices from the very beginning. I mostly used Google Chrome DevTools, but as soon as I deployed the website (using GitHub Pages) I pushed my code very often to see the results of the changes in real time on my own personal devices (Samsung S8+, Samsung A70, HP Envy 13", Samsung 5Se Tablet) and make sure the site was responsive on various viewports.

Apart from that, I used an online app by [Media Genesis](https://responsivedesignchecker.com/) as well as Google Chrome Developer tools to check responsiveness on those screens I did not have access to. The results of these testings are below (the results of the tests were written on a xcel and converted to png, so the excel was broken in 4 parts):

- [Part1](docs/testing/device+browser-tests/device-responsiveness-1.png)
- [Part2](docs/testing/device+browser-tests/device-responsiveness-2.png)
- [Part3](docs/testing/device+browser-tests/device-responsiveness-3.png)
- [Part4](docs/testing/device+browser-tests/device-responsiveness-4.png)

Most phones share screen sizes so on those I did not see many changes. Saying that, on narrow screens (for example in the Galaxy Fold with a viewport of 286x653) some on the headings (especially on headings in services.html) broke on the middle. To fix these, I added some extra css to media queries for screens with max width 450, reducing margings to fit to screen better. (find these in style.css lines 487 - 509)

---

## BROWSER COMPATIBILITY

I thoroughly checked on different devices and different browsers. Wherever posible I downloaded the browsers into my devices and I tested my site on them manually, making sure all links were checked and tested. In some cases I had to ask friends and family to check the live site on their own devices (due to not being personally able to install the different operating system like iPhone and Macbook's safari into my own devices).
As a main conclusion of these tests, I have to add that I did not find any differences from one browser to another. There was full compatibility of all features and links cross browser/device. Following Bootstrap documentation's advice, I checked if the navigation bar was sticky on all the devices/browsers, as they recognize that the sticky navbar is not responsive/compatible on some browsers like for example, Opera. But after running my manual tests, my navbar did respond and was responsive as I intended to be on my design even in the Opera browser.

All the screenshots to my manual tests on various major devices are below:

- Samsung Galaxy S8+ (My personal device) (mobile device): As mentioned before, I continuously tested my code on my own mobile device as I went writting and styling the code, so I could see how it looked on smaller screens. Thanks to testing on my phone I noticed some headings had to be made smaller so they did not look oversized. Below there is screenshots of a last test done on this device:

  - [Samsung S8+ screenshot index](docs/testing/device+browser-tests/Samsungs8+screenshot-index.jpg)
  - [Samsung S8+ screenshot services](docs/testing/device+browser-tests/samsungs8+screenshot-services.jpg)
  - [Samsung S8+ screenshot contact](docs/testing/device+browser-tests/samsungs8+screenshot-contact.jpg)
  - [Samsung S8+ screenshot feedback](docs/testing/device+browser-tests/Samsungs8+screenshot-feedback.jpg)
  - [Samsung S8+ screenshot of footer](docs/testing/device+browser-tests/Samsungs8+screenshot-footer.jpg)

- Samsung A70 (mobile device): I also tested the website on another mobile device:

  - [Samsung A70 Screenshot index](docs/testing/device+browser-tests/samsungA70-index.jpg)
  - [Samsung A70 Screenshot map/footer](<(docs/testing/device+browser-tests/samsungA70-map.jpg)>)
  - [Samsung A70 Screenshot services](docs/testing/device+browser-tests/samsungA70-services.jpg)
  - [Samsung A70 Screenshot reviews](docs/testing/device+browser-tests/samsungA70-reviews.jpg)
  - [Samsung A70 Screenshot contact](docs/testing/device+browser-tests/samsungA70-contact.jpg)
  - [Samsung A70 Screenshot form](docs/testing/device+browser-tests/samsungA70-form.jpg)

- Samsung S5e (tablet): As I tested the site on my Tablet, I noticed the headers on the service's cards that the margin was too great and the personalized header was breaking into another line. I added a media querie to fix this and below are screenshots showing the results:

  - [Galaxy Tab S5e Index](docs/testing/device+browser-tests/Galaxy-Tab-S5e-index.jpg)
  - [Galaxy Tab S5e Services](docs/testing/device+browser-tests/Galaxy-Tab-S5e-services.jpg)
  - [Galaxy Tab S5e Service Cards](docs/testing/device+browser-tests/Galaxy-Tab-S5e-servicestabs.jpg)
  - [Galaxy Tab S5e Contact](docs/testing/device+browser-tests/Galaxy-Tab-S5e-contact.jpg)
  - [Galaxy Tab S5e Feedback](docs/testing/device+browser-tests/Galaxy-Tab-S5e-feedback.jpg)

- HP Envy 13" (laptop)

  - Google Chrome (browser):

    - [HP Envy index screenshot](docs/testing/device+browser-tests/HP-envy-index.png)
    - [HP Envy services screenshot](docs/testing/device+browser-tests/HP-envy-services.png)
    - [HP Envy reviews screenshot](docs/testing/device+browser-tests/HP-envy-reviews.png)
    - [HP Envy contact screenshot](docs/testing/device+browser-tests/HP-envy-contact.png)
    - [HP Envy feedback screenshot](docs/testing/device+browser-tests/HP-envy-feedback.png)
    - [HP Envy footer screenshot](docs/testing/device+browser-tests/HP-envy-footer.png)

  - Mozilla Firefox (browser)

    - [HP Envy Mozilla index screenshot](docs/testing/device+browser-tests/hp-mozilla-index.png)
    - [HP Envy Mozilla services screenshot](docs/testing/device+browser-tests/hp-mozilla-services.png)
    - [HP Envy Mozilla reviews screenshot](docs/testing/device+browser-tests/hp-mozilla-reviews.png)
    - [HP Envy Mozilla contact screenshot](docs/testing/device+browser-tests/hp-mozilla-contact.png)
    - [HP Envy Mozilla feedback screenshot](docs/testing/device+browser-tests/hp-mozilla-feedback.png)
    - [HP Envy Mozilla footer screenshot](docs/testing/device+browser-tests/hp-mozilla-footer.png)

  - Microsoft Edge (brower)

    - [HP Envy Edge index screenshot](docs/testing/device+browser-tests/edge-HP-index.png)
    - [HP Envy Edge services screenshot](docs/testing/device+browser-tests/edge-HP-services.png)
    - [HP Envy Edge reviews screenshot](docs/testing/device+browser-tests/edge-HP-reviews.png)
    - [HP Envy Edge contact screenshot](docs/testing/device+browser-tests/edge-HP-contact.png)
    - [HP Envy Edge feedback screenshot](docs/testing/device+browser-tests/edge-HP-feedback.png)
    - [HP Envy Edge footer screenshot](docs/testing/device+browser-tests/edge-HP-footer.png)

  - Opera (browser)
    - [HP Envy Opera index screenshot](docs/testing/device+browser-tests/Opera-HP-index.png)
    - [HP Envy Opera services screenshot](docs/testing/device+browser-tests/Opera-HP-services.png)
    - [HP Envy Opera reviews screenshot](docs/testing/device+browser-tests/Opera-HP-reviews.png)
    - [HP Envy Opera contact screenshot](docs/testing/device+browser-tests/Opera-HP-contact.png)
    - [HP Envy Opera feedback screenshot](docs/testing/device+browser-tests/Opera-HP-feedback.png)
    - [HP Envy Opera footer screenshot](docs/testing/device+browser-tests/Opera-HP-footer.png)

- PC HP desktop 31.5" screen

  - Google Chrome (browser)

    - [HP Desktop index screenshot](docs/testing/device+browser-tests/hp-desktop-chrome-index.png)
    - [HP Desktop services screenshot](docs/testing/device+browser-tests/hp-desktop-chrome-services.png)
    - [HP Desktop reviews screenshot](docs/testing/device+browser-tests/hp-desktop-chrome-reviews.png)
    - [HP Desktop contact screenshot](docs/testing/device+browser-tests/hp-desktop-chrome-contact.png)
    - [HP Desktop feedback screenshot](docs/testing/device+browser-tests/hp-desktop-chrome-feedback.png)
    - [HP Desktop footer screenshot](docs/testing/device+browser-tests/hp-desktop-chrome-footer.png)

  - Microsoft Edge (browser)
    - [HP Desktop index screenshot](docs/testing/device+browser-tests/hp-desktop-edge-index.png)
    - [HP Desktop services screenshot](docs/testing/device+browser-tests/hp-desktop-edge-services.png)
    - [HP Desktop reviews screenshot](docs/testing/device+browser-tests/hp-desktop-edge-reviews.png)
    - [HP Desktop contact screenshot](docs/testing/device+browser-tests/hp-desktop-edge-contact.png)
    - [HP Desktop feedback screenshot](docs/testing/device+browser-tests/hp-desktop-edge-feedback.png)
    - [HP Desktop footer screenshot](docs/testing/device+browser-tests/hp-desktop-edge-footer.png)

- iOs and MacOs operating system tested on Safari browser: no differences were found even on apple operating systems.

  - iPhone 12

    - [iPhone index screenshot](docs/testing/device+browser-tests/iphone-index.jpeg)
    - [iPhone collapsible navbar screenshot](docs/testing/device+browser-tests/iphone-collapsible-navbar.jpeg)
    - [iPhone services screenshot](docs/testing/device+browser-tests/iphone-services-head.jpeg)
    - [iPhone services header screenshot](docs/testing/device+browser-tests/iphone-services.jpeg)
    - [iPhone reviews screenshot](docs/testing/device+browser-tests/iphone-reviews.jpeg)
    - [iPhone contact form header screenshot](docs/testing/device+browser-tests/iphone-contact-head.jpeg)
    - [iPhone contact form top screenshot](docs/testing/device+browser-tests/iphone-contactform.jpeg)
    - [iPhone contact form submit screenshot](docs/testing/device+browser-tests/iphone-contactform-submit.jpeg)
    - [iPhone footer screenshot](docs/testing/device+browser-tests/iphone-footer.jpeg)

  - MacBook 13"
    - [MacBook index screenshot](docs/testing/device+browser-tests/macbook-index.jpeg)
    - [MacBook services screenshot](docs/testing/device+browser-tests/macbook-services.jpeg)
    - [MacBook reviews screenshot](docs/testing/device+browser-tests/macbook-reviews.jpeg)
    - [MacBook contact screenshot](docs/testing/device+browser-tests/macbook-contactform.jpeg)
    - [MacBook footer screenshot](docs/testing/device+browser-tests/macbook-footer.jpeg)

---

## FURTHER TESTING

- All features have been thoroughtly tested by myself on different screen sizes/operating systems, including all internal and external links, the form, music playlists, feedback page buttons, etc.

- The live project has been tested by family and friends, acting as first time visitors, on their own devices of different makes and sizes to make sure everything was working as designed. They checked all features mentioned above. They found issues mentioned on Bugs including heading size issues on iPhone 5SE, playlist activity issue that have been added to known bugs. They mentioned that the required fields on the contact form did not have any hints as being required, and adviced me to add the very well known required  asterisk to those fields. This has been edited as it was a great feedback for UX improvement.

---

## BUGS

1.  h1 font-size not reducing for big screens

    - Tried to make index.html h1 smaller in font-size for larger screens but something is not lettig the size get smaller.
      - When testing the responsivness of it, I can see the font-size
        reducing, but not in higher resolution screens.
      - It was a cache issue. After clearing the cache and restarting google Chrome, it's now responsive.

2.  Bootstrap toggle collapse is not working

    - The toggle icon is responsive and it appears when tested with dev-
      tools, but the dropdown menu is not working
    - SOLUTION: I noticed i forgot to place the jquery needed to make the Bootstrap
      JavaScript to work properly at the end of the file, before </body>. Found this solution reading the Boostrap documentation.

3.  In mobile screen, the dropdown items are not showing aligned and centered under the toggle icon

    - Fixed this removing mr-5 from class. This was giving nice looking spacing between the nav-links,
      but when rendering to phone view it gave too much margin in the right hand side.
    - To add spacing between the nav-links I added padding between them.

4.  In mobile screen, the card headings (h4) break and separate to the next line

    - I noticed in line 310 on the style.css file the margin was too large (margin: 20px 100px)
    - Changed the margin right and left to 70px, so when rendered to mobile, the h4 doesn't break in two and it's still balanced with the body of the cards, as well as the heading on the contact page.

5.  On desktop view, the review columns would render with 140px of margin in left and right.

    - SOLUTION: added a media queries for screens 992px and higher so the max width is 90%.
    - style.css line 384 +.

6.  On mobile view, there is a line across the footer dividing the footer in two colors.

    - I changed the max-height on line 134 of syle.css for min-height to match the height of the container content and added h-100 to the footer.
    - This has fixed the issue.

7.  When submitting the form, once filled the required fields and submitting the form, the page gave a 501 Error as showing in the image below.

    - I tried to fix this by adding another html page called response.html. I thought adding this the CTA button would ask the user to fill the required fields and then redirect them to a feedback page. But this did not work as when adding the response.html, the required attributes stopped working.

    - I contacted Code Institute tutor help and these were the outcomes: 
      - Scott suggested instead of trying to add another page I could use a modal to give the user a feedback. This wouldn't require to have a separated page and it would avoid the error from showing. But it also meant I had to add JS and jQuery, and eventhough I tried my hardest to learn fast and try to implement ( "form" ).submit(function() { into my head for responsiveness, the modal kept opening over the required fields and the function would not react to any changes.

      - I had to contact tutor support again and Tim helped me solving the issue. Unfortunatelly at this time of the course my skills are not advanced enough to add any JavaScript or functions. Tim advised me to remove the modal, as it wouldn't work as I intended without JS. After removing all code related to this, I noticed I still got the 501 error.

      - Tim noticed my form method=POST and action="/" were stopping my page from refreshing. So we changed the method to GET and removed action all together. This has solved the issue: if the user tried to submit the form without filling the required fields, the form won't submit and the user will get a notification under or over the field to be filled. When all information has been correctly filled and the user pushes the CTA button, the page will refresh leaving all fields empty to be used again.

      - Althought I would have liked to have some sort of feedback for the user to receive when they submitted the form, this couldn't be done at this time, but it would be implemented as a feature on future releases. (see [features left to implement](README.md) on README.md]

      ![screenshot showing the 501 ERROR](docs/testing/501-error.png)

    - _***EDIT & UPDATE: SOLUTION:***_ my mentor Rohit thought that for best user experience, users should be directed to a feedback page once they have submitted the form. After all the failed trials with tutor support, Rohit found a solution to the problem: on line 128 of contact.html he suggested to add :
      ```
      <form
         action="feedback.html"
         class="container-fluid contact-form"
         id="contactform"
         method="GET"
       >
      ```
    - by doing this the form redirects the user (not until all required fields are filled) into another page created in my workspace called feedback.html. Inside this page I created a thank you note and a button redirecting the user back to the home page.

8.  H1 on every page got smaller when I finished testing the pages on all devices:

  - I noticed all the h1s on all the pages were much smaller than supposed to. This happened because I added media queries to suit smaller screen sizes.

  - I fixed this by changing the media querie previously added from min-width: 810px to max-width: 810px. This allows the h1 to decrease on size when it reaches 810px or less and increase for bigger screens.

---

## KNOWN BUGS

- When clicked on the Spotify music list it plays 30 seconds of the list as a teaser for the song. The user needs to log into their spotify account to play the whole list. Premium account is needed to access Spotify.

  - There is three playlist each embedded inside an iframe. During the testing I noticed that if I play a second playlist, the first one does not stop, but as it's an external code, I do not have the way to fix this with my actual knowledgde and skillset. So the playlists have to manually be paused, otherwise they all play at the same time.

- In some screens a white line appears under the map eventhough I fixed this for big screen sizes like laptops and desktops. This can be seen on some smaller phone sizes. For more info please see Device Responsiveness tables.

  - Although I reviews this bug on Devtools, I haven't been able to find a solution for this as for today.

- The third inline block at the footer appears not to be centered (Maialen & Sua , Bettystown | Ireland). I tried to fix this but all the changes I did on Devtools did not show any changes.

- On some devices/browsers, the background color of the sections seem to get a little darker than the parent container fluid, but I could not manage to fix this.

---

---

## <center> Back to [README.md](README.md)

---

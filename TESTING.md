
# TESTING DOCUMENT | **Wet Paws** | Dog Walking and Sitting Services

## OVERVIEW

This being my first ever project in Web Development, I need to start saying that I did encounter quite a few obstacles that made me start the project from the begining once or twice (as seen in a commit history).

As my project started taking form and I could visualize it on a browser as I went along, I felt more and more confident on what i was doing, even trying new things like adding music tracks and trying different hover styles.

But I still had to redo a few things that did not quite work as I planned, like loading libraries, js, jQuery... 

From the very beginning I used Google Chrome Dev Tools to style and fix my code, so thanks to that I found it much easier to see real time changes and add the write css/code to my workspace.

Once finished, I planned to test my site on a few different phones, laptop, tablet and desktop:

- Samsung Galaxy S8+ (My personal device) (mobile device)
- Samsung A70 (mobile device)
- Iphone 11 (mobile device)
- Xaomin (mobile device)

- Samsung S5 (tablet)

- HP Envy 13" (laptop)

- PC desktop 32" screen 

## Table of Content

1. [USER STORIES](#user-stories)
2. [FAVICON TEST](#favicon-test) 
3. [VALIDATOR CHECKS](#validator)
    - [HTML](#html-validator)
        - Index.html
        - Services.html
        - Contact.html
    - [CSS](#css-validator)
4. [LIGHTHOUSE TESTING](#lighthouse-testing)
5. [BUGS](#bugs)

## USER STORIES

- As a visiting user I want to:
    - Find out what the company is about.
    - Easily visualize and understand what services the company offers.
    - Be able to use and book one or more services the company has to offer.
    - Be able to use the contact form for the business and service enquiries.
    - Have the option to personalize the services offered.
    - Feel that the company cares and I can trust them caring for my loved dog by seeing other peoples reviews.
    - Be able to know more about the owner by having the option to personally meet them.
    - Know the location of the business and know where those services are offered.
    - Get in touch with the business easily by having contact details clearly available.
    - Be able to book a service quickly by having a direct tab to the contact form.
    - Find social links to be able to follow the business in social media platforms.

---

## FAVICON TEST

I noticed when I introduced the first and second favicon I could not see the shape on the brower tab as they were very
blurry and unidentifyable, so I created a new favicon with bold black color and simple shape, so it can be easily identified 
in between the rest of the opened tabs. This change has improved the user experience as I can identify the site's tab in one
fast look.

- [Favicon 1](docs/favicon_test/test-favicon1.png)
- [Favicon 2](docs/favicon_test/test-favicon2.png)
- [Chosen Favicon](docs/favicon_test/test-favicon3.png)

As seen in the examples above, the new favicon is visually more appealing than the first two.

---

## VALIDATOR:

As I wrote my code during the whole project, I continuouly checked my code using [W3 Validator](https://validator.w3.org/#validate_by_uri) to make sure I fixed my code as I wrote it. At the end of the project I ran all the finished pages and made sure all the errors were fixed (see below).

As a css validator I also used [w3 Validator](https://jigsaw.w3.org/css-validator/) to make sure it checked my style.css file to CSS level 3 + SVG standards. 

(See passed validator results at the end of [HTML](#results-after-fixing-validator-errors) and [CSS](#results-for-css-validator-check) sections.

### HTML VALIDATOR:

Test results and errors to be fixed (after the first check):

- The type attribute is unnecessary for JavaScript resources.
    - I removed the type attribute form them.


- Some of the images are not loading and the path seems to be broken
    - I checked with dev-tools on google chrome. 
    - I fixed this fixing the source path where I made a mistake (my assets 
    directory is called static, but I wrote assets/images)
    - It's fixed. All pictures are showing as they are meant to and they are responsive

- missuse of Aria attribute (Aria-label) on line 65 (span aria-label="image of an ..."). 
    - To make it accessible and have an image description I added a role="img" to be able make a relevant description of the purpose of the parent element.


INDEX.html

- line 152: text-center not allowed on div
    - fixed error adding class="text-center"

 - line 155: Attribute target not allowed on element iframe at this point. 
    - removed all target attributes from iframe elements.

- line 155:  Attribute autoplay not allowed on element iframe at this point.
    - removed autoplay from iframe elements

- line 158: The frameborder and allowtransparency attribute on the iframe element are obsolete.
    - to comply with the w3 validator, I added inline styles to the iframes (style="border:none;") and removed allowtransparency="true as I didn't need it.

- line 172:  Bad value 100% for attribute width on element iframe: Expected a digit but saw % instead.
    - removed width="100%" and added class="w-100" to the map iframe 

- line 170: section is missing a header
    - added h2 to map section for better accessibility and organization of information

SERVICES.html

 - line 148: No p element in scope but a p end tag seen.
    - error: a ul element was inside the p element. To fix this i closed the p element in line 138 and put the ul as a child of div (card-body) 

- line 170: Attribute heigh not allowed on element img at this point.
    - Fixed by removing height and width from the img element and added them using css under .img-responsive (style.css line 350, 351)

- line 170:  An img element must have an alt attribute
    - added alt attribute to all img elements within article element on lines 170, 191, 214, 235.

- line 162:  Article lacks heading. Consider using h2-h6 elements to add identifying headings to all articles.
    - moved h2 from line 164 to line 163 over the div-reviews element.

CONTACT.html 

- line 169: Element h5 not allowed as child of element label in this context.
    - removed h5 element from label. I added the id="tell-more" to the label and styled the same way as h5 (style.css line 397)

---

Results after fixing Validator errors

- [Index.html Validator result](docs/testing/index.html-w3-pass.png)

- [Services.html Validator result](docs/testing/services.html-w3-pass.png)

- [Contact.html Validator result](contact.html-w3-pass.png)

---

### CSS VALIDATOR 

Results for CSS validator check

- [CSS Validator result](docs/testing/CSS-validator-pass.png)

---
### LIGHTHOUSE TESTING

Using DevTool's Lighthouse tester, I checked all pages on mobile and desktop to make sure the scores were as high as I posibly could. Below you can find the results and scores of first time tests and after implementing suggestions that the tool offered:

- Phone 
    - Index.html Lighthouse test:

        - [Before](docs/testing/index-phone-before) implementing changes: 
            - The performance score was very low and in red. This was due to very big images and unused javascript libraries. To fix that I reduced all images with Tinypng and cropped them to make equal squares. I also changed two of the images as it was impossible to make them any lower on weight without pixelating them and they ended up not looking too good. I also changed the grid system so all pictures show on top of each other in mobile view.
        -[After](docs/testing/lighthouse-mobile-after-index) following lighthouse suggestions:
            - I managed to increase the very low performance score to 74%. Although this is not ideal, I found it very difficult to implement any more changes as this meant to add attributes to elements that made the validator fail. So I decided to leave the index at this level until I have more time for further changes and improvements.

    - Services page Lighthouse test:
        - [Before](docs/testing/services.html-phone-before.png) implementing changes
            - as in the index page, the performance score was quite low because of the weight of the images
        - [After](docs/testing/services.html-phone-after.png) following lighthouse suggestions:
            - once I implemented the suggestions given by the lighthouse tool, the score increased to 84%. I decreased the size of the images and added meta data to the head for better SEO (%100)

    - Contact page Lighthouse test:
        - [Before](docs/testing/contact.html-before.png)
        - [After]()



## BUGS


1. h1 font-size not reducing for big screens
    - Tried to make index.html h1 smaller in font-size for larger screens but something is not lettig the size get smaller.
        - When testing the responsivness of it, I can see the font-size
        reducing, but not in higher resolution screens.
        - It was a cache issue. After clearing the cache and restarting google Chrome, it's responsive.

2. Bootstrap toggle collapse is not working
    - The toggle icon is responsive and it appears when tested with dev-
    tools, but the dropdown menu is not working
    - SOLUTION: I noticed i forgot to place the jquery needed to make the Bootstrap
    JavaScript to work properly at the end of the file, before </body>.

3. In mobile screen, the dropdown items are not showing alignedand centered under the toggle icon
    - Fixed this removing mr-5 from class. This was giving nice looking spacing between the nav-links,
    but when rendering to phone view it gave too much margin in the right hand side.
    - To add spacing between the nav-links I added padding between them.

4. In mobile screen, the card headings (h4) break and separate to the next line
    - I noticed in line 310 on the style.css file the margin was too large (margin: 20px 100px)
    - Changed the margin right and left to 70px, so when rendered to mobile, the h4 doesn't break in two
    and it's still balanced with the body of the cards, as well as the heading on the contact page.

5. on desktop view, the review columns would render with 140px or margin in left and right.
    - SOLUTION: added a media queries for screens 992 and higher so the max width is 90%.
    - style.css line 384 +.

6. on mobile view, there is a line across the footer divingding the footer in two colors.
    - I changed the max-height on line 134 of syle.css for min-height to match the height of the container content and added h-100 to the footer. 
    - This has fixed the issue.

---

Back to [README.md](README.md)
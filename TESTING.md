# TESTING DOCUMENT

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

3. In mobile screen, the dropdown items are not showing aligned
and centered under the toggle icon
    - Fixed this removing mr-5 from class. This was giving nice looking spacing between the nav-links,
    but when rendering to phone view it gave too much margin in the right hand side.
    - To add spacing between the nav-links I added padding between them.

4. In mobile screen, the card headings (h4) break and separate to the
next line
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

## VALIDATOR:

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

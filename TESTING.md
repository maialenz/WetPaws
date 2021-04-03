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

## BUGS

---

### Bug 1 - h1 font-size not reducing for big screens
- Tried to make index.html h1 smaller in font-size for larger screens
but something is not lettig the size get smaller.
    - When testing the responsivness of it, I can see the font-size
    reducing, but not in higher resolution screens.
    

### Bug2 - Bootstrap toggle collapse is not working
    - The toggle icon is responsive and it appears when tested with dev-
    tools, but the dropdown menu is not working
    - SOLUTION: I noticed i forgot to place the jquery needed to make the Bootstrap
    JavaScript to work properly at the end of the file, before </body>.

### Bug 3 - In mobile screen, the dropdown items are not showing aligned
and centered under the toggle icon


## VALIDATOR:

---

- 28/03/2021 - Test result:
    - The type attribute is unnecessary for JavaScript resources.
        - I removed the type attribute form them.


- Some of the images are not loading and the path seems to be broken
    - I checked with dev-tools on google chrome. 
    - I fixed this fixing the source path where I made a mistake (my assets 
    directory is called static, but I wrote assets/images)
    - It's fixed. All pictures are showing as they are meant to and they are responsive
## REFERENCES USED TO LEARN, PERFECT AND FIX ISSUES FOUND ON THE CODE: 

### Bootstrap library documentation

- To refresh on lessons on the course, I rewatched videos explained by [Matt Rudge](https://github.com/lechien73) from [Code Institute](https://codeinstitute.net/) as well as previous projects done during th course (Coders Coffee House project, Love Running project, CV project, Whiskey Drop Project...)[maialenz](https://github.com/maialenz/Bootstrap-lesson-walkthrough/blob/master/)

- To create the decoration of the social links on the footer, I used the whiskey drop lesson on bootstrap from Code Institute. Lesson by [Matt Rudge](https://github.com/lechien73)
    ``` 
    .social-links li a i {
    width: 40px;
    height: 40px;
    padding: 16px 0;
    border-radius: 50%;
    font-size: 15px;
    line-height: 7px;
    text-align: center;
    color: #373d3f;
    background-color: #dae0e5;
    transition: all 0.35s ease-in-out;
    -moz-transition: all 0.35s ease-in-out;
    -webkit-transition: all 0.35s ease-in-out;
    -o-transition: all 0.35s ease-in-out;
    }
    ```
    
- As template for the README.md I used the template created by [Code Institute](https://github.com/Code-Institute-Solutions/SampleREADME#)

- Bootstrap navbar for responsive navigation header:
[Bootstrap documentation](https://getbootstrap.com/docs/4.0/components/navbar/#placement)

- Bootstrap form examples and template used in content.html
[Bootstrap documentation](https://getbootstrap.com/docs/4.0/components/forms/) - by Bootstrap

- Bootstrap button for CTA 
[Bootstrap documentation](https://getbootstrap.com/docs/4.0/components/buttons/) - by Bootstrap

- Bootstrap input width to make age field certain size:
[Bootstrap helpers](https://mdbootstrap.com/snippets/jquery/ascensus/143796) - by Michal Szymanski

- Bootstrap cards for service cards:
[Bootstrap documentation](https://getbootstrap.com/docs/4.0/components/card/)

- Bootstrap Spacing and Gutters: Margin and Padding: used to fix issues with cards bottom padding in services.html
[Bootstrap documentation Spacing](https://getbootstrap.com/docs/5.0/utilities/spacing/)
[Bootstrap documentation Gutters](https://getbootstrap.com/docs/5.0/layout/gutters/)

- Bootstrap Media Objects: "EDIT" i modified the media classes and removed them from my code as they were not responding as I wanted them to.
[Bootstrap documentation](https://getbootstrap.com/docs/4.0/layout/media-object/)

- Bootstrap Typography: Blockquotes: used as a reference to add blockquote elements to the review section in services.html
[Bootstrap documentation](https://getbootstrap.com/docs/5.0/content/typography/#blockquotes)


---

### LOCATIONS AND CODES WHERE I FOUND SOLUTIONS TO MY QUESTIONS/ISSUES/...:

- Picture transparency
[w3schools](https://www.w3schools.com/css/css_image_transparency.asp)

- Using figure tag
[W3schools](https://www.w3schools.com/tags/tag_figure.asp)

- Meta Descriptions 
[Seobility](https://www.seobility.net/en/wiki/Meta_Description?utm_source=google&utm_medium=cpc&utm_campaign=wiki_en&utm_term={meta%20description}&utm_content=lp_meta_description&gclid=CjwKCAjwjbCDBhAwEiwAiudBy-epL2rpkLLDqJb88jp65G95F3nlQOuhmnIzONLDApkr03Q6_vQu3BoCpDoQAvD_BwE)

- Navbar visual examples used for navbar collapsable toggle and modified to suit my own code:
[Forked by Skelly](https://www.codeply.com/go/kTGlK9Axdk)
        ```
        <nav class="navbar navbar-light navbar-expand-md bg-light justify-content-center">
            <a href="/" class="navbar-brand mr-0">Brand</a>
            <button class="navbar-toggler ml-1" type="button" data-toggle="collapse" data-target="#collapsingNavbar2">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="navbar-collapse collapse justify-content-between align-items-center w-100" id="collapsingNavbar2">
                <ul class="navbar-nav mx-auto text-center">
                    <li class="nav-item active">
                        <a class="nav-link" href="#">Link <span class="sr-only">Home</span></a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="//codeply.com">Codeply</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Link</a>
                    </li>
                </ul>
                <ul class="nav navbar-nav flex-row justify-content-center flex-nowrap">
                    <li class="nav-item"><a class="nav-link" href=""><i class="fa fa-facebook mr-1"></i></a> </li>
                    <li class="nav-item"><a class="nav-link" href=""><i class="fa fa-twitter"></i></a> </li>
                </ul>
            </div>
        </nav>
        ```

- Bootstrap Navbar toogle .collapse not working
[Stack Overflow](https://stackoverflow.com/questions/41497826/bootstrap-toggle-collapse-not-working) - answered by Saroj
> "Make sure you are loading all the libraries correctly,do open your debugger and check if everything is loaded. one more thing load jquery before boostrap.js"

- Where to load the ajax/js libraries on the html page
[Stack Overflow](https://stackoverflow.com/questions/7669996/where-is-the-best-place-to-put-javascript-ajax-in-a-document) - asnwered by Tamzin Blake
> "In general, unless for some reason you need it elsewhere, put all of your JS last in the body. The browser won't continue until it's parsed your JS, so it is nice to let the page load first. See http://developer.yahoo.com/performance/rules.html"

- How to draw a border around the cards used in services.html
[Stack overflow](https://stackoverflow.com/questions/9102900/css-outside-border) - answer by Bear In Hat
> "Border affects the outside edge of the element, making the element different in size. Outline will not change the size or position of the element (takes up no space) and goes outside the border." 

- How to make all Bootstrap cards the same height (services.html)
[Stack Overflow](https://stackoverflow.com/questions/35868756/how-to-make-bootstrap-4-cards-the-same-height-in-card-columns#:~:text=You%20can%20apply%20the%20class,which%20stands%20for%20height%20100%25.&text=UPDATE%3A%20In%20Bootstrap%204%2C%20flexbox,will%20fill%20to%20full%20height.) - answer by user3350279 
> "With "col-sm-12 col-lg-6" I've made the cards responsive. With "card h-100" I've set all cards to the height of their parent column. On my system this works, but I'm not a pro. So, hopefully I helped someone."

- How to center the Reviews images in the middle of the column
[Starck Overflow](https://stackoverflow.com/questions/18462808/responsive-image-align-center-bootstrap-3) -answer by Bojangles
> This is a pleasantly easy fix. Because .img-responsive from Bootstrap already sets display: block, you can use margin: 0 auto to center the image"

- How to Embed a Spotify Playlist on Your Website
[Jimdo](https://www.jimdo.com/blog/embed-spotify-playlist-on-website/)
> 1.Open up your Spotify account and find your band’s music.
> 2. Click on the album or playlist you want to share.
> 3. Click on the icon with the three dots “…” > “Share” and choose “Copy Embed Code.” 
> 4. Return to your site and paste the code for your Spotify iframe into a Widget/HTML element. 

- How to add images to README.md 
[Stack overflow](https://stackoverflow.com/questions/14494747/how-to-add-images-to-readme-md-on-github) - asnwer by captainclam
> Try this markdown:![alt image](http://url/to/img.png)

- SOLUTION to the issue with the form submission. Code fixed by ROHIT SHARMA -mentor to my MS1 project. (To see more information about the steps taken to fix this bug, see [TESTING.md document](TESTING.md))
    - line 128 on contact.html
        ```
        <form
            action="feedback.html"
            class="container-fluid contact-form"
            id="contactform"
            method="GET"
          >
        ```


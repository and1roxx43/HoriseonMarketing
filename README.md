# Project Name: HTML, CSS, and GIT: Code Refactor
___
## OVERVIEW

HORISEON Marketing, a marketing agency has acquired a developer to refactor an existing site to make it more accessible for people with disabilities and to improve optimisation for search engines.

The web page and source code should meet the following acceptance criteria:

- Source code should be semantic HTML elements.
- The elements follow a logical structure independent of styling and positioning.
- All images should find accessible alt attributes.
- The heading attributes should fall in sequential order.
- The Title element should be concise and descriptive.
- All links should be functional.
- Comments added before each HTMl elements and CSS element selector.


___
## Task

- Replace all div elements with semantic HTML elements and all images added an alt attributes to improve readability, and accessibility for people with disabilities and search engine optimisations.
- Replaced empty div with a section element and an image element, and added an alt attribute.
- Descriptive title added.
- css selector altered, and modified as too many repetitions.
___
## HTML code added (changes made)

1. First div was replaced with a header element
```html

    <header></header>
```  

2. Second div replaced with a nav element
```html

    <nav></nav>
```  

3. Third div replaced with an image element within a section element 
```html

    <section class="hero">
        <img  src="./assets/images/digital-marketing-meeting.jpg" alt="page banner">
    </section>
```  

4. Forth div element was replaced with the main element including 3 article elements

```html
    <main>
        <article><article>
    </main>
```

5. Fifth div element was replaced with a section element including 3 aside elements

```html
    <section>
        <aside></aside>
    </section>

```

6. Sixth div was replaced with a footer element

```html
    <footer></footer>
```

### Errors found from original

1. First link was not functioning correctly.

```html
    <li>
      <a href="#search-engine-optimization">Search Engine Optimization</a>
    </li>

    <!--Missing an id attribute to first link navigation -->
    <article id="search-engine-optimization" class="search-engine-optimization">
```

2. Image banner did not provide accessibilty to people with disabilities

```html
    <!--Section area to hold banner-->
    <section class="hero">
        <img  src="./assets/images/digital-marketing-meeting.jpg" alt="page banner">
    </section>
        <!--section banner ends here-->
```

3. 
```html
    <!--Image tag had an opening and a closing tag, fixed with a self closing tag-->
    <img src="./assets/images/cost-management.png" alt="cost-management logo" />
```

___

## CSS code altered

```css

header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}

/* Sets h1 within parent selector to display to inline block and font-size 48px*/
header h1 {
    display: inline-block;
    font-size: 48px;
}

/* Sets class seo span color */
header h1 .seo {
    color: #d9dcd6;
}

/* -- Nav selector -- */

/* Sets padding-top 15px, margin-right 20px, float-right, font-family, font-size 20px to nav seletor */
header nav {
    padding-top: 15px;
    margin-right: 20px;
    float: right;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 20px;
}

/* Remove list style from ul child of nav */
header nav ul {
    list-style-type: none;
}

/* Display li in inline-block and set a margin-left of 25px */
header nav ul li {
    display: inline-block;
    margin-left: 25px;
}

/* removed background-image for accessibility from HTML from class hero.

Sets a height to 800px, width: 100%, and a margin-bottom of 25px 
*/
.hero {
    height: 800px;
    width: 100%;
    /* background-image: url("../images/digital-marketing-meeting.jpg"); */
    margin-bottom: 25px;
}

/* 
Added a Section elemen to hold the image selector
Sets height and width to 100%, background-size, background-size and background-position
*/
.hero img{
    height: 100%;
    width: 100%;
    background-size: cover;
    background-position: center;
}
```
```css
/* Sets main element selector width to 75%, display to inline-block, and margin-left to 20px */
main {
    width: 75%;
    display: inline-block;
    margin-left: 20px;
}
```

```css
footer {
    padding: 30px;
    clear: both;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    text-align: center;
}

/* Sets font-size to 20px */
footer h2 {
    font-size: 20px;
}
```
___
## Review url 

Deployed application URL:

```
https://and1roxx43.github.io/HoriseonMarketing/
```
GitHub repository URL

```
https://github.com/and1roxx43/HoriseonMarketing
```
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
## Resolution 

- All div elements were replaced with semantic HTML elements and all images added an alt attributes.
- Empty divs were replaced with semantic HTML and background image added and alt attribute.
- Descriptive title added.
- css selector altered.
___
## HTML code added

1. First div was replaced with a header element
```html

    <header class="header"></header>
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

5. Fifth div element was replaced with a section element including 3 article elements

```html
    <section>
        <article></article>
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
Sets height and width to 100%, background-size, background-size and background-position
*/
.hero img{
    height: 100%;
    width: 100%;
    background-size: cover;
    background-position: center;
}
```

___

Deployed application URL:

```
https://and1roxx43.github.io/HoriseonMarketing/
```
GitHub repository URL

```
https://github.com/and1roxx43/HoriseonMarketing
```
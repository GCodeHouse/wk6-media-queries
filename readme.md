# Responsive Web Design - Media Queries
In this exercise, you'll be practicing writing media queries in CSS to make your web page responsive to different screen sizes.

## Download the Code
You can get the code for the exercises by either [cloning this GitHub repository](#clone-repository) onto your computer, or [copying the source code](#copy-source-code) and pasting it into files in VS Code.

### Clone Repository
* In GitHub Desktop, click on File > Clone repository (Ctrl/Cmd + Shift + O)
* Select URL tab
![screenshot of a window in GitHub Desktop for user to clone a repository](image.png)
* Paste the link to this repository `https://github.com/GCodeHouse/wk6-media-queries.git` into the Repository URL field, and choose where on your computer you'd like to download the repository, then click Clone

[Move on to exercise](#design-the-page-for-a-small-screen)

### Copy Source Code
* Create a new folder on your computer where you would like to store your code, then open that folder in VS Code
* Create a new file called `index.html`
* Create another new file called `media-query-example1.css`
* Open this link (right-click and open in new tab): [Media Query Exercise HTML](http://web.simmons.edu/~grovesd/comm328/demo/media-query-exercises/media-query-example1.html)
    * Right-click anywhere on the page and select "View Page Source" from the dropdown menu (Ctrl/Cmd + U)
    * Select all text on the page (Ctrl/Cmd + A), then copy it (Ctrl/Cmd + C) and paste it (Ctrl/Cmd + V) into your 'index.html' file
* Open this link (right-click and open in new tab): [Media Query Exercise CSS](http://web.simmons.edu/~grovesd/comm328/demo/media-query-exercises/media-query-example1.css)
    * Select all text on the page and paste it into your 'media-query-example1.css' file

## Design the Page for a Small Screen
* Open the HTML file using the Live Preview extension in VS Code. The Live Preview panel should have an address bar at the top of it that looks something like this:

![screenshot of Live Preview panel address bar in VS Code](image-1.png)

* Copy that address into the address bar of a tab in your external browser of choice and load the page in that browser. Doing this will allow you to expand your browser window and the web page to the full-width of your screen, unlike VS Code Live Preview. This will also allow you to test the media queries you’ll be writing during this exercise. 
    * Updates to your page may not happen automatically in your external browser, so make sure to refresh the page anytime you make changes to your HTML or CSS.
* Use your mouse to grow and shrink the width of the browser window containing the Media Query Exercise 1 HTML page from above. Watch how it changes as the browser window’s width grows and shrinks, then leave it at a small size to simulate what the page might look like on a mobile device.

### Adjust CSS to fine-tune how the page displays
* Add ids to different elements on the page that you may want to target
* Make the page's font-size larger
* Make the h1 font-size smaller
* Add a small amount of margin to the page edges

By designing for the small screen first we're using what is known as a *mobile first* approach. By doing this, we start with a basic design or lowest common denominator and then work on enhancing more sophisticated browsers with advanced features or layouts. This ensures that we're designing an experience that will work smoothly for as many users as possible. It also can have the added benefit of helping us realize what content on our website is most important and the content we might be able to do without.

Ask the facilitator to demonstrate responsive design browser tools depending on what browser you’re using. These tools will help simulate the screen size and/or DPI of different resolutions, tablet, phone and mobile devices.

### Finding your browser window size
In Chrome you can easily find out what size your browser window is by using the Web Inspector. Open the web inspector in Chrome and resize your browser window while watching the top right corner. The pixel dimensions should appear as you resize.

### Introduce a new breakpoint
Start expanding your browser window width. Do this until you get to a point where the design no longer works. For example, the line length might become too long for the text to be easily readable. Or perhaps the page becomes wide enough that it no longer makes sense for the images to display in a stack.

Record the width of the browser window at this point. This will be your first *breakpoint*. A breakpoint is simply a point at which we're defining that the design should change.

Create a new media query in your browser using the pixel dimension you recorded as the `min-width` media feature test. Within this breakpoint, change your CSS to do the following:
* Change the background color to help you see when the media query takes effect
* Adjust the font-size if necessary
* Adjust the page margins
* Make the photos display in two columns

### Create another breakpoint for large screens
Resize your browser window again to find another breakpoint. Add a new media query in your CSS and adjust the following rules:
* Change the background color
* Adjust the font-size if necessary
* Adjust the page margins
* Make the photos display in three columns
* Add a max-width to the page to make sure the line length never gets too long

## See Completed Example
Below is an example of a finished CSS solution. Yours will likely look different, but should have similar media queries.
<details>
<summary>Sample CSS solution</summary>

```css
/* 
 * @see http://www.paulirish.com/2012/box-sizing-border-box-ftw/
 * apply a natural box layout model to all elements, but allowing components to change 
 */
html {
  box-sizing: border-box;
}
*, *:before, *:after {
  box-sizing: inherit;
}


body {
  font: 1.2em/1.2 Helvetica, aria, sans-serif;
  margin: 0 3%;
}

h1 {
  font-size: 1.8em;
  margin: .9em 0 0 0;
}

h2 {
  font-size: 1.5em;
  margin: 1.5em 0 0 0;
}

img {
  max-width: 100%;
}
figure {
  background: black;
  border-radius: 5px;
  color: white;
  margin: 0 0 25px 0;
  padding: 10px;
  text-align: center;
  
}

figcaption {
  font-size: .8em;
}


@media screen and (min-width: 794px) {
  body {
    background: rgba(0,0,255,.2);
    margin: 25px 6%;
  }
  
  figure {
    float: left;
    width: 45%;
    margin-right: 4.5%;
  }
}


@media screen and (min-width: 1020px) {
  body {
    background: rgba(0,255,0,.2);
    margin: 25px 10%;
    max-width: 1130px;
  }
  
  figure {
    width: 30%;
    margin-right: 2.5%;
  }
}
```
</details>
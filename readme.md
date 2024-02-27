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
* Open the HTML file you created above using the Live Preview extension in VS Code. The Live Preview panel should have an address bar at the top of it that looks something like this:

![screenshot of Live Preview panel address bar in VS Code](image-1.png)

* Copy that address into the address bar of a tab in your external browser of choice and load the page in that browser. Doing this will allow you to expand your browser window and the web page to the full-width of your screen, unlike VS Code Live Preview. This will also allow you to test the media queries you’ll be writing during this exercise. 
    * Updates to your page may not happen automatically in your external browser, so make sure to refresh the page anytime you make changes to your HTML or CSS.
* Use your mouse to grow and shrink the width of the browser window containing the Media Query Exercise 1 HTML page from above. Watch how it changes as the browser window’s width grows and shrinks, then leave it at a small size to simulate what the page might look like on a mobile device.

### Adjust CSS to fine-tune how the page displays
* Add ids to different elements on the page that you may want to target
* Make the page's font-size larger
* Make the h1 font-size smaller
* Add a small amount of margin to the page edges

By designing for the small screen first we're using what is known as a <span style="color:red">mobile first</span> approach. By doing this, we start with a basic design or lowest common denominator and then work on enhancing more sophisticated browsers with advanced features or layouts.
# [Rock Hammer](http://stuffandnonsense.co.uk/projects/rock-hammer/)

[Rock Hammer](http://stuffandnonsense.co.uk/projects/rock-hammer/) is dedicated to [Alex Clarke](http://beardyscientist.com), a real life geologist.

What’s Rock Hammer? It’s a curated project library for [Hammer For Mac](http://hammerformac.com) designed and developed by [Stuff and Nonsense](http://stuffandnonsense.co.uk) and friends. Rock Hammer contains baseline typography, styling for common HTML elements including images, forms and tables, as well as navigation, responsive modules and widgets. These are the foundation for every project we start. Rock Hammer can be used as a design/style template or pattern primer or as the foundation for developing a responsive website.

Clone the repo, `git clone git@github.com:malarkey/Rock-Hammer.git`, (whatever that means) or [download the latest release](https://github.com/malarkey/rock-hammer/zipball/master).





## 1. Getting started with Rock Hammer

Rock Hammer works with [Hammer For Mac](http://hammerformac.com). If you develop in Windows or you don’t (yet) use Hammer, skip to the section ‘Using Only the Build Folder‘ below.

For styling, Rock Hammer uses [Sass](http://sass-lang.com). Hammer For Mac compiles Sass into CSS so you won’t need the Terminal. In most cases, you’ll need to edit just three .scss files to get started:

### _imports.scss

Configure which Sass partials you need for your individual project. We’ve included some of the most useful parts of Bootstrap, but if you don’t need styles for a carousel or a hero box, there’s no sense in including them. Comment out the partials you don’t need with // at the the beginning of the line on which that partial appears.

### lte-ie8.scss

For versions of Microsoft Internet Explorer that didn’t implement CSS3 Media Queries, this file contains compiled styles from all stylesheets, including those inside Media Queries. These are served up using a completely configurable, conditional class to identify those styles and only apply them to Internet Explorer 8 and before. Use this file to also serve styles specifically to Internet Explorer 8 and before.

### _config.scss

You’ll do most of your work in this config file; everything from setting typefaces and choosing colours to defining styles for HTML elements and widgets. Follow steps one to four for the broadest brushstrokes, then make finer strokes by defining styles for popular interface elements:

### 1. NAVIGATION				

-   Site navigation				
-   Basic navbar				
-   Breadcrumbs					
-   Pagination
-   Pager

### 2. MODULES

-   Hero
-   Alerts
-   Wells

### 3. FORMS
   
-   Inputs
-   Help						
-   Buttons

### 4. TABLES
### 5. MISC





## 2. Rock Hammer’s structure

Rock Hammer includes Sass partials for the three components of ‘design atmosphere:’

2.1. **Colour**: Emotion and interaction vocabulary.

2.2. **Typography**: Typefaces, type treatments and white space.

2.3. **Texture**: Decorative elements, line-work, patterns and shapes.

2.4. **Partials**:

-   Site-wide styles
-   Misc HTML elements
-   Placeholders for Modernizr classes
-   @2x images

2.5. Utilities such as mixins, normalise and reset and print styles.

2.6. Layout for structural styles. Use it in combination with breakpoint files _bp2 – bp6 as required.

2.7. Speaking of breakpoints, there are six placeholder breakpoint values included. Use and change them as you need in conjunction with the media-query-bp mixin within your SASS selectors. The defaults are:

-   $bp2 		480px		30em		
-   $bp3 		600px		37.5em  	
-   $bp4 		768px		48em 		
-   $bp5 		992px	 	62em		
-   $bp6 		1382px		86.375em 	

2.8. Matching HTML partials and Sass partials for forms, tables, navigation and other commonly used interface elements derived from Bootstrap. If there are Bootstrap components you use regularly, add them to the partials folder. Don’t forget to reference them from _imports.scss too. Certain Bootstrap plugins require JavaScript to work correctly, so ensure that the required JavaScript files are referenced correctly from the _scripts.html partial. There are a couple of dependencies with Bootstrap plugins, but these are explained in the comments found in _scripts.html.

2.9. Matching HTML partials and Sass partials for responsive navigation patterns. We’ve included three popular patterns but feel free to add more. Brad Frost’s [Responsive Patterns](http://bradfrost.github.com/this-is-responsive/patterns.html#navigation) is a cracking place to start.

-   _navigation-footer-anchor.scss
-   _navigation-left-nav-flyout.scss
-   _navigation-toggle.scss

To use these navigation patterns: 

-   Copy the HTML from your chosen pattern into the <body> of a new template
-   Uncomment the pattern you’ve chosen in rock-hammer.scss
-   Uncomment the pattern you’ve chosen in _scripts.html





## 3. Using Only the Build Folder

We built Rock Hammer to work with [Hammer For Mac](http://hammerformac.com). It’s great. You should try it. But if you develop on Windows or haven’t yet used Hammer:

1.  First, you’re weird. Nice. But weird. Sorry.

2.  You can still use Rock Hammer’s compiled HTML, CSS and Javascript. It won‘t be as good as developing from the original Rock Hammer, but what are you going to do?









### CSS Preprocessor Options

+ SCSS





## Author

**Andy Clarke**

+ http://twitter.com/malarkey
+ http://github.com/malarkey
+ http://stuffandnonsense.co.uk

### Default theme design






**Sue Davies**

+ http://twitter.com/suehayesdavies






### Javascript

**Aaron Allport**

+ http://twitter.com/aaronallport
+ https://github.com/aaronallport
+ http://www.aaronallport.com






### Components

1.  [320 and Up](http://stuffandnonsense.co.uk/projects/320andup)
2.  [Bootstrap](http://twitter.github.com/bootstrap)
3.  [jQuery](http://jquery.com)
4.  [Modernizr](http://modernizr.com)
5.  [Responsive Patterns](http://bradfrost.github.com/this-is-responsive/patterns.html)
6.  [Selectivizr](http://selectivizr.com)
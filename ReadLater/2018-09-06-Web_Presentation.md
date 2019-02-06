# How To Build A Captivating Presentation Using HTML, CSS, & JavaScript

![](https://cdn-images-1.medium.com/max/2000/1*d57o560SJ8jthOajFUxMfA.jpeg)

Building beautiful presentations is hard. Often you’re stuck with Keynote or
PowerPoint, and the templates are extremely limited and generic. Well not
anymore.

Today, we’re going to learn how to create a stunning and animated presentation
using HTML, CSS, and JavaScript.

If you’re a beginner to web development, don’t fret! This tutorial will be easy
enough to keep up with. So let’s slide right into it!

![](https://cdn-images-1.medium.com/max/2000/1*CN43a2YgQ82c5Fl1wIoZ2A.png)

We’re going to be using an awesome framework called
[Reveal.js](https://revealjs.com/#/). It provides robust functionality for
creating interesting and customizable presentations.

1.  Head over to [the Reveal.js repository](https://github.com/hakimel/reveal.js)
and clone the project (you can also fork this to your GitHub namespace).

![](https://cdn-images-1.medium.com/max/1600/1*S_ZYbkd7Y6j1_Lj1RE0sWg.png)

2. Change directories into your newly cloned folder and run `npm install` to
download the package dependencies. Then run `npm start` to run the project.

![](https://cdn-images-1.medium.com/max/1600/1*Pw39d6yELnp3yckd8UBAfQ.png)

The `index.html` file holds all of the markup for the slides. This is one of the
downsides of using Reveal.js; all of the content will be placed inside this HTML
file.

![](https://cdn-images-1.medium.com/max/2000/1*m53gA3UQzLjzYBGFlaNtDQ.png)

### **Built-In Themes**

Reveal includes 11 built-in themes for you to choose from:

![](https://cdn-images-1.medium.com/max/2600/1*ap5v9NJodgzByZEJzMCGfA.jpeg)

#### Changing The Theme

1.  Open `index.html`
1.  Change the CSS import to reflect the theme you want to use

![](https://cdn-images-1.medium.com/max/2000/1*mAPjCb73GiiiJUHEnRInOQ.png)

**The theme files are:**

* beige.css
* black.css
* blood.css
* league.css
* moon.css
* night.css
* serif.css
* simple.css
* sky.css
* solarized.css
* white.cs

### Custom Themes

It’s quite easy to create a custom theme. Today, I’ll be using my custom theme
from a presentation I gave called [“How To Build Kick-Ass Website: An
Introduction To Front-end
Development.”](https://ejbostian.github.io/how-to-become-a-web-developer/)

Here is what my custom slides look like:

![](https://cdn-images-1.medium.com/max/2000/1*ihTBdnMw9G83aD1hj45__w.png)

#### **Creating A Custom Theme**

1.  Open `css/theme/src` inside your IDE. This holds all of the Sass files (.scss)
for each theme. These files will be transpiled to CSS using
[Grunt](https://gruntjs.com/) (a JavaScript task runner). If you prefer to write
CSS, go ahead and just create the CSS file inside `css/theme`.
1.  Create a new `.scss` file. I will call mine `custom.scss`. You may have to stop
your localhost and run `npm run build` to transpile your Sass code to CSS.
1.  Inside the `index.html` file, change the CSS theme import in the `<head>` tag to
use the name of the newly created stylesheet. The extension will be `.css`, not
`.scss`.
1.  Next, I created variables for all of the different styles I wanted to use. You
can find custom fonts on [Google Fonts](https://fonts.google.com/). Once the
font is downloaded, be sure to add the font URL’s into the `index.html` file.

Here are the variables I chose to use:

* **Title Font: **[Viga](https://fonts.google.com/specimen/Viga)
* **Content Font:** [Open Sans](https://fonts.google.com/specimen/Open+Sans)
* **Code Font:** [Courier New](https://fonts.google.com/?query=Courier+New)
* **Cursive Font:** [Great Vibes](https://fonts.google.com/specimen/Great+Vibes)
* **Yellow Color:** #F9DC24

5. Add a `.reveal` class to the custom Sass file. This will wrap all of the
styles to ensure our custom theme overrides any defaults. Then, add your custom
styling!

*Unfortunately, due to time constraints, I’ll admit that I used quite a bit of
*`!important`* overrides in my CSS. This is horrible practice and I don’t
recommend it. The reveal.css file has extremely specific CSS styles, so I should
have, if I had more time, gone back and ensured my class names were more
*[specific](https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity)* so I
could remove the *`!importants`*.*

#### Mixins & Settings

Reveal.js also comes with mixins and settings you can leverage in your custom
theme.

To use the mixins and settings, just import the files into your custom theme:

    @import "../template/mixins";

    @import "../template/settings";

**Mixins**

You can use the vertical-gradient, horizontal-gradient, or radial-gradient
mixins to create a neat visual effect.

All you have to do is pass in the required parameters (color value) and voila,
you’ve got a gradient!

**Settings**In the settings file, you’ll find useful variables like heading
sizes, default fonts and colors, and more!

![](https://cdn-images-1.medium.com/max/2000/1*lK72ePLIQbehCt0BLgidTg.png)

### Elements

The structure for adding new content is:

    .reveal > .slides > section

The `<section>` element represents one slide. Add as many sections as you need
for your content.

#### **Vertical Slides**

To create vertical slides, simply nest sections.

### Transitions

There are several different slide transitions for you to choose from:

* None
* Fade
* Slide
* Convex
* Concave
* Zoom

To use them, add a `data-transition="{name}"` to the `<section>` which contains
your slide data.

### Fragments

Fragments are great for highlighting specific pieces of information on your
slide. [Here](https://revealjs.com/#/fragments) is an example.

To use fragments, add a `class="fragment {type-of-fragment}"` to your element.

The types of fragments can be:

* grow
* shrink
* fade-out
* fade-up
* fade-in-then-out
* fade-in-then-semi-out
* highlight-current-blue
* highlight-red
* highlight-green
* highlight-blue

You can additionally add indeces to your elements to indicate in which order
they should be highlighted or displayed. You can denote this using
the`data-fragment-index={index}` attribute.

*****

There are way more features to reveal.js which you can leverage to build a
beautiful presentation, but these are the main things which got me started.

To learn more about how to format your slides, check out the [reveal.js
tutorial](https://revealjs.com/#/10).

All of the code for my presentation can be viewed on
[GitHub](https://github.com/ejbostian/how-to-become-a-web-developer). Feel free
to steal my theme!

### [Emma Wedekind](https://levelup.gitconnected.com/@emmawedekind)

Software Engineer @ LogMeIn by day, cat Mom by night. Also a full-time
Bibliophile. I enjoy all things Front-end & Design

### [gitconnected.com | Level Up Your
Coding](https://levelup.gitconnected.com/?source=footer_card)

Our community publishes stories about software development, design, data
science, and blockchain. gitconnected - The Developer Homepage
[https://gitconnected.com](https://gitconnected.com/)


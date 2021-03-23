
#### The website can be found [here](https://static-website-with-animation.herokuapp.com/).
# Static Website with Animate.css

## Table of Contents

* [Introduction](#introduction)
* [Animate.css](#animatecss)
* [Wow.Js](#wowjs)

## Introduction
Static Websites are undoubtedly the dominant kind of websites. They contain web pages with fixed contents that are displayed to each user in the same way.

Each webpage is coded in [HTML](https://www.w3schools.com/html/default.asp) and then [CSS](https://www.w3schools.com/css/css_intro.asp) specifies how each HTML elements should appear on a screen.

Following advantages of static websites are described on [Wikipedia](https://en.wikipedia.org/wiki/Static_web_page):
* Provide improved security over dynamic websites (dynamic websites are at risk to web shell attacks if a vulnerability is present).
* Improved performance for end users compared to dynamic websites.
* Fewer or no dependencies on systems such as databases or other application servers. 
* Cost savings from utilizing cloud storage, as opposed to a hosted environment.
* Security configurations are easy to setup, which makes it more secure.


## Animate.css

CSS allows animation of HTML elements without using JavaScript or Flash! You must be thiking, why would we use animations in a static website? Because they are **COOL** and also can improve the UX of an interface.

One great way to add animation to any static website is with the help of [*animate.css*](https://animate.style/). It is a library of cross-browser animations that you can use in your web projects.
 
### Getting Started
There are two simple methods for getting started with animate.css.

* #### Download the Library
    In the **Resources** folder of this repository, there is a file present with the name of animate.css. Download that file to your project and link it to your HTML file by using the following syntax:
    `<link href="animate.css" type="text/css" rel="stylesheet">`

* #### Installing with npm
    In your Terminal or Command Prompt, type the command `npm install animate.css --save` to install the required dependecies for using animate.css. 

That's it! You are ready to animate your HTML elements. 

### Animating the HTML Element

When using animate.css, you must use a specific syntax.

1. Select the type of animation to apply to the element. There are many different kinds of animation to choose from. To test the animations, go to the [animate.style](https://animate.style/) website.
2. Add a `class` tag to the element you want to animate.
3. Set the `class` tag to the name of the animation you want to use, and prefix it with the word **animate**. 

After you've completed all of the steps, the element should look like: `<h3 class="animate fadeInUp">Animated Element</h3>`

#### **BUT**

## Wow.Js

After adding the animations to all the HTML elements you might notice that the animation on the lower end of the web page do not work. Why is that?
It is because when you load a web page, all of the animations start playing at the same time, regardless of where they are on the screen. As a result, if an element is at the bottom of the page, its animation will be completed before you reach it.

So, how can you ensure that the animation only plays when it is visible on the screen? Here comes in [Wow.js](https://wowjs.uk/).

The Animate CSS library provides a complete set of CSS3 animations you can apply to any HTML element and WOW is a Javascript library which provides more control over those animations. Using the wow.js library with the Animate CSS library, the CSS animations of the HTML elements will start when those elements become visible as you scroll down the page.

#### Initializing Wow.Js
It is a three step process to make Wow.js work. 
1. Link to animate.css
2. Add the following code to the bottom of the page, inside the `body` tag:

```
<script src="Resources/wow.min.js"></script>
        <script>
            new WOW().init();
		</script>
```

3. Replace the **animate** word inside the HTML tag with **wow**. 

The element now becomes: `<h3 class="wow fadeInUp">Animated Element</h3>`

## Conclusion

These are some easy ways to spice up your static website and entice your users. Simply let your imagination run wild and see what you can come up with.
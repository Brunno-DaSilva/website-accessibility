![](/ga_cog.png)

---
Title: Website Accessibility <br>
Type: Warm Up Exercise<br>
Duration: "0:45"<br>
Created by: [Bruno DaSilva](https://github.com/Brunno-DaSilva) Course: SEIR<br>
Competencies: HTML & CSS <br>
Prerequisites:  HTML & CSS <br>

---
# Warm Up Exercise


## Accessability for the Web

When we refer to a web site as being accessible, we mean that this site is available to anyone. Web site accessability, refers to the ability of an user to interact with the web site differently from the narrow range of the "typical" user scenario, specially users with some type of impairment or disability. A site is accessible when people can perceive, understand, navigate, and interact with it.

W3.org has a [Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/TR/WCAG20/) that goes in-depth through a wide range of recommendations for making web content more accessible. This accessability guidelines ensure that users with visual, auditory, physical, speech, cognitive, language, learning, and neurological disabilities can interact with the Web site just like any other user. 


WCAG is organized around four principles often called by the acronym **POUR**:

* **Perceivable**: Can users perceive the content? This helps us keep in mind that just because something is perceivable with one sense, such as sight, that doesn't mean that all users can perceive it.

* **Operable**: Can users use UI components and navigate the content? For example, something that requires a hover interaction cannot be operated by someone who can't use a mouse or touch screen.

* **Understandable**: Can users understand the content? Can users understand the interface and is it consistent enough to avoid confusion?

* **Robust**: Can the content be consumed by a wide variety of user agents (browsers)? Does it work with assistive technology?


Why Accessibility? Because it supports social inclusion for people with disabilities as well as others, such as:

* Older people
* People in rural areas
* People in developing countries


There is also a strong business case for accessibility. As accessability improves overall user experience and satisfaction across multiple devices.  

**Also in many cases Web accessibility is required by law.**


[W3C](https://www.w3.org/WAI/videos/standards-and-benefits/) provides a great introductory video [Introduction to Web Accessibility and W3C Standards](https://www.youtube.com/watch?v=20SHvU2PKsM)


## Tools and Methods to browse the Web

* Screen readers (ex. ChromeVox) 
* Keyboard board, 
* Head wand and/or Mouthstick
* Magnification 
* Single switch 

These are some tool and methods users utilize to browse the web and interact with a website. 


## Semantic HTML 

Semantic HTML refers to the use of element tags with a clear meaning to the developer and browser. Some examples of semantic tags are `<form>`, `<aside>`, `<article>`, `<button>`.

Non-Semantic HTML elements, as you might have imagine, are tags that does not co-relate a meaning, like `<div>`, `<span>`


| Tag             | Description                                 |
| --------------- | ------------------------------------------- |
| `<article>`     | Defines independent, self-contained content |
| `<details>`     | Defines content aside from the page content |
| `<figcaption>`  | Defines a caption for a `<figure>` element  |
| `<figure>`      | Specifies self-contained content, like illustrations, photos, etc.|
| `<footer>`      | Defines a footer for a document or section  |

[More on Semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)


#### Anti Patterns

* `<div class="button" >Not a Button</div>`
* `<span class="checkbox"></span>`
* `<img src="./img/tacocat.png"/>`

#### Semantic Patterns

* `<button class="button" >A Button</button>`
* `<input type="checkbox" id="vehicle1" name="vehicle1" value="Bike"> <label for="vehicle1"> I have a bike</label><br>`
* `<img src="./img/tacocat.png" alt="A junction of a cat and a taco"/>`

##### Note about alt text and Screen readers

* An empty `alt=""` will be skipped by screen readers
* `alt="UPPERCASE"` screen reader will individually read letters.  


#### Hide elements

From Screen Readers: 
* `display: none`
* `visibility: hidden`
* `input hidden />` 

From users: 

* Approach used by Twitter

```
.screenreader{
    position: absolute; 
    left: -10000px;
    width: 1px; 
    height: 1px; 
    overflow: hidden; 
}

```


## Hungry For More? 

Here you have extra readings with real world example of what accessability is all about and how you can implement it in your projects going forward. 

* [Google](https://developers.google.com/web/fundamentals/accessibility)
* [Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/TR/WCAG20/)
* [W3C accessability Fundamentals](https://www.w3.org/WAI/fundamentals/)
* [Skip Links](https://webaim.org/techniques/skipnav/)
# QuizMechanics

How to build an educational quiz.

## Quiz question types

* Pick all the red squares
* Pick the cow
* Pick the smallest cow
* Pick the animal that make this sound
* Pick the blue circle
* ?

## Quiz types

Identify:

* Shapes
* Animals
* Vehicle
* ?

What noise, which size etc. Any thing else?

It would be great if we can do this in Xhosa, Zulu and other ZA languages

## Quiz components:

This is a quick brain dump of the things one need to be able to do the create a quiz

* Setting up the questionairre
* Play instructional audio
* Rendering questions
* Checking question answers
* Keep track of answers questioned
* Resume a quiz
* Store quiz results
* Select next quiz
* Player profile screen
* Multi language support
* ?

## Skills required

* DOM manipulation
* CSS layout
* Client side event handling form events
* Template rendering
* Display images
* JSON basics - stringify/parse
* Play audio in the browser
* ?

## Tools and Technology

### User Interface (buttons and boxes)

Use [Twitter's Bootstrap Framework](http://getbootstrap.com/) for basic styling and User Interface interactions. It's not always the best choice, but we want to get the interface together quickly, with minimal fuss, to be polished later.

* What it is: HTML, CSS, and JavaScript framework.
* How to use it: add `link` and `script` to your HTML page, then follow their HTML patterns in [CSS](http://getbootstrap.com/css/) (Grid, Forms, Buttons), [Components](http://getbootstrap.com/components/) (Glyphicons, Dropdowns, Navigation), and [JavaScript](http://getbootstrap.com/javascript/) (Tabs, Alerts, Collapse) to get fancy styling and behaviour.
* Pros and Cons: Fast, easy, but heavy and someone else's solution.
* Activity: build a start page using the grid. Change the layout over different screen sizes.
* Activity: add a navigation bar at the top. Add some icons to some of the items.
* Activity: add a log in form.

### User Experience

It's important to think about the User Experience of your application: **does it meet the needs of user**, as simply and quickly as possible?

For our quizzes, that means thinking about the **layout of the page**, and **which HTML element** we use for each piece.

### Icons and Images

If you want to use icons in your interface, have a look at Bootstrap's [Glyphicons](http://getbootstrap.com/components/#glyphicons). Make sure that you always have text next to an icon: don't use an icon on its own, as the meaning might not be clear to your users.

For other images, do a web search. To find ones that you are allowed to use, look at **Search Tools**, **Usage Rights**, and choose a license. If you want to use icons instead of photos, have a look at [Flaticon](http://www.flaticon.com/).

### jQuery

Bootstrap requires [jQuery](https://jquery.com/) (a JavaScript library that provides a simpler way of doing things). Have a look at [their base template](http://getbootstrap.com/getting-started/#template) for how to get started.

Use jQuery for things like [DOM manipulation](http://api.jquery.com/category/manipulation/), [event handling](http://api.jquery.com/category/events/), [forms](http://api.jquery.com/category/forms/), [Ajax](http://api.jquery.com/category/ajax/). It's not always the right choice, but since you're including it for Bootstrap, it makes sense to use here.

* Pros and Cons: (see bits in Field Guide [Field Guide](https://github.com/SteveBarnett/Front-end-Field-Guide/blob/gh-pages/technology-and-tools.md#frameworks))
* usage: add `script` to your HTML page.
* Activity: refactor something you've already done to use jQuery instead of regular JavaScript. Pick something with `addClass` and `addEventListener`.
* Activity: form handling on submit
* Chat: ajax. What it is. We won't use it for this (because PouchDB), but very important and popular.

### Handlebars

Use [Handlebars](http://handlebarsjs.com/) for templating. It's a popular, powerful, templating language that we'll be using a lot.

* Variables. E.g. `{{name}}` or `{{author.name}}`.
* Loops. E.g. `  {{#each items}} ... {{/each}}`.
* Partials. E.g. `{{> userMessage }}` or `{{> userMessage tagName="h1" }}`.

## PouchDB

Use [PouchDB](http://pouchdb.com/) to store the data. It stores the data in the user's browser (and can sync to a remote database, which we might look at later).

* What is is: open-source JavaScript database.
* Stores in browser.
* Syncing (but we probably won't use that bit).
* Activity: CRUD, [To Do list](http://pouchdb.com/getting-started.html).

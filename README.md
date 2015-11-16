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

## Tools

* Use [Flaticon](http://www.flaticon.com/) (or another source of your choice) to add icons. Icons should always have text next to them.
* Use [Twitter's Bootstrap Framework](http://getbootstrap.com/) for basic styling and User Interface interactions. It's not always the right choice, but we want to get the interface together quickly, with minimal fuss, to be polished later.
  * Bootstrap requires [jQuery](https://jquery.com/) (a JavaScript library that provides a simpler way of doing things). Have a look at [their base template](http://getbootstrap.com/getting-started/#template) for how to get started.
* Use jQuery for things like [DOM manipulation](http://api.jquery.com/category/manipulation/), [event handling](http://api.jquery.com/category/events/), [forms](http://api.jquery.com/category/forms/), [Ajax](http://api.jquery.com/category/ajax/). It's not always the right choice, but since you're including it for Bootstrap, it makes sense to use here.
* Use [Handlebars](http://handlebarsjs.com/) for templating. It's a popular, powerful, templating language that we'll be using a lot.
* Use [PouchDB](http://pouchdb.com/) to store the data. It stores the data in the user's browser (and can sync to a remote database, which we might look at later).

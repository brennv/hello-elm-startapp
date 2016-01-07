# Hello Elm StartApp

Getting started with Elm is now easier than ever with the [StartApp][start-app] package.

## Getting started

Make sure you have [elm][elm-install] installed. 

Clone this repo.

```git clone https://github.com/brennan-v-/hello-elm-startapp.git```

>You need two files in a fresh directory:
>
* **HelloElmStartApp.elm**, from the start-app README
* **elm-package.json**, so elm knows what packages to install

Step into your new directory and make your app:

```elm-make HelloElmStartApp.elm```

Elm will start installing the necessary components with your approval. 

```
Some new packages are needed. Here is the upgrade plan.

  Install:
    elm-lang/core 3.0.0
    evancz/elm-effects 2.0.1
    evancz/elm-html 4.0.2
    evancz/start-app 2.0.2
    evancz/virtual-dom 2.1.0

Do you approve of this plan? (y/n) y
Downloading elm-lang/core
Downloading evancz/elm-effects
Downloading evancz/elm-html
Downloading evancz/start-app
Downloading evancz/virtual-dom
Packages configured successfully!
Success! Compiled 40 modules.                                       
Successfully generated index.html
```

Done!

Grab your browser and open your new **index.html** file :)

[arch]: https://github.com/evancz/elm-architecture-tutorial/
[elm-html]: http://elm-lang.org/blog/Blazing-Fast-Html.elm
[start-app]: http://package.elm-lang.org/packages/evancz/start-app/2.0.2/
[elm-install]: http://elm-lang.org/install

## Further Learning

For more guidelines and examples of making apps in Elm, check out the following resources:

  * [Language Docs](http://elm-lang.org/docs) &mdash; tons of learning resources that go from syntax to language features to design guidelines.
  * [The Elm Architecture][arch] &mdash; simple examples demonstrating how our basic counter app can scale to huge applications that are easy to test, maintain, and refactor.
  * [elm-todomvc][] &mdash; a typical TodoMVC program ([live][]) built on the Elm Architecture. You will see the `model`, `update`, `view` pattern but for a more realistic application than a counter.
  * [dreamwriter][] &mdash; a writing app built in Elm that again uses the Elm Architecture. The creator has *never* had a runtime exception in his Elm code. Unlike JavaScript, Elm is designed for reliability that scales to any size.

[elm-todomvc]: https://github.com/evancz/elm-todomvc/blob/master/Todo.elm
[live]: http://evancz.github.io/elm-todomvc/
[dreamwriter]: https://github.com/rtfeldman/dreamwriter/

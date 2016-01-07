# Elm StartApp example

Getting started with [Elm][elm-lang] is now easier than ever with the Elm [StartApp][start-app] package. This repo is an excerpt from the StartApp readme example and contains the minimal code needed to create a simple counter with Elm using StartApp.

## Getting started

Make sure you have [Elm installed][elm-install]. 

Clone this repo...

```git clone https://github.com/brennan-v-/hello-elm-startapp.git```

...or grab the code from the [StartApp][start-app] readme, and include the following in a new **elm-package.json** file:

>```
{
    "version": "1.0.0",
    "summary": "",
    "repository": "",
    "license": "BSD3",
    "source-directories": [
        "."
    ],
    "exposed-modules": [],
    "dependencies": {
        "elm-lang/core": "3.0.0 <= v < 4.0.0",
        "evancz/elm-html": "4.0.2 <= v < 5.0.0",
        "evancz/start-app": "1.0.0 <= v < 3.0.0"
    },
    "elm-version": "0.16.0 <= v < 0.17.0"
}
```

## Running elm-make
Step into your new directory and make your app by running elm-make.

```elm-make HelloElmStartApp.elm```

Elm will install the necessary components with your approval. 


>```
Some new packages are needed. Here is the upgrade plan.
>
  Install:
    elm-lang/core 3.0.0
    evancz/elm-effects 2.0.1
    evancz/elm-html 4.0.2
    evancz/start-app 2.0.2
    evancz/virtual-dom 2.1.0
>
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

And you're done! 

Grab your browser and open the new **index.html** file :)

[arch]: https://github.com/evancz/elm-architecture-tutorial/
[elm-html]: http://elm-lang.org/blog/Blazing-Fast-Html.elm
[start-app]: http://package.elm-lang.org/packages/evancz/start-app/2.0.2/
[elm-install]: http://elm-lang.org/install
[elm-lang]: http://elm-lang.org/

## Further Learning

For more guidelines and examples of making apps in Elm, check out the following resources:

  * [Language Docs](http://elm-lang.org/docs) &mdash; tons of learning resources that go from syntax to language features to design guidelines.
  * [The Elm Architecture][arch] &mdash; simple examples demonstrating how our basic counter app can scale to huge applications that are easy to test, maintain, and refactor.
  * [elm-todomvc][] &mdash; a typical TodoMVC program ([live][]) built on the Elm Architecture. You will see the `model`, `update`, `view` pattern but for a more realistic application than a counter.
  * [dreamwriter][] &mdash; a writing app built in Elm that again uses the Elm Architecture. The creator has *never* had a runtime exception in his Elm code. Unlike JavaScript, Elm is designed for reliability that scales to any size.

[elm-todomvc]: https://github.com/evancz/elm-todomvc/blob/master/Todo.elm
[live]: http://evancz.github.io/elm-todomvc/
[dreamwriter]: https://github.com/rtfeldman/dreamwriter/

## Credit

Elm, StartApp, the start-app example and portions of this readme were created by [@evancz](https://github.com/evancz).

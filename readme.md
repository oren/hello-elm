# Hello World in Elm

The simplest website written in Elm

## Run
```
npm install -g elm
elm package install evancz/elm-html
elm make hello.elm --warn --output index.html
```

Notice a new file called index.html. Open it with your browser. You should see 'Hello, World!'.


## Explanation of every line

```elm
import Html exposing (text)
```
The line above take the text function from the Html module

Where to find the Html module?
* online documentation: http://package.elm-lang.org and search for elm-html
* in your project's folder: elm-stuff/packages/evancz/elm-html

```elm
main : Html.Html
```
This line is called Type Annotation in Elm. It tells the Elm compailer what type is the main variable.
In this case the main variable is of type Html.Html.

```elm
main =
  text "Hello, World!"
```
TBD

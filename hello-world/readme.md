# Hello World in Elm

The simplest website written in Elm

## Install Elm
```bash
npm install -g elm
```

## Create the website

**Create hello.elm**

``` elm
import Html exposing (text)

main : Html.Html
main =
  text "Hello, World!"
```

**Install the Html package**
```
elm package install evancz/elm-html
```

**Compile hello.elm into index.html**
```
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
This line is called Type Annotation in Elm. It tells the Elm compiler what type is the main variable. In this case the main variable is of type [Html.Html](http://package.elm-lang.org/packages/evancz/elm-html/4.0.2/Html#Html). The reason for that is that the [text](http://package.elm-lang.org/packages/evancz/elm-html/4.0.2/Html#text) function returns Html.

```elm
main =
  text "Hello, World!"
```
This is simple assignment - the return value of the `text` function is assigned to the `main` variable.
Notice that it could have been written in a single line but the convention in Elm is to start the body of a function in a new line.

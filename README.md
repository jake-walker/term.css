# term.css
A super simple CSS framework made to look terminal-like.

> Please note this project is not complete. Not every single HTML element is added so request one by creating an issue.

## Getting Started
You can use term.css by including it at the top of the page:
```
<link rel="stylesheet" href="https://raw.githubusercontent.com/jake-walker/term.css/master/term.css">
```
or you can use the [starter template](https://github.com/jake-walker/term.css/blob/master/template.html).

## Elements
*This list might not be up to date but I'll try to update it.*

### Typography
#### Elements
* `<p>` - Default text
* `<b>` - Emphasised Green text to stand out
* `<h1>` (1 to 6) - Headings
* `<a>` - Links
* `<code>` - Code
#### Classes
* `.emph` - Slightly emphasised text. White instead of normal text which is grey
* `.un-emph` - Makes text grey instead of white. Useful for parts of headings.

### Section
A section is used for seperating main parts of content. They should be used with the `.container` class (see below).
```
<section class="container">
  <h1>Welcome</h1>
  <p>Hi</p>
</section>
<section class="container">
  <h1>About Me</h1>
  <p>I have a cat named Mellow</p>
</section>
```

### Navigation
```
<div class="container">
  <p class="emph inline">Site Name</p>
  <div class="pull-xs-right inline">
    <p class="inline nav-link"><a class="active nav-link" href="">Home</a></p>
    <p class="inline nav-link"><a class="nav-link" href="http://example.com">Another link</a></p>
  </div>
</div>
```

Copy the above example and move the `.active` class to whichever link should be diplayed as active.

### Container, Grid and Push
*Based on Bootstrap*
#### Container
A container helps to keep your content in the center of the screen away from edges.
```
<div class="container">
  Your HTML here...
</div>
```
#### Grid
```
<div class="row">
  <div class="col-md-6">
    Half row
  </div>
  <div class="col-md-6">
    Half row
  </div>
</div>
```

Syntax:
  `col-`
  `xs` - Portrait Phones, `sm` - Landscape Phones, `md` - Tablets, `lg` - Computers, `xl` - Massive Screens
  `-`
  A whole width of a screen is 12. For 2 columns it would be 6 (6+6=12). `1` to `12`

Read more [here](http://v4-alpha.getbootstrap.com/layout/grid/).

#### Pull
The pull class is used to float elements on the left, right or center of the screen.

```
<p class="pull-xs-right">I'm on the right</p>
```

Similar to the grid. `xs` - Portrait Phones, `sm` - Landscape Phones, `md` - Tablets, `lg` - Computers, `xl` - Massive Screens

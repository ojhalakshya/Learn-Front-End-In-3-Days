# CSS in 1 Day

#### CSS reference sources:
1. https://www.w3schools.com/cssref/css_selectors.asp
2. https://css-tricks.com/almanac/

Basic CSS syntax type:

```css
Selector
{
  Property: value;
}
```
Example
```css
h2
{
  color: red;
}
```

#### Cascading

* If same selector is defined more then once then the latest one is considered.

```css
p
{
  color: pink;
}

p
{
  color: green;
}
```
* The final color for the paragraph will be *green*.

> In chrome the style.css or more specifically style for any section of the webpage can be edited from the browser itself.

#### Adding style.css to html

#### 1st way
```html
<link rel = "stylesheet" type = "text/css" href = "style.css">
```
#### 2nd way
```html
<header style = "background-color: green; color: yellow;">
```
* This will apply these style to everything, unless somethings are personally overrided like links will have different color then yellow.

#### 3rd way
```html
<head>
  <title>Home</title>
  <style>
    li
    {
      background-color: yellow;
    }
  </style>
</head>
```
* This can be used directly inside the html file, no seperate css file is needed for this.
* But for huge websites this can mess up the code.

#### Sample css selector
```css
li
{
  color: red;
  background-color: white;
  list-style: none;
  display: inline-block;
}
```

#### CSS referances

1. Use [css-tricks](https://css-tricks.com/almanac/) to referance any selector/property knowledge.
2. Use [paltton](http://paletton.com/) to choose colors for anything, it gives a good color comparison and contrasts for any color.

### Selectors

* Selector referance: [w3schools](https://www.w3schools.com/cssref/css_selectors.asp).

* Some basic selectors:
```
.class
#id
element
element, element
element element
element > element
element + element
:hover
:last-child
:first-child
!important (not recommended)
```

#### Class

* Enables you to create a class, make some elements/things in html file to this class and then edit the class properties.

```css
.class
```

* The 1st lorem ipsum will inherit properties from 2 classes -> **webtext** and **active**.
```css
    <p class = "webtext active">Lorem Ipsum.</p>
    <p class = "webtext">Lorem Ipsum.</p>
    <p class = "webtext">Lorem Ipsum.</p>
    <p class = "webtext">Lorem Ipsum.</p>
```

* There can be any number of classes and elements can inherit properties from any number of classes.

#### ID

```css
#div1
{
  background: yellow;
}
```
* An element or group of elements can have **only 1** id. Here `div1` is the id.

* We use division tag to use id for a division in the webpage.

```html
  <div id = "div1">
    <p class = "webtext active">Lorem Ipsum.</p>
    <p class = "webtext">Lorem Ipsum.</p>
    <p class = "webtext">Lorem Ipsum.</p>
    <p class = "webtext">Lorem Ipsum.</p>
  </div>
```
> **NOTE:**
>
> rgba(0, 0, 255, 0.2) -> (r, g, b, opacity)
>
> opacity = 0.2

#### * select all elements
* Selects all elements and applies the given properties to all the elements in the whole webpage.
```css
*
{
  text-align: center;
}
```

#### Important
* Specificity: CSS file is read from top to bottom, so even if in **select all elements '*'** the `align = right`, but if later on it is change by lets say *p, body or h2 etc* then the first align is over-rided.
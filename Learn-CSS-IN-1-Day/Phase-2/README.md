#### Continuing Selectors

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

#### Elements
* h2 and p are elements which come from the tag used in HTML.

```
h2
p
```

* Elements can also be used to define properties of something which are under both the elements.

#### element, element
```
h1, p
```
* Select all `<h1>` elements and `<p>` elements and apply properties provided inside the style.

#### element element
```
h2 p
```
* Select all `<p>` elements inside `<h2>` elements.

#### element > element
```
h2 > p
```
* Select all `<p>` elements whose immediate parent is `<h2>`.

#### :hover
```html
.hoverClass:hover
```
* Select the element when you hover over it.
#### Continuing Selectors

### Selectors

* Selector referance: [w3schools](https://www.w3schools.com/cssref/css_selectors.asp).

* Some basic selectors:
```html
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

```html
h2
p
```

* Elements can also be used to define properties of something which are under both the elements.

#### element, element
```html
h1, p
```
* Select all `<h1>` elements and `<p>` elements and apply properties provided inside the style.

#### element element
```html
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

#### !important
```html
p
{
  text-align: center !important;
}
```
* This will override any following cascading being applied to the `<p>` tag.
* This selector is **NOT RECOMMENDED** because it may confuse fellow coders who are now working on your code base.

What seletors win out in the cascade depends on:
1. Specificity -> [Specificity Calculator](https://specificity.keegan.st/)
   * In line styles always win in specificity.
2. Importance
   * !important selector
3. Source Order

> **NOTE**: If there are multiple sylesheets included in the HTML then they are read in order of top to down and are cascaded.
> Like shown below, `syle2.css` will override any common features from `style1.css`
```html
  <link rel = "stylesheet" type = "text/css" href = "style.css">
  <link rel = "stylesheet" type = "text/css" href = "style2.css">
```

#### clear
```html
/* both -> clear both left, right floating */
clear: both;
```
* Used to clear any floating property from before for the current selected elements.

#### display:
```html
display: inline-block;
```
* Used to display the selected elements according to the choosed property.
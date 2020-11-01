# Advanced HTML

## Forms

Use this [reference](https://www.w3schools.com/html/html_forms.asp) for `form tag` and its properties.
```html
  <!-- This is forms tag, it has its own tags and different attributes -->
  <!-- It also has request type as attribute, by default the form information is sent in 'GET' request -->
  <!-- But you can use 'method' keyword in forms to change it to any other like 'POST' -->
  <form>
    First Name:<input type = "text" name = "firstname"><br>
    Last Name: <input type = "text" name = "lastname"><br>

    Gender: <br>
    <!-- Here the information is stored in 'name' and 'value' i.e -->
    <!-- the information has name = "gender" and for this tag the value = "Male/Female/Other" -->
    <input type = "radio" name = "gender" value = "Male">Male<br>
    <input type = "radio" name = "gender" value = "Female">Female<br>
    <input type = "radio" name = "gender" value = "Other">Other<br>

    Pets: <br>
    <input type = "checkbox" name = "cat" value = "cat">Cat<br>
    <input type = "checkbox" name = "Dog" value = "Dog">Dog<br>
    <input type = "checkbox" name = "Other" value = "Other">Other<br>

    Email: <input type = "email" required name = "email"><br>
    Password: <input type = "password" minlength="5" name = "password"><br>

    Birthday: <input type = "date" name = "birthday"><br>

    Cars: <br>
    <select name = "Cars">
      <option value = "Volvo" name = "Volvo">Volvo</option>
      <option value = "BMW" name = "BMW">BMW</option>
    </select><br>

    <!-- Automatically creates the submit button -->
    <input type = "submit" value = "Register">
    <input type = "reset">
  </form>
  ```
* Forms tag have their own attribute tags and different features.
* Reset button will reset all filled details from any tag inside the forms tag.

* **Form automatically uses 'GET' method to send the information throught the url like this.**
```
firstname=Lakshya&lastname=Ojha&gender=Male&cat=cat&Other=Other&email=ojhalakshya%40gmail.com&password=fbsdggbhhfg&birthday=2020-10-30&Cars=BMW
```

So this would show all the information through the url link.

To change this you can use 'POST' method in which all the information is sent through body of the url not the url itself.

```html
<form method = "POST">
```

### Forms tag can have its own underlining tags

1. Fill Box
    * ```html
      <input type = "text" name = "firstname">
      ```
    * This will create a fill box where user can enter information of type 'text' here. Ex like this.
    * <input type = "text" name = "firstname">
    * ```html
      <input type = "radio" name = "gender" value = "Male">
      ```
      Here the information is having name = 'gender' and the value = 'Male'.
2. Drop Down List / Select Tag
    * ```html
          <select name = "Cars">
          <option value = "Volvo" name = "Volvo">Volvo</option>
          <option value = "BMW" name = "BMW">BMW</option>
          </select><br>
      ```
    * This creates a drop down list in which you can have option from which the user can choose from.
    * The drop down list can also be made multiple select.
3. Division Tag
    * ```html
      <div></div>
      ```
    * It is used to create division between different portions of the webpage.
    * It helps greatly when we are later using css with the html.
4. Span Tag
    * ```html
      <span></span>
      ```
    * This does the same work as the division tag just that it does it to individual elements of the webpage.
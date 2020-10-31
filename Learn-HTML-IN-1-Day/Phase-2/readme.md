# Advanced HTML

### Forms

Use this [reference](https://www.w3schools.com/html/html_forms.asp) for `form tag` and its properties.
```html
<form>
  First Name:<input type = "text"><br>
  Last Name: <input type = "text"><br>

  Gender: <br>
  <input type = "radio" name = "gender">Male<br>
  <input type = "radio" name = "gender">Female<br>
  <input type = "radio" name = "gender">Other<br>

  Pets: <br>
  <input type = "checkbox">Cat<br>
  <input type = "checkbox">Dog<br>
  <input type = "checkbox">Other<br>

  Email: <input type = "email" required><br>
  Password: <input type = "password" minlength="5"><br>

  Birthday: <input type = "date"><br>

  Cars: <br>
  <select>
    <option value = "Volvo">Volvo</option>
    <option value = "BMW">BMW</option>
  </select><br>

  <!-- Automatically creates the submit button -->
  <input type = "submit" value = "Register">
  <input type = "reset">
</form>
  ```
* Forms tag have their own attribute tags and different features.
* Reset button will reset all filled details from any tag inside the forms tag.

* **Form automatically uses get method to send the information throught the url like this.**
```
http://127.0.0.1:5500/Learn-HTML-IN-1-Day/Phase-2/src/register.html?firstname=Lakshya&lastname=Ojha&gender=Male&cat=cat&Other=Other&email=ojhalakshya%40gmail.com&password=fbsdggbhhfg&birthday=2020-10-30&Cars=BMW
```

So this would show all the information through the url link.
To change this you can use POST method in which all the information is sent through body of the url not the url itself.

```html
<form method = "POST">
```
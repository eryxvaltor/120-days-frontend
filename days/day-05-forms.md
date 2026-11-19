# Day 5: HTML Forms

## The form Element

`<form>` groups controls that collect and submit data.

|Attribute|Purpose|
|---|---|
|`action`|Destination the data is sent to|
|`method`|`GET` or `POST`|

```html
<form action="/login" method="post">
  ...
</form>
```

## Input Types

`<input>` creates different controls based on `type`.

|Type|Control|
|---|---|
|`text`|Single-line text|
|`email`|Email address|
|`password`|Masked text|
|`number`|Numeric value|
|`checkbox`|Independent on/off choice|
|`radio`|One choice from a group|

```html
<input type="text" name="username">
<input type="email" name="email">
<input type="password" name="password">
<input type="number" name="age">
```

## Labels

`<label for="email">` connects to `<input id="email">`, which improves accessibility.

```html
<label for="email">Email</label>
<input type="email" id="email" name="email">
```

## Common Attributes

|Attribute|Purpose|
|---|---|
|`id`|Uniquely identifies the element|
|`name`|Identifies the submitted data|
|`placeholder`|Hint shown inside the field|
|`required`|Enables validation, field cannot be empty|

```html
<input type="text" id="user" name="user" placeholder="Enter username" required>
```

## Textarea

`<textarea>` allows multiline text input.

```html
<textarea name="message" rows="4" cols="30"></textarea>
```

## Select and Option

`<select>` contains `<option>` choices. The option **text is displayed**, while the **value is submitted**.

```html
<select name="course">
  <option value="html">HTML Basics</option>
  <option value="css">CSS Basics</option>
</select>
```

## Checkboxes and Radio Buttons

|Control|Behavior|
|---|---|
|Checkbox|Independent choices, any number can be selected|
|Radio|Buttons sharing the same `name` allow one selection per group|

```html
<input type="checkbox" id="html" name="skills" value="html">
<label for="html">HTML</label>

<input type="radio" id="beginner" name="level" value="beginner">
<label for="beginner">Beginner</label>
<input type="radio" id="advanced" name="level" value="advanced">
<label for="advanced">Advanced</label>
```

## Fieldset and Legend

`<fieldset>` groups related controls and `<legend>` labels the group.

```html
<fieldset>
  <legend>Experience Level</legend>
  <input type="radio" id="beginner" name="level" value="beginner">
  <label for="beginner">Beginner</label>
</fieldset>
```

## Submit Button

```html
<button type="submit">Submit</button>
```

## GET vs POST

|Method|Behavior|
|---|---|
|GET|Sends form values in the URL query string. Must not be used for passwords|
|POST|Sends values in the request body. Use over HTTPS for real credential submission|

## Validation

- Browser validation improves usability
- It does **not** replace server-side validation

## Styling

Use CSS for spacing and visual presentation, not repeated `<br>` elements.

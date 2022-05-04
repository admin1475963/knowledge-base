# Forms
For making forms, there is tag '_form_'.

Main attributes are '_action_' and '_method_'
The attribute '_action_' define handler of form (often it is relative link)
The attribute '_method_' define method of transfering data (usually, it is '_get_' or '_post_')
If form has file attachments, for sending it to server attribute '_method_' must be '_post_'. 
Also form must have attribute '_enctype_' with value '_multipart/form-data_'
Every form element have an attribute '_name_'
__Warning:__ All form elements must have different '_name_'.
Only '_radio_' is an exception.

```html
<form action="path/to/handler/link" method="post" enctpye='multipart/form-data'>
</form>
```

## Inputs
Inputs are inline elements.
All input tags have an attribute '_value_'. 
When we send the form, the attribute '_value_' is used as values of elements.

### Text
A simple text field. 
```html
<input type="text" name="username" value=""/>
```

### Password
Similar to a text field, but symbols will be hidden
```html
<input type="password" name="userpassword" value=""/>
```

### Tel
Similar to a text field, but in mobile devices when an user begin input, number keyboard will be opened
```html
<input type="tel" name="usertel" value=""/>
```
For '_text_', '_password_' and '_tel_' the attribute '_value_' is initial text in field.
So usually for these elements this attribute is empty.

### Radio
'_radio_' is used for creating radio buttons.
For grouping radio buttons, you must give them same name.
```html
<p><input type="radio" name="choice" value="option 1"/>option 1</p>
<p><input type="radio" name="choice" value="option 2"/>option 2</p>
```
For making some '_radion_' is checked by default, you must add '_checked_' attribute.
```html
<p><input type="radio" checked name="choice" value="option 1"/>option 1</p>
<p><input type="radio" name="choice" value="option 2"/>option 2</p>
```

### Checkbox
'_checkbox_' is used for creating checkboxes.
```html
<p><input type="checkbox" name="boolean" value="yes"/>Boolean question</p>
```
'_checkbox_' has also '_checked_' attribute.
```html
<p><input type="checkbox" checked name="boolean" value="yes"/>Boolean question</p>
```

### File
'_file_' is used for attaching file to form
```html
<input type="file" name="attachment"/>
```
You shouldn't give attribute 'value' to tag '_file_'

## Textarea
'_textare_' is field for multiline text.
```html
<textarea name="comment"></textarea>
```
You can control size of this field by attributes '_row_' and '_col_'.
But it is recommended to do this by __CSS__

## Select + option
These tags used for making popup list.
```html
<select name="colors">
    <option value="red">red</option>
    <option value="blue">blue</option>
    <option value="green">green</option>
</select>
```
'_select_' has attribute '_multiple_' which allows select multiple options.
In this case '_select_' is showed as simple list (not as popup list).
```html
<select multiple name="colors">
    <option value="red">red</option>
    <option value="blue">blue</option>
    <option value="green">green</option>
</select>
```
For option by default use '_selected_' attribute of '_option_'
```html
<select name="colors">
    <option value="red">red</option>
    <option selected value="blue">blue</option>
    <option value="green">green</option>
</select>
```
## Button
There are 3 types of button:
- '_submit_' - send the form to server.
- '_reset_' -  reset all fields to initial values.
- 'button' - do nothing. But you can attach client scripts to this button.
```html
<button type="submit">Send</button>
<button type="reset">Reset</button>
<button type="button">Simple button</button>
```

## Placeholder
Tags for text (e.g. '_text_', '_password_', '_textarea_') has an attribute '_placeholder_'.
This attribute can show hints in field when it is empty.
```html
<input type="text" name="username" placeholder="username" value=""/>
```

## Disabled
Disable element.
```html
<input type="text" disabled name="username" placeholder="username" value=""/>
```

## Tabindex
'_tabindex_' defines order of elements when user switches between them by key __Tab__
```html
<input tabindex="1" type="text" name="username" value=""/>
<input tabindex="2" type="password" name="userpassword" value=""/>
<input tabindex="3" type="tel" name="usertel" value=""/>
```
For grouped '_radio_' elements '_tabindex_' must be same.
# Forms

**HTML Form Controls**
There are different types of form controls that you can use to collect data using HTML form:

1. Text Input Controls
2. Checkboxes Controls
3. Radio Box Controls
4. Select Box Controls
5. File Select boxes
6. Hidden Controls
7. Clickable Buttons
8. Submit and Reset Button

**Syntax:**

< form action="server url" method="get|post">
  //input controls e.g. textfield, textarea, radiobutton, button
< /form> 

**Text Input Controls**

**There are three types of text input used on forms:**

- **Single-line text input controls**
  This control is used for items that require only one line of user input, such as search boxes or names. They are created using HTML `<input>` tag.

- **Password input controls**
  This is also a single-line text input but it masks the character as soon as a user enters it. They are also created using HTMl `<input>` tag.

- **Multi-line text input controls**
  This is used when the user is required to give details that may be longer than a single sentence. Multi-line input controls are created using HTML `<textarea>` tag.

  **Forms Attributes:**
  Following is the list of attributes for `<input>` tag for creating text field:

  | **Attribute** | **Description**                                                                                   |
  | ------------- | ------------------------------------------------------------------------------------------------- |
  | type          | Indicates the type of input control and for text input control it will be set to text             |
  | name          | Used to give a name to the control which is sent to the server to be recognized and get the value |
  | value         | This can be used to provide an initial value inside the control                                   |
  | size          | Allows to specify the width of the text-input control in terms of characters                      |
  | maxlength     | Allows to specify the maximum number of characters a user can enter into the text box             |

  **HTML Form Tags**

  | **Tag**     | **Description**                                           |
  | ----------- | --------------------------------------------------------- |
  | < form>     | It defines an HTML form to enter inputs by the used side  |
  | < input>    | It defines an input control                               |
  | < textarea> | It defines a multi-line input control                     |
  | < label>    | It defines a label for an input element                   |
  | < fieldset> | It groups the related element in a form                   |
  | < legend>   | It defines a caption for a < fieldset> element            |
  | < select>   | It defines a drop-down list                               |
  | < optgroup> | It defines a group of related options in a drop-down list |
  | < option>   | It defines an option in a drop-down list                  |
  | < button>   | It defines a clickable button                             |

**The list of HTML 5 form tags**

| **Tag**     | **Description**                                              |
| ----------- | ------------------------------------------------------------ |
| < datalist> | It specifies a list of pre-defined options for input control |
| < keygen>   | It defines a key-pair generator field for forms              |
| < output>   | It defines the result of a calculation                       |

- **HTML < input> element**
The HTML **< input>** element is fundamental form element. It is used to create form fields, to take input from user. We can apply different input filed to gather different information form user. Following is the example to show the simple text input.
Ex: 
< form>  
     Enter your name  < br>  
    < input type="text" name="username">  
  </ form>
 
 - **HTML TextField Control**
The type="text" attribute of input tag creates textfield control also known as single line textfield control. The name attribute is optional, but it is required for the server side component such as JSP, ASP, PHP etc.
ex: 
< form>  
    First Name: < input type="text" name="firstname"/> < br/>  
    Last Name:  < input type="text" name="lastname"/> < br/>  
 < /form> 

- **HTML < textarea> tag in form**
The < textarea> tag in HTML is used to insert multiple-line text in a form. The size of < textarea> can be specify either using "rows" or "cols" attribute or by CSS.
 ex:

   < form>  
        Enter your address:< br>  
      < textarea rows="2" cols="20">< /textarea>  
  < /form> 

 - **It is good to use < label> tag with form, although it is optional but if you will use it, then it will provide a focus when you tap or click on label tag. It is more worthy with touchscreens.**

 ex:
 < form>  
    < label for="firstname">First Name: < /label> < br/>  
              < input type="text" id="firstname" name="firstname"/> < br/>  
   < label for="lastname">Last Name: </ label>  
              < input type="text" id="lastname" name="lastname"/> < br/>  
 < /form> 
 - **HTML Password Field Control**

The password is not visible to the user in password field control.
ex:
< form>  
    < label for="password">Password: </ label>  
              < input type="password" id="password" name="password"/> < br/>  
< /form>  

- **HTML 5 Email Field Control**
The email field in new in HTML 5. It validates the text for correct email address. You must use @ and . in this field.
ex: 
< form>  
    < label for="email">Email: </ label>  
              < input type="email" id="email" name="email"/> < br/>  
< /form> 

- **Radio Button Control**
The radio button is used to select one option from multiple options. It is used for selection of gender, quiz questions etc. 
If you use one name for all the radio buttons, only one radio button can be selected at a time.
Using radio buttons for multiple options, you can only choose a single option at a time.
ex: 
< form>  
    < label for="gender">Gender: </ label>  
              < input type="radio" id="gender" name="gender" value="male"/>Male  
              < input type="radio" id="gender" name="gender" value="female"/>Female < br/>  
< /form> 

- **Checkbox Control**
The checkbox control is used to check multiple options from given checkboxes.
ex:
< form>  
Hobby:< br>  
              < input type="checkbox" id="cricket" name="cricket" value="cricket"/>  
                 < label for="cricket">Cricket </ label> < br>  
              < input type="checkbox" id="football" name="football" value="football"/>  
                 < label for="football">Football < /label> < br>  
              < input type="checkbox" id="hockey" name="hockey" value="hockey"/>  
                 < label for="hockey">Hockey </ label>  
< /form> 

- **Submit button control**
HTML < input type="submit"> are used to add a submit button on web page. When user clicks on submit button, then form get submit to the server.

**Syntax:**

< input type="submit" value="submit">  

Example:
< form>  




# JS EVENTS

***What is an Event ?***
JavaScript's interaction with HTML is handled through events that occur when the user or the browser manipulates a page.

When the page loads, it is called an event. When the user clicks a button, that click too is an event. Other examples include events like pressing any key, closing a window, resizing a window, etc.

In the case of the Web, events are fired inside the browser window, and tend to be attached to a specific item that resides in it — this might be a single element, set of elements, the HTML document loaded in the current tab, or the entire browser window. There are many different types of events that can occur. For example:

- The user selects a certain element or hovers the cursor over a certain element.
- The user chooses a key on the keyboard.
- The user resizes or closes the browser window.
- A web page finishes loading.
- A form is submitted.
- A video is played, paused, or finishes.
- An error occurs.


| **Event**   |                  **Description**                   |
| ----------- | :------------------------------------------------: |
|             |                                                    |
| onchange    |          An HTML element has been changed          |
| onclick     |          The user clicks an HTML element           |
| onmouseover |   The user moves the mouse over an HTML element    |
| onmouseout  | The user moves the mouse away from an HTML element |
| onkeydown   |           The user pushes a keyboard key           |
| onload      |     The browser has finished loading the page      |

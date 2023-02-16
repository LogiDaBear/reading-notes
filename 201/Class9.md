# Reading Notes for HTML Forms and JS Events

## HTML Forms
- [YourFirstForm](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form)
- [HowToStructureAWebForm](https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_structure_a_web_form)

1. Why are forms so important in web development?
They are one of the main points of interaction between a user and a website application. Forms allow data to be entered, stored and processed via a web server.

2. When designing a form, what are some key things to keep in mind when it comes to user experience?
Keep it simple and only ask for data you absolutley need.

3. List 5 form elements and explain their importance.
- `form` element defines a form and is a container that supports specific attributes to configure the way forms behave.
- `input` allows a single line of text input from the user to be stored with numerous additional attributes that can be applied with it, most importantly is `type` attribute
- `button` allows a send or submit button on the webpage that sends information to perform an action that its given
- `fieldset` creates groups of widgets that share the same purpose for styling and semantic purposes
- `label` gives definition to an HTML widget and is the most important element to build successful forms; can be clickable to activare a widget
    <form action="/my-handling-form-page" method="post">
      <ul>
        <li>
          <label for="name">Name:</label>
          <input type="text" id="name" name="user_name" />
        </li>
        <li>
          <label for="mail">Email:</label>
          <input type="email" id="mail" name="user_email" />
        </li>
        <li>
          <label for="msg">Message:</label>
          <textarea id="msg" name="user_message"></textarea>
        </li>
      </ul>
    </form>

## JS Intro to events
- [IntroToEvents](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

1. How would you describe events to a non-technical friend?
Events are an alert system to something that has happened or is happening.

2. When using the `addEventListener()` method, what 2 arguments will you need to provide?
The name of the event we want to register the handler for and the code that comprises the handler function we want to run in response to it.

3. Describe the event object. Why is the target within the event object useful?
It is automatically passed to event handlers to provide extra features and information. The target within the event is useful because it stores additional information, for example the keydown event and its event object keyboardevent. Keydown goes off when the user presses a key and keyboardevent tells which key was pressed.

4. What is the difference between event bubbling and event capturing?
Event Bubbling − Whenever an event happens on an element, the event handlers will first run on it and then on its parent and finally all the way up to its other ancestors. Event Capturing − It is the reverse of the event bubbling and here the event starts from the parent element and then to its child element.

## Things I want to know more about
The following bookmarked content:
- [HTML5InputTypes](https://developer.mozilla.org/en-US/docs/Learn/Forms/HTML5_input_types)
- [EventReferenceandlistings](https://developer.mozilla.org/en-US/docs/Web/Events)
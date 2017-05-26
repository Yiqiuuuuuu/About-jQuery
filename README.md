# About-jQuery

## :yellow_heart:jQuery Selectors

| Selector             | Example                    | Selects                                                                                                         |
|----------------------|----------------------------|-----------------------------------------------------------------------------------------------------------------|
| *                    | $("*")                     | All elements                                                                                                    |
| #id                  | $("#lastname")             | The element with id="lastname"                                                                                  |
| .class               | $(".intro")                | All elements with class="intro"                                                                                 |
| .class,.class        | $(".intro,.demo")          | All elements with the class "intro" or "demo"                                                                   |
| element              | $("p")                     | All \<p> elements                                                                                                |
| el1,el2,el3          | $("h1,div,p")              | All \<h1>, \<div> and \<p> elements                                                                                |
|                      |                            |                                                                                                                 |
| :first               | $("p:first")               | The first \<p> element                                                                                           |
| :last                | $("p:last")                | The last \<p> element                                                                                            |
| :even                | $("tr:even")               | All even \<tr> elements                                                                                          |
| :odd                 | $("tr:odd")                | All odd \<tr> elements                                                                                           |
|                      |                            |                                                                                                                 |
| :first-child         | $("p:first-child")         | All \<p> elements that are the first child of their parent                                                       |
| :first-of-type       | $("p:first-of-type")       | All \<p> elements that are the first \<p> element of their parent                                                 |
| :last-child          | $("p:last-child")          | All \<p> elements that are the last child of their parent                                                        |
| :last-of-type        | $("p:last-of-type")        | All \<p> elements that are the last \<p> element of their parent                                                  |
| :nth-child(n)        | $("p:nth-child(2)")        | All \<p> elements that are the 2nd child of their parent                                                         |
| :nth-last-child(n)   | $("p:nth-last-child(2)")   | All \<p> elements that are the 2nd child of their parent, counting from the last child                           |
| :nth-of-type(n)      | $("p:nth-of-type(2)")      | All \<p> elements that are the 2nd \<p> element of their parent                                                   |
| :nth-last-of-type(n) | $("p:nth-last-of-type(2)") | All \<p> elements that are the 2nd \<p> element of their parent, counting from the last child                     |
| :only-child          | $("p:only-child")          | All \<p> elements that are the only child of their parent                                                        |
| :only-of-type        | $("p:only-of-type")        | All \<p> elements that are the only child, of its type, of their parent                                          |
|                      |                            |                                                                                                                 |
| parent > child       | $("div > p")               | All \<p> elements that are a direct child of a \<div> element                                                     |
| parent descendant    | $("div p")                 | All \<p> elements that are descendants of a \<div> element                                                        |
| element + next       | $("div + p")               | The \<p> element that are next to each \<div> elements                                                            |
| element ~ siblings   | $("div ~ p")               | All \<p> elements that are siblings of a \<div> element                                                           |
|                      |                            |                                                                                                                 |
| :eq(index)           | $("ul li:eq(3)")           | The fourth element in a list (index starts at 0)                                                                |
| :gt(no)              | $("ul li:gt(3)")           | List elements with an index greater than 3                                                                      |
| :lt(no)              | $("ul li:lt(3)")           | List elements with an index less than 3                                                                         |
| :not(selector)       | $("input:not(:empty)")     | All input elements that are not empty                                                                           |
|                      |                            |                                                                                                                 |
| :header              | $(":header")               | All header elements \<h1>, \<h2> ...                                                                              |
| :animated            | $(":animated")             | All animated elements                                                                                           |
| :focus               | $(":focus")                | The element that currently has focus                                                                            |
| :contains(text)      | $(":contains('Hello')")    | All elements which contains the text "Hello"                                                                    |
| :has(selector)       | $("div:has(p)")            | All \<div> elements that have a <p> element                                                                      |
| :empty               | $(":empty")                | All elements that are empty                                                                                     |
| :parent              | $(":parent")               | All elements that are a parent of another element                                                               |
| :hidden              | $("p:hidden")              | All hidden \<p> elements                                                                                         |
| :visible             | $("table:visible")         | All visible tables                                                                                              |
| :root                | $(":root")                 | The document's root element                                                                                     |
| :lang(language)      | $("p:lang(de)")            | All \<p> elements with a lang attribute value starting with "de"                                                 |
|                      |                            |                                                                                                                 |
| [attribute]          | $("[href]")                | All elements with a href attribute                                                                              |
| [attribute=value]    | $("[href='default.htm']")  | All elements with a href attribute value equal to "default.htm"                                                 |
| [attribute!=value]   | $("[href!='default.htm']") | All elements with a href attribute value not equal to "default.htm"                                             |
| [attribute$=value]   | $("[href$='.jpg']")        | All elements with a href attribute value ending with ".jpg"                                                     |
| [attribute\|=value]   | $("[title\|='Tomorrow']")   | All elements with a title attribute value equal to 'Tomorrow', or starting with 'Tomorrow' followed by a hyphen |
| [attribute^=value]   | $("[title^='Tom']")        | All elements with a title attribute value starting with "Tom"                                                   |
| [attribute~=value]   | $("[title~='hello']")      | All elements with a title attribute value containing the specific word "hello"                                  |
| [attribute*=value]   | $("[title*='hello']")      | All elements with a title attribute value containing the word "hello"                                           |
|                      |                            |                                                                                                                 |
| :input               | $(":input")                | All input elements                                                                                              |
| :text                | $(":text")                 | All input elements with type="text"                                                                             |
| :password            | $(":password")             | All input elements with type="password"                                                                         |
| :radio               | $(":radio")                | All input elements with type="radio"                                                                            |
| :checkbox            | $(":checkbox")             | All input elements with type="checkbox"                                                                         |
| :submit              | $(":submit")               | All input elements with type="submit"                                                                           |
| :reset               | $(":reset")                | All input elements with type="reset"                                                                            |
| :button              | $(":button")               | All input elements with type="button"                                                                           |
| :image               | $(":image")                | All input elements with type="image"                                                                            |
| :file                | $(":file")                 | All input elements with type="file"                                                                             |
| :enabled             | $(":enabled")              | All enabled input elements                                                                                      |
| :disabled            | $(":disabled")             | All disabled input elements                                                                                     |
| :selected            | $(":selected")             | All selected input elements                                                                                     |
| :checked             | $(":checked")              | All checked input elements                                                         



## :yellow_heart:jQuery Event Methods

| Method / Property                     | Description                                                                                                                                         |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| bind()                                | Deprecated in version 3.0. Use the on() method instead. Attaches event handlers to elements                                                         |
| blur()                                | Attaches/Triggers the blur event                                                                                                                    |
| change()                              | Attaches/Triggers the change event                                                                                                                  |
| click()                               | Attaches/Triggers the click event                                                                                                                   |
| dblclick()                            | Attaches/Triggers the double click event                                                                                                            |
| delegate()                            | Deprecated in version 3.0. Use the on() method instead. Attaches a handler to current, or future, specified child elements of the matching elements |
| die()                                 | Removed in version 1.9. Removes all event handlers added with the live() method                                                                     |
| error()                               | Removed in version 3.0. Attaches/Triggers the error event                                                                                           |
| event.currentTarget                   | The current DOM element within the event bubbling phase                                                                                             |
| event.data                            | Contains the optional data passed to an event method when the current executing handler is bound                                                    |
| event.delegateTarget                  | Returns the element where the currently-called jQuery event handler was attached                                                                    |
| event.isDefaultPrevented()            | Returns whether event.preventDefault() was called for the event object                                                                              |
| event.isImmediatePropagationStopped() | Returns whether event.stopImmediatePropagation() was called for the event object                                                                    |
| event.isPropagationStopped()          | Returns whether event.stopPropagation() was called for the event object                                                                             |
| event.namespace                       | Returns the namespace specified when the event was triggered                                                                                        |
| event.pageX                           | Returns the mouse position relative to the left edge of the document                                                                                |
| event.pageY                           | Returns the mouse position relative to the top edge of the document                                                                                 |
| event.preventDefault()                | Prevents the default action of the event                                                                                                            |
| event.relatedTarget                   | Returns which element being entered or exited on mouse movement.                                                                                    |
| event.result                          | Contains the last/previous value returned by an event handler triggered by the specified event                                                      |
| event.stopImmediatePropagation()      | Prevents other event handlers from being called                                                                                                     |
| event.stopPropagation()               | Prevents the event from bubbling up the DOM tree, preventing any parent handlers from being notified of the event                                   |
| event.target                          | Returns which DOM element triggered the event                                                                                                       |
| event.timeStamp                       | Returns the number of milliseconds since January 1, 1970, when the event is triggered                                                               |
| event.type                            | Returns which event type was triggered                                                                                                              |
| event.which                           | Returns which keyboard key or mouse button was pressed for the event                                                                                |
| focus()                               | Attaches/Triggers the focus event                                                                                                                   |
| focusin()                             | Attaches an event handler to the focusin event                                                                                                      |
| focusout()                            | Attaches an event handler to the focusout event                                                                                                     |
| hover()                               | Attaches two event handlers to the hover event                                                                                                      |
| keydown()                             | Attaches/Triggers the keydown event                                                                                                                 |
| keypress()                            | Attaches/Triggers the keypress event                                                                                                                |
| keyup()                               | Attaches/Triggers the keyup event                                                                                                                   |
| live()                                | Removed in version 1.9. Adds one or more event handlers to current, or future, selected elements                                                    |
| load()                                | Removed in version 3.0. Attaches an event handler to the load event                                                                                 |
| mousedown()                           | Attaches/Triggers the mousedown event                                                                                                               |
| mouseenter()                          | Attaches/Triggers the mouseenter event                                                                                                              |
| mouseleave()                          | Attaches/Triggers the mouseleave event                                                                                                              |
| mousemove()                           | Attaches/Triggers the mousemove event                                                                                                               |
| mouseout()                            | Attaches/Triggers the mouseout event                                                                                                                |
| mouseover()                           | Attaches/Triggers the mouseover event                                                                                                               |
| mouseup()                             | Attaches/Triggers the mouseup event                                                                                                                 |
| off()                                 | Removes event handlers attached with the on() method                                                                                                |
| on()                                  | Attaches event handlers to elements                                                                                                                 |
| one()                                 | Adds one or more event handlers to selected elements. This handler can only be triggered once per element                                           |
| $.proxy()                             | Takes an existing function and returns a new one with a particular context                                                                          |
| ready()                               | Specifies a function to execute when the DOM is fully loaded                                                                                        |
| resize()                              | Attaches/Triggers the resize event                                                                                                                  |
| scroll()                              | Attaches/Triggers the scroll event                                                                                                                  |
| select()                              | Attaches/Triggers the select event                                                                                                                  |
| submit()                              | Attaches/Triggers the submit event                                                                                                                  |
| toggle()                              | Removed in version 1.9. Attaches two or more functions to toggle between for the click event                                                        |
| trigger()                             | Triggers all events bound to the selected elements                                                                                                  |
| triggerHandler()                      | Triggers all functions bound to a specified event for the selected elements                                                                         |
| unbind()                              | Deprecated in version 3.0. Use the off() method instead. Removes an added event handler from selected elements                                      |
| undelegate()                          | Deprecated in version 3.0. Use the off() method instead. Removes an event handler to selected elements, now or in the future                        |
| unload()                              | Removed in version 3.0. Attaches an event handler to the unload event                                                                               |


## :yellow_heart:jQuery Effect Methods

| Method        | Description                                                                  |
|---------------|------------------------------------------------------------------------------|
| animate()     | Runs a custom animation on the selected elements                             |
| clearQueue()  | Removes all remaining queued functions from the selected elements            |
| delay()       | Sets a delay for all queued functions on the selected elements               |
| dequeue()     | Removes the next function from the queue, and then executes the function     |
| fadeIn()      | Fades in the selected elements                                               |
| fadeOut()     | Fades out the selected elements                                              |
| fadeTo()      | Fades in/out the selected elements to a given opacity                        |
| fadeToggle()  | Toggles between the fadeIn() and fadeOut() methods                           |
| finish()      | Stops, removes and completes all queued animations for the selected elements |
| <font color="#ff1a8c">hide()</font>       | Hides the selected elements <font color="#ff1a8c">$(selector).hide(speed,callback);<font>                                                  |
| queue()       | Shows the queued functions on the selected elements                          |
| <font color="#ff1a8c">show()</font>        | Shows the selected elements <font color="#ff1a8c">$(selector).show(speed,callback);<font>                                                  |
| slideDown()   | Slides-down (shows) the selected elements                                    |
| slideToggle() | Toggles between the slideUp() and slideDown() methods                        |
| slideUp()     | Slides-up (hides) the selected elements                                      |
| stop()        | Stops the currently running animation for the selected elements              |
| <span style="color:#ff1a8c">toggle()</span>     | Toggles between the hide() and show() methods    <font color="#ff1a8c">$(selector).toggle(speed,callback);<font>                              |





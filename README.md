
ABOUT FEEDBACK UI DESIGN PROJECT OVERVIEW
_________________________

### **HTML Structure**

* `<!DOCTYPE html>` – Declares HTML5 document type.
* `<html lang="en">` – Starts the HTML document, sets language to English.
###  **Head Section**

* `<head>` – Contains metadata and links for styles and icons.

  * `<meta charset="UTF-8">` – Sets character encoding to UTF-8.
  * `<meta name="viewport"...>` – Makes page responsive on all devices.
  * `<link rel="stylesheet" href="font-awesome">` – Loads Font Awesome icons.
  * `<link rel="stylesheet" href="style.css">` – Loads external CSS for styling.
  * `<title>` – Sets the page title shown in browser tab.

###  **Body Section**

* `<body>` – Contains everything visible on the web page.


###  **Main Feedback Panel**

* `<div id="panel" class="panel-container">` – Main container for the feedback form.

#### Inside the Panel:

* `<strong>` – Bold question text asking for customer support feedback.

  * `<br />` – Breaks the line in the question.

###  **Ratings Section**

* `<div class="ratings-container">` – Container for emoji rating options.

Each rating:

* `<div class="rating">` – One rating option (emoji + label).

  * `<img src="...">` – Emoji icon image.
  * `<small>` – Text label (e.g., "Unhappy", "Neutral", "Satisfied").
* `class="rating active"` – The default selected emoji is marked with `active`.

###  **Submit Button**

* `<button class="btn" id="send">` – A button to send the selected review.
_____________________________________
JAVASCRIPT CODE 

###  `<!DOCTYPE html>`

Declares the document as HTML5.

###  `<html lang="en">`

Root of the HTML page, language set to English.

###  `<head>`

Contains metadata and links (not visible on the page).

* `<meta charset="UTF-8">` – Sets character encoding.
* `<meta name="viewport"...>` – Makes the layout responsive.
* `<link>` – Links external stylesheets (CSS and icons).
* `<title>` – Sets the page title shown in browser/tab.

###  `<body>`

Holds all **visible content**.

###  `<div>`

Generic container used to group content.

* `id="panel"` – Identifies the main feedback panel.
* `class="panel-container"` – Applies styles from CSS.
* `class="ratings-container"` – Groups all the emoji ratings.
* `class="rating"` – Represents a single rating block.
* `class="rating active"` – Highlights the selected rating.

###  `<strong>`

Displays bold, emphasized text (used for headings/questions).

###  `<br>`

Line break (moves content to the next line).

###  `<img>`

Displays an image (used here for emoji icons).

* `src="..."` – Image URL.
* `alt="..."` – Alternative text (for accessibility).

### `<small>`

Displays smaller-sized text (used for labels under emojis).

###  `<button>`

Clickable button (used to submit feedback).

* `class="btn"` – For styling.
* `id="send"` – For targeting in JavaScript.

###  `<script>`

Links an external JavaScript file to add interactivity.
___________________
STYLE CSS  CODE

###  `@import`
* Imports the **Montserrat** font from Google Fonts.

### `*`

* Applies to **all elements**.
* Uses `box-sizing: border-box` to include padding and border in element width/height.
### `body`

* Sets **background color**, **font**, and centers content using Flexbox.
* Fills full screen height (`100vh`), hides overflow, removes default margin.

### `.panel-container`

* Styles the main feedback **box**.
* Adds white background, shadow, padding, rounded corners, and centers content.

###  `.panel-container strong`

* Sets **line height** for the bold text (question).

###  `.ratings-container`

* Arranges the emoji ratings in a **horizontal row** with some spacing.


### `.rating`

* Each emoji + label block.
* Makes it clickable (`cursor: pointer`), adds padding and margin.

###  `.rating:hover`, `.rating.active`

* Adds **hover effect** and highlight for selected rating:

* Shadow and rounded corners.

###  `.rating img`

* Sets emoji icon size to **40px**.

###  `.rating small`

* Styles the label text below emojis:

* Gray color, spacing on top.

### `.rating:hover small`, `.rating.active small`

* Changes label color to darker gray when hovered or selected.

###  `.btn`

* Styles the **"Send Review" button**:

* Dark background, white text, rounded corners, padding.

###  `.btn:focus`

* Removes blue outline when button is focused.

### `.btn:active`

* Slightly shrinks the button on click (`scale(0.98)`).

###  `.fa-heart`

* Styles the **heart icon**:

  * Red color, larger size (30px), margin below.




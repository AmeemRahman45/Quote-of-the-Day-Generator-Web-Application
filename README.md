<h1>🌟 Quote of the Day Generator 🌟</h1>
<p>
    Welcome to the Quote of the Day Generator! This simple yet powerful web app delivers daily doses of motivation with a fresh quote every time you reload the  
    page or click a button.
</p>
<br>
<h3>🚀 Features</h3>
<ul>
    <li>🎉 Interactive Quote Display: Click a button to reveal a new inspiring quote.</li>
    <li>🎨 Elegant Design: A visually appealing background and clean layout.</li>
    <li>🔄 Dynamic Content: Quotes are displayed randomly from a predefined list.</li>
</ul>
<br>
<h3>🔧 Technologies Used</h3>
<ul>
    <li>HTML: Structure and layout.</li>
    <li>CSS: Styling and responsive design.</li>
    <li>JavaScript: Functionality for generating and displaying quotes.</li>
</ul>
<br><br>
<h3>📋 Code Explanation</h3>
<ol>
    <li>
        <h4>HTML Structure</h4>
        <pre>
&lt;!DOCTYPE html&gt;: Defines the document type and version of HTML.
&lt;html lang="en"&gt;: Begins the HTML document and specifies English as the language.
&lt;head&gt;: Contains meta-information about the document, such as character encoding, viewport settings, and links to external resources.
    &lt;meta charset="UTF-8"&gt;: Sets the character encoding to UTF-8.
    &lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;: Ensures the page is responsive on all devices.
    &lt;title&gt;: Sets the title of the page that appears in the browser tab.
    &lt;link&gt;: Includes external resources such as fonts from Google Fonts and a stylesheet for styling.
&lt;/head&gt;
&lt;body&gt;: Contains the content of the webpage.
    &lt;div class="container"&gt;: A central container for aligning and styling content.
        &lt;h1 class="quoteTitle"&gt;: A heading for the quote section, styled to stand out.
        &lt;blockquote id="quote"&gt;: Displays the quote. It starts with a placeholder text.
        &lt;button id="newQuoteBtn"&gt;: A button that, when clicked, will trigger the display of a new quote.
    &lt;/div&gt;
    &lt;script src="/js/main.js"&gt;&lt;/script&gt;: Links to an external JavaScript file that contains the logic for generating and displaying quotes.
&lt;/body&gt;
        </pre>
    </li>
    <li>
        <h4>CSS Styling</h4>
        <pre>
body: Styles the background and centers the content vertically and horizontally.
    background-image: url('/img/Niagara-Falls.jpg'): Sets a full-screen background image.
    background-size: cover: Ensures the image covers the entire background area.
    background-repeat: no-repeat: Prevents the image from repeating.
    background-position: center center: Centers the background image.
.container: Styles the container that holds the content.
    text-align: center: Centers text inside the container.
    background-color: #fff: Sets a white background for better contrast.
    padding: 25px: Adds padding inside the container.
    border-radius: 10px: Rounds the corners of the container.
    border: solid #44B9BD 5px: Adds a border with a specific color and thickness.
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1): Adds a subtle shadow for a 3D effect.
.quoteTitle: Styles the heading for the quote section.
    font-family: "Playfair Display", serif: Uses a serif font for a classic look.
    font-size: 44px: Makes the font size large for emphasis.
    font-weight: 600: Makes the font slightly bold.
blockquote: Styles the quote text.
    font-size: 22px: Sets a readable font size for quotes.
    font-family: "Roboto", sans-serif: Uses a sans-serif font for modern readability.
    font-weight: 600: Makes the font bold.
    margin: 0: Removes default margin.
    padding: 10px: Adds padding around the quote text.
    border-left: 5px solid #99D9DF: Adds a left border with a specific color for emphasis.
button: Styles the button used to generate a new quote.
    background-color: #0BA5A4: Sets a turquoise background color.
    color: #ffff: Makes the button text white.
    border: none: Removes default button border.
    padding: 10px 20px: Adds padding inside the button.
    font-size: 18px: Sets the font size of the button text.
    border-radius: 5px: Rounds the corners of the button.
    cursor: pointer: Changes the cursor to a pointer when hovering over the button.
    margin-top: 20px: Adds space above the button.
button:hover: Styles the button when hovered over.
    background-color: #68B7D0: Changes the button color on hover for a visual effect.
        </pre>
    </li>
    <li>
        <h4>JavaScript Functionality</h4>
        <pre>
const quotes = [...]: An array of motivational quotes.
function getRandomQuote(): Returns a random quote from the array.
    Math.floor(Math.random() * quotes.length): Generates a random index to select a quote.
function displayNewQuote(): Updates the text content of the blockquote element with a new quote.
    document.getElementById('quote').textContent = getRandomQuote();: Sets the text of the quote element.
document.getElementById('newQuoteBtn').addEventListener('click', displayNewQuote);: Adds an event listener to the button to call displayNewQuote when clicked.
displayNewQuote();: Calls the function to display a quote when the page loads.
        </pre>
    </li>
</ol>

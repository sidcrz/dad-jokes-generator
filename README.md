<u>WORKING OF DAD <U>



This code is a JavaScript implementation that utilizes the Document Object Model (DOM) and the Fetch API to retrieve a dad joke from an API endpoint and display it on the webpage.

The first step is to access the necessary HTML elements. The code declares two variables, "btnEl" and "jokeEl", which use the document.getElementById() method to select the elements with the corresponding ids "btn" and "joke" from the HTML document.

Next, the code declares a variable "apiKey" that contains the API key required to make requests to the API endpoint. A "options" variable is then declared, which contains an object that specifies the request method as "GET" and includes the API key in the headers with the key "X-Api-Key". A variable named "apiURL" that contains the API endpoint URL is also declared.

The code then defines an asynchronous function "getJoke" which is used to handle the joke retrieval and display process. Inside this function, the inner text of the "jokeEl" element is updated to "Updating...", the "btnEl" element is disabled, and its inner text is changed to "Loading...".

The code then uses the Fetch API's fetch() method to make a request to the API endpoint using the "options" and "apiURL" variables. The promise returned by the fetch method is awaited and the response is saved to a variable "response". The json method is used on the response to parse the data and the result is saved to a variable "data".

The code then sets the "btnEl" element to be enabled again, changes its text back to "Tell me a joke", and displays the joke on the page by setting the inner text of the "jokeEl" element to the joke in the "data" variable.

In case of any error, the code updates the text of the "jokeEl" element to "An error happened, try again later", enables the "btnEl" element again, changes its text back to "Tell me a joke", and logs the error to the console.

Finally, an event listener is added to the "btnEl" element that listens for click events and calls the "getJoke" function when triggered, allowing the user to retrieve a new joke by clicking the button

<img width="959" alt="image" src="https://user-images.githubusercontent.com/57244923/213877541-9ec641bc-cda6-45dd-b13c-b49d85b2c197.png">

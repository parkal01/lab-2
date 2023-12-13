questions answers
a. Assume that in your API call you received a 401 status code. Which part of your code most probably is not correct?

If you receive a 401 status code in your API call, it most likely indicates an authentication issue. Check the following:

Ensure that you have a valid API key and that it's correctly set in the x-rapidapi-key header.
Verify that your API key has the necessary permissions to access the Open Weather Map API.
b. Explain your design choices and how you used CSS to realize those changes.

In designing our weather app, we aimed for a clean and user-friendly interface. Here are some of our design choices and how CSS was used:

Background: We set a light background color to make the content more readable and visually pleasing.
Text and Font: We used different colors for text to provide visual contrast. The "h1" heading is blue, and "p" elements are red. We adjusted the font family to "Arial, sans-serif" for better readability.
Container: We styled a container div element with a maximum width, padding, background color, box shadow, and border radius to create a well-defined and centered content area.
Input Fields: We adjusted the input fields to have a white background, padding, border, and rounded corners for a polished look.
Submit Button: We designed the submit button with a blue background, white text, rounded corners, and a cursor pointer for user interactivity.


 steps:
 
Install Node.js:

If you don't have Node.js installed, download and install it from here. Choose the LTS version.
Open a Terminal:

Open your terminal of choice.
On Windows, you can use the Windows Terminal or git-bash.exe (run as admin).
On Unix-based systems, use your preferred terminal.
Set Up Your Project:

bash
Copy code
mkdir WeatherApp
cd WeatherApp
touch index.html weatherapp.js
Initialize the Project:

Run npm init to set up package management.
Install Express:

Install the Express package using npm.
bash
Copy code
npm install express
Edit weatherapp.js:

Open weatherapp.js and write the following code:
javascript
Copy code
// Require express
const express = require('express');
const app = express();

// Start server on port 8002
const port = 8002;
app.listen(port, () => {
  console.log(`Server is running on port ${port}`);
});

// Your API call and weather data processing code here
Make API Call:

Follow Stack Overflow or online resources to make an external API call.
Use the https module and https.get().
Parse API Response:

Parse the result from https.get() using JSON.parse().
Check Status Code:

Check if the status code is 200 (successful communication).

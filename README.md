# Weather-Connect

# On Form Submission
Each time a user submits the form by pressing the Enter key or the Submit button, we’ll do two things:

Stop the form from submitting, hence prevent reloading the page.
Grab the value which is contained in the search field.

# Perform an AJAX Request
We’ll start with the assumption that the list is empty. That said, it has never run any AJAX request in the past. In such a case, we’ll execute a request to the OpenWeatherMap API and pass the following parameters:

The city name (e.g. athens) or the comma-separated city name along with the country code (e.g. athens,gr) which will be the value of the search field
The API key. Again, you should use your own key to avoid unexpected errors due to API call limits.
The unit of temperature for the requested city. In our case, we’ll go with Celcius.
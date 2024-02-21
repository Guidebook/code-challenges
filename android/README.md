# Summary
Create an Android application that displays information received over the network.

*Note: As you will be uploading your solution to GitHub, please do do not include the word “Guidebook” anywhere in your code.*

# Details

The server at the following url responds with JSON formatted data:

```(GET) https://builder.guidebook.com/service/v2/upcomingGuides/```

The response represents a list of “Guide” objects:

```json
{
  "data": [
  {
    "startDate": "<date>",
    "endDate": "<date>",
    "name": "<name>",
    "url": "<url>",
    "venue": {"city": "<city>", "state": "<state>"},
    "icon": "<url to png image>"
    },
    … <more objects>
    ]
  }
  ```

# Deliverables
Spend rougly 1 - 2 hours completing as many of the following deliverables as possible. Please use the MVVM pattern to structure your code.

* Retrieve and print out the data received from the url above.

* Parse the data retrieved from the server into a list of objects (Kotlin or Java).

* Display your objects in a ListView or RecyclerView
  - Every item should show the guide name and start date

* Create two build configurations, labeled 'Build A', and 'Build B'
  - Depending on which configuration was built, the app should show text at the top of the list with the current build. For example, if the project was built for 'Build A', then 'Build A' would show at the top of the screen, followed by the list of guides.

* Write tests that cover the above requirements, how many tests you write and what you write them for is up to you

# Notes

* A README that explains a quick summary of the process you took when building this challenge is encouraged

* Note roughly how long this took you. If the challenge takes substantially longer than 1 - 2 hours, stop and write notes on where you left off before submitting
# Summary
Create an Android application that displays information received over the network.

*Note: As you will be uploading your solution to GitHub, please do do not include the word “Guidebook” anywhere in your code.*

# Details

The server at the following url responds with JSON formatted data:

```(GET) http://guidebook.com/service/v2/upcomingGuides/```

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

# Milestones
Spend no more than an hour completing as many of these steps as possible.

1. Retrieve and print out the data received from the url above.

2. Parse the data retrieved from the server into a list of Java objects

3. Display your objects in an organized fashion (ListView, GridView, etc.)
  - Only worry about displaying the name for this step

4. In addition the object’s **name**, have your view display the image located at each object’s **icon** url.

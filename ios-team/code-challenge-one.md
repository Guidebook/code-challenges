# iOS Coding Challenge One

Create an iOS application that fetches JSON data from a Guidebook API endpoint and displays
it using a table view. You may use any 3rd party libraries to build the application.

## API Endpoint
The following endpoint responds with JSON data, representing a list of upcoming guides.

More specifically, the value for the `data` key is an array of JSON objects where
each object contains key-value information about a specific guide.

**URL:**
`GET https://www.guidebook.com/service/v2/upcomingGuides/`

**Sample Response:**

```js
{  
  "total":"1",
  "data":[  
            {  
              "startDate":"Jan 23, 2015",
              "endDate":"Jan 25, 2015",
              "name":"PAX South 2015",
              "url":"/guide/27558",
              "venue":{  
                "city":"San Antonio",
                "state":"TX"
              },
              "objType":"guide",
              "icon":"https://s3.amazonaws.com/media.guidebook.com/service/ghuQSj9675C8zKbaXtUTAMWxsVGkJf4r/logo.png"
            }
        ]
}
```

##Challenge Milestones

#### Milestone One
- Create an iOS XCode project or workspace for this application in a new git repo.
- Asynchronously fetch and print (NSLog) the response data received from the API endpoint described above.

#### Milestone Two
- Parse the retrieved JSON data into an array of objects of class `Guide`

#### Milestone Three
- Display the `Guide` objects in a UITableView. Each table cell represents one `Guide` object and should display it's name, city, state, start date, and end date.

#### Milestone Four
- Display the table cells sorted in ascending order by guide start date.

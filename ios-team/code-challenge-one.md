# iOS Coding Challenge One

Create an iOS application written in **Objective-C** that fetches JSON data from a Guidebook API endpoint and displays
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
- Display the `Guide` objects in a UITableView or UICollectionView. Each cell represents one `Guide` object and should display it's name, city, state, and end date.

#### Milestone Four
- Group the cells within UITableView or UICollectionView Sections by the `startDate` attribute.
  - The sections should be displayed in ascending `startDate` order.
  - The section header titles should be the `startDate` value in the sample format: "Jan 23, 2015"

**Example of cells:**  
**You may customize the design however you like!**

![image](https://s3.amazonaws.com/uploads.hipchat.com/17292/98408/x1KgCYy0SXeyRQq/Screen%20Shot%202015-06-29%20at%204.08.03%20PM.png)

#### Bonus:
- Implement Pull to Refresh functionality.

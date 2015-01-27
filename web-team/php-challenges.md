# PHP challenge #

We want to create a database of all the PAX related guide currently available on Guidebook for a case study.

**Challenge:** Create a PHP(5) project that will retrieve a list of guides using the `pax` keyword and save it into a database.

In this challenge, your project must be Object-Oriented.
The URL used to search for guides is `https://guidebook.com/om/service/v2/search/`. You will have to send a GET parameter `q` with the keyword you want to use to do your research.

a guide object will look like:

```javascript
{
    "startDate":"2014-10-17T00:00:00",
    "endDate":"2014-10-19T00:00:00",
    "landing_url":"/g/WellesleyFamilyandFriendsWeekend",
    "default_venue":"",
    "large_icon":"",
    "id":"22866",
    "icon":"https://s3.amazonaws.com/media.guidebook.com/service/CTnHck9pxbLt7gKu54vN3JoVmjYwhB8r/logo.png",
    "guideVersion":34,
    "gb_url":"gb://redeem/?guideId=22866",
    "minAppVersion-Android":31,
    "name":"Wellesley Family & Friends Weekend and Homecoming 2014",
    "url":"/guide/22866/",
    "venue":{
        "city":"Wellesley",
        "state":"MA",
        "street":"106 Central Street",
        "name":"Wellesley College",
        "zipcode":"02481"
    },
    "productIdentifier":"CTnHck9pxbLt7gKu54vN3JoVmjYwhB8r",
    "bundleVersion":0,
    "minAppVersion-iOS":"30",
    "type":"guide"
}
```

Once you have the list of guides, save them into a database. It could be a good idea to use PDO here.
You might have to create several tables but the schema structure is entirely up to you.

### What We'll Be Looking At ###

We want to make sure that the solution implements OO patterns properly and that the project is structured in a logical manner.
We also want to make sure that your code is clean and commented.
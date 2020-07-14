# Projects

## GET

###  List of all projects
Returns a list (array of JSON objects) of all projects.

Route: `/projects`

<!-- Sample Response -->
<details>
<summary>Sample Response</summary>
<pre>
[
    {
        "contributors": [
            "test",
            "test2"
        ],
        "_id": "5f089dcf520ee1090b7bea56",
        "createdDate": "2020-07-10T16:56:29.830Z",
        "name": "wonderful API",
        "description": "The wonderful api"
    },
    {
        "contributors": [
            "test1",
            "test2"
        ],
        "_id": "5f089dde520ee1090b7bea57",
        "createdDate": "2020-07-10T16:56:29.830Z",
        "name": "Wonderful API 2",
        "description": "The 2nd wonderful api"
    },
]
</pre>
</details>


## POST

### Create a project
Uploads a new project details to database

Route: `/projects`

Fields:
* contributors (Required, [Strings])
* name (Required, String)
* description (Required, String)
* createdDate (Required, Date<sup>1</sup>)

<!-- Sample Request -->
<details>
<Summary>Sample Request</Summary>
<pre>
{
    "contributors": ["test" ,"test"],
    "name":"wonderful API",
    "description": "The wonderful api"
}
</pre>
</details>

<!-- Sample Response -->
<details>
<Summary>Sample Response</Summary>
<pre>
{
    "contributors": [
        "test",
        "test"
    ],
    "_id": "5f08a564024426120ebfcfcd",
    "name": "wonderful API",
    "description": "The wonderful api",
    "createdDate": "2020-07-10T17:29:08.996Z",
    "__v": 0
}
</pre>
</details>

---
1. Checkout [momentJS docs](https://momentjs.com/docs/#/parsing/string/) for formating date and time.
---

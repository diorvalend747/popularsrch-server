# I Project - PopularSrch 

RESTful endpoint 
JSON formatted response

## RESTful endpoints

## 
##

### GET /reddit

> Get data Search from Reddit


_Request Body_

```
{
    "q": "<insert string>",

}
```


Response (200)

```
{
    approved_at_utc": null,
    "subreddit": "Bossfight",
    "selftext": "",
    "author_fullname": "t2_c5y87hiy",
    "saved": false,
    "mod_reason_title": null,
    ...
}   
```

Response (400 - Bad Request)

```
{
  "message": "Invalid request"
}
```

Response (500 - Bad Request)

```
{
  "message": "Internal server error"
}
```

### get /twitter

> Get data Search from Twitter


Request Body

```
{
  "query": "<insert string>",
}
```

Response (200 - Created)

```
{
    "data": [
                {
                    "id": "1400338663762919425",
                    "text": "string"
                },
                {
                    "id": "1400338652643971077",
                    "text": "string"
                },
            ]
}
```


Response (401 - Request Failed)

```
{
    "message": "Request failed with status code 401"
}
```

Response (500 - Bad Request)

```
{
  "message": "Internal server error"
}
```

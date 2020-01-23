# API Project: URL Shortener Microservice for freeCodeCamp


## Specification from freeCodeCamp

### User Stories

1. I can POST a URL to `[this_project_url]/api/shorturl/new` and I will receive a shortened URL in the JSON response. Example : `{"original_url":"www.google.com","short_url":1}`
2. If I pass an invalid URL that doesn't follow the valid `http(s)://www.example.com(/more/routes)` format, the JSON response will contain an error like `{"error":"invalid URL"}`. *HINT*: to be sure that the submitted url points to a valid site you can use the function `dns.lookup(host, cb)` from the `dns` core module.
3. When I visit the shortened URL, it will redirect me to my original link.

#### Creation Example:

POST [this_project_url]/api/shorturl/new - body (urlencoded) : url=https://www.google.com

#### Usage:

[this_project_url]/api/shorturl/3

#### Will redirect to:

https://www.freecodecamp.org/forum/


## Project Documentation

### This Project URL:

https://wikankun-urlshortener.glitch.me

### API Documentation:

1. [this_project_url]/api/shorturl/new [HTTP POST]  : record link to database 
2. [this_project_url]/api/shorturl [HTTP GET]       : get all saved links
3. [this_project_url]/api/shorturl/<id> [HTTP GET]  : get link by shortened url and redirect
# PagesJaunes-API
Complete API of Pages Jaunes to Scrap Data www.pagesjaunes.fr with Free Version

https://rapidapi.com/schmidtfischer2/api/pagesjaunes1

### POST /search
get our data with the search field and the place field that we got on the /placecode route. To have the following pages we will use the pagenb and the searchid field that we retrieved during our previous request. Please note that searchid expires after 30 min maximum

#### First Request JSON BODY
```
{
    "search": "plombier",
    "place": {
        "name": "Ile-de-France",
        "place_code": "R11"
    }
}
```
#### Seconde Request JSON BODY
```
{
    "search": "plombier",
    "page_nb": 2,
    "place": {
        "name": "Ile-de-France",
        "place_code": "R11"
    },
    "search_id": "20816058917350980025825118"
}
```

### POST /place_code
route to search adresse and to get place code of each adresse

#### JSON BODY
```
{
    "search": "ile de france"
}
```

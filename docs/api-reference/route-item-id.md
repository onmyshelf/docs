# API route: /collections/{id}/items/{id}

## GET method
Get details of an item

### Parameters
Nothing

### Return example
```json
{
  "id": 3,
  "collectionId": 1,
  "properties": {
    "cover": "media://2/2769c8c4a2627996223914b8.jpg",
    "title": "Book title",
    "author": "M. Book Author",
    "pages": 350
  },
  "visibility": 0
}
```

## DELETE method
Deletes item

### Parameters
Nothing

### Return example
```json
{
  "deleted": true
}
```

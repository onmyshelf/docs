# API route: /collections/{id}/items

## GET method
Get a preview of all items of a collection

### Parameters
Nothing

### Return example
```json
[
  {
    "id": 1,
    "properties": {
      "cover": "media://2/25279b78a99329a56f1e0b4242a3cf4a.jpg",
      "title": "Book title"
    },
    "thumbnail": {
      "small": "media://2/25279b78a99329a56f1e0b4242a3cf4a-small.jpg",
      "normal": "media://2/25279b78a99329a56f1e0b4242a3cf4a-normal.jpg",
    }
  },
]
```

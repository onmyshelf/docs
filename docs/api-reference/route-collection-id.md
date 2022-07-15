# API route: /collections/{id}

## GET method
Get a collection summary

### Parameters
Nothing

### Return example
```json
{
  "id": 1,
  "cover": "media://path/to/image.jpg",
  "owner": 1,
  "visibility": 0,
  "name": {
    "en_US": "My books",
    "fr_FR": "Mes livres"
  },
  "description": {
    "en_US": "My collection of books",
    "fr_FR": "Ma collection de livres"
  },
  "properties": {
    "cover": {
      "type": "image",
      "suffix": null,
      "default": null,
      "authorizedValues": null,
      "visibility": 0,
      "required": 0,
      "hideLabel": 0,
      "isId": 0,
      "isTitle": 0,
      "isSubTitle": 0,
      "isCover": 1,
      "preview": 1,
      "multiple": 0,
      "filterable": 0,
      "searchable": 0,
      "sortable": 0,
      "order": 0,
      "label": [],
      "description": []
    },
    "title": {
      "type": "text",
      "suffix": null,
      "default": null,
      "authorizedValues": null,
      "visibility": 0,
      "required": 0,
      "hideLabel": 0,
      "isId": 0,
      "isTitle": 1,
      "isSubTitle": 0,
      "isCover": 0,
      "preview": 1,
      "multiple": 0,
      "filterable": 0,
      "searchable": 1,
      "sortable": 1,
      "order": 0,
      "label": {
        "en_US": "Title",
        "fr_FR": "Titre"
      },
      "description": {
        "en_US": "Title of the book",
        "fr_FR": "Titre du livre"
      }
    },
  },
  "items": 42
}
```

## DELETE method
Deletes collection

### Parameters
Nothing

### Return exemple
```json
{
  "deleted": true
}
```

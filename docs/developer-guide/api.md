# API server

## Sources
On GitHub: [https://github.com/onmyshelf/api](https://github.com/onmyshelf/api)

## API language
OnMyShelf's API server is developed in PHP from scratch.

Contributors are welcome to help us make OnMyShelf API server a more secured
and (why not) make a complete refactoring.

## API documentation
To understand API, you can use the OpenAPI definition in `inc/openapi.json`.

## How it works
### Front calls
- The `Api` class manages every web requests
- The `bin/oms` file is used to run some admin operations from the command line

#### The Api class
Routes and controllers are defined in this class. Controllers calls main classes like `Collection`, `Item`, `User`, etc.

#### The oms command
The admin operations are made by command line. You have to go first into the project directory and do:
```bash
php bin/oms COMMAND
```

### Main classes
The main classes are stored in `inc/classes` and defines the main components like:

- Collection
- Item
- Property
- User
- ...

### Secondary classes
#### The Database class
The `Database` class manages every database operations.

You can create your own database modules to support any other DBMS.

#### The Storage class
The `Storage` class manages every file operations, espectially the media library.

You can create your own storage modules to support any other file system or protocol.

#### The Import class
The `Import` class manages every import requests, including query websites to autocomplete items.

You can create your own import modules to import data from API, websites, XML, CSV, etc.

#### Modules
As said above, you can extend or override the secondary classes by adding your own in `modules` directory.
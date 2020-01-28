# mongo-db
Studies on mongo and mongo express.

## Create database

#### To activate mongo: 
``` $ mongo ```

#### To display current database: 
``` $ db ```

#### For change particular database: 
``` $use <your_db_name> ```

#### Data structure: 
[references](https://github.com/ozlerhakan/mongodb-json-files/blob/master/datasets/books.json)
```
{
    "_id" : 1, 
    "title" : "Unlocking Android", 
    "isbn" : "1933988673", 
    "pageCount" : 416, 
    "publishedDate" : { 
        "$date" : "2009-04-01T00:00:00.000-0700"
    }, 
    "thumbnailUrl" : "https://s3.amazonaws.com/AKIAJC5RLADLUMVRPFDQ.book-thumb-images/ableson.jpg", 
    "shortDescription" : "Unlocking Android: A Developer's Guide provide [...]", 
    "longDescription" : "Android is an open source mobile phone platform [...]", 
    "status" : "PUBLISH", 
    "authors" : [ 
        "W. Frank Ableson", 
        "Charlie Collins", 
        "Robi Sen"
    ],
    "categories" : [ 
        "Open Source", 
        "Mobile" 
    ]
}
```

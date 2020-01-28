# mongo-db
Studies on mongo and mongo express.

## Instalation

#### Use the docker compose for build a workspace: 
``` docker-compose -f docker-compose.yml up -d ```

#### To access the container mongo: 
``` docker exec -it {container_id} /bin/bash  ```

#### To acess the mongo express: 
[http://localhost:8081/](http://localhost:8081/)

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

## Import database

#### To access the container mongo: 
``` docker exec -it {container_id} /bin/bash  ```

#### For import file:

``` 
$ mongoimport 
    --host 127.0.0.1:27017 
    -u root 
    -p root 
    --authenticationDatabase "admin" 
    -d students 
    -c students 
    --file data/db/students.json <--- file in volume
```

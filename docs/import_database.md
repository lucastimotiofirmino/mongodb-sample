# mongo-db
Studies on mongo and mongo express.

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

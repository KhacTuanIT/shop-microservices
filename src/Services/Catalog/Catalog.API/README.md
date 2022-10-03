## Install mongo on docker
### Pull image
```
docker pull mongo
```

### Create new image for mongodb on docker
``` 
docker run -d -p 27017:27017 --name shopping-mongo mongo
```

### Run mongo on docker /bin/bash
```
docker exec -it shopping-mongo /bin/bash
```

### To show mongo-cli
```
mongosh
```

## How to use command to interact with mongodb
### Show database list
```
show dbs
```

### Create new database in mongo
```
use [database_name]
```

### Create new Collection in database mongo
```
db.createCollection('Products')
```

### Insert many record into mongo database
```
db.Products.insertMany([{"Name": "Asus Laptop", "Category": "Computers", "Summary": "Summary", "Description": "Description", "ImageFile": "ImageFile", "Price": 54.93}, {"Name": "HP Laptop", "Category": "Computers", "Summary": "Summary", "Description": "Descriptioni", "ImageFile": "ImageFile", "Price": 88.93}])
```

### Query data from mongo database
```
db.Products.find({}).pretty()
```

### Remove data from mongo databse
```
db.Products.remove({})
```
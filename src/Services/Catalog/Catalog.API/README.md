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
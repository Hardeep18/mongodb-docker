# mongodb-docker-kube



```
cd docker-compose-replicaset
docker-compose up --build -d
```

```
docker exec -it <container name> /bin/bash

```

```
rs.initiate(
  {
    _id : 'rs0',
    members: [
      { _id : 0, host : "serverIP:27011" },
      { _id : 1, host : "serverIP:27012" },
      { _id : 2, host : "serverIP:27013" }
    ]
  }
)
```
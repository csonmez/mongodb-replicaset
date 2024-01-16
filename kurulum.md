```shell
docker exec -it mongodb1 mongo

rsconf = { _id : "rs0",members: [{"_id": 0,"host": "wn-mongodb1:27017","priority": 4},{"_id": 1,"host": "wn-mongodb2:27018","priority": 2},{"_id": 2,"host": "wn-mongodb3:27019","priority": 1 }]}

rs.initiate(rsconf); 
rs.conf() 
rs.secondaryOk() 
```

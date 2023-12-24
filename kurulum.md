```shell
docker exec -it mongodb1 mongo

rsconf = { _id : "rsmongo",members: [{"_id": 0,"host": "mongodb1:27017","priority": 4},{"_id": 1,"host": "mongodb2:27018","priority": 2},{"_id": 2,"host": "mongodb3:27019","priority": 1 }]}

rs.initiate(rsconf); 
rs.conf() 
rs.secondaryOk() 
```

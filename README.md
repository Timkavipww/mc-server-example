# HOW TO INIT

### Firstly, in folder data add your server with name "world" or edit it in file /data/server.properties
```level-name={world_name}```
### configure this file in your hands
### docker-compose 
### image: zg/minecraft-server:java8 <--- java8 is curruent verison of java you can edit it or use lasf of you can without this tag image: zg/minecraft-server

```
    environment:
      EULA: "TRUE"
      LEVEL: "world"
      TYPE: "FORGE"
      VERSION: "1.7.10"
      FORGEVERSION: "10.13.4.1614"
      MEMORY: "2G"
      ENABLE_RCON: "true"
      JVM_OPTS: -Dfml.queryResult=confirm
```
### all this environments can be editable

### to connect to your server cli
```bash
docker exec -i {mc-server} rcon-cli
```
### {mc-server} is container name

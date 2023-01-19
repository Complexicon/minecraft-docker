# minecraft-docker
launch commands for running minecraft in docker


```sh
# for minecraft >= 1.17
docker run -dit -p <port>:25565 -v $(pwd):/app -w /app -u $(id -u):$(id -g) --name <name> eclipse-temurin:17-jre-alpine java -jar spigot.jar

# for minecraft <= 1.16.5 
docker run -dit -p <port>:25565 -v $(pwd):/app -w /app -u $(id -u):$(id -g) --name <name> eclipse-temurin:8-jre-alpine java -jar spigot.jar
```

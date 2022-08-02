# Hello World Rest API

- Main class com.mailsonymathew.rest.webservices.restfulwebservices.RestfulWebServicesApplication 


### Creating Containers

- mvn clean package
- docker run --publish 8200:8080 mailsonymathew/aws-hello-world-rest-api:1.0.0-RELEASE

```
docker login
docker push @@REPO@@/aws-hello-world-rest-api:0.0.1-SNAPSHOT
```

## Test URLs

- http://localhost:8200/hello-world

```txt
Hello World
```

- http://localhost:8200/hello-world-bean

```json
{"message":"Hello World - Changed"}
```

- http://localhost:8200/hello-world/path-variable/tiger

```json
{"message":"Hello World, tiger"}
```

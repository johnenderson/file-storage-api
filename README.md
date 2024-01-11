# File Storage API

Servidor de armazenamento de arquivos utilizando Spring Boot.

## Tecnologias
 
- [Spring Boot](https://spring.io/projects/spring-boot)
- [Spring MVC](https://docs.spring.io/spring-framework/reference/web/webmvc.html)

## Como Executar

- Construir o projeto:
```
./mvnw clean package
```
- Executar:
```
java -jar ./target/file-storage-api-0.0.1-SNAPSHOT.jar
```

## Testando Apis

- Upload file:
```
curl -X POST -F "file=@path/to/your/file.txt" http://localhost:8080/api/files/upload
```
- Download file:
```
curl -OJL http://localhost:8080/api/files/download/your-file-name.txt
```
- List uploaded files:
```
curl http://localhost:8080/api/files/list
```
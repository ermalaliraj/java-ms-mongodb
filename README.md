# Campus Student Microservice

### Run Locally
1) Run MongoDB in local or change connection string to a remote instance 

2) Run MS CampusStudentApplication.

3) Call the API


### Microservice API

Run `CampusStudentApplication`, the service will be listen on the port `8085`
```
GET http://localhost:8085/students
GET http://localhost:8085/students?name=Er&surname=Al
GET http://localhost:8085/students/61e06f182f28bd1f82b5a0190

DELETE http://localhost:8085/students
DELETE http://localhost:8085/students/61e06f182f28bd1f82b5a0190

POST http://localhost:8085/students
{
    "name": "Ermal",
    "surname": "Aliraj",
    "registrationCode": "001"
}
```

### MongoDB

```
cd ./docker
docker-compose up -d
```

Connect from the client
```
mongodb://campus:campus@localhost:27017/?authSource=admin
```

### Links
- [Campus](https://github.com/ermalaliraj/campus)
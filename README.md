# Job Application Platform
Job-Application-Platform using Spring Framework(Spring Boot, Security, JPA) and React, Redux

* Rol based(Applicant and Human Resources) Authentication and Authorization with JSON Web Token.
* Create, and Delete and Job for only Human Resources user.
* Apply job for Applicant user
* File Upload an Download
* Secured routes both by client and server

### Technologies

The technologies used to develop this web app were diverse, the main ones being:

- Spring Framework(Spring Boot, Spring Security, Spring Data JPA)
- React
- SQL(Postgresql and H2)

### Installation
 
Clone and install server

```sh
$ git clone https://github.com/tayfurunal/Job-Application-Platform.git

$ cd hr-application-backend
$ mvn clean install or import IDE(Intellij IDEA etc.)
$ mvn spring-boot:run
```

Database Settings:

Default is H2 and you don't need configuration

if using Postgresql, Settings:

```sh
hr-application-backend > src > main > resources > application.properties

add the line

spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect

and Fill in the blanks

spring.datasource.url=
spring.datasource.username=
spring.datasource.password=
```

install client

```sh
$ cd hr-application-client
$ yarn
$ yarn start
```

### Usage

Human Resources
```sh
username: hradmin
password: hradmin
```

Applicant
```sh
username: tayfur
password: tayfur
```

Create new user with role on Postman:

- HR user => role:["HR"]
- APPLICANT user => role:["APPLICANT"]

![image](https://i.imgur.com/DD7tEsz.png)

### Screenshots

![image](https://i.imgur.com/MDOHVNL.png)

![image](https://i.imgur.com/7LBTRqO.png)

![image](https://i.imgur.com/Pt9MezI.png)

![image](https://i.imgur.com/QZlB6Qu.png)

# Strategic Imperatives
Recruitment Exercise:
https://docs.google.com/document/d/1unk6IzcIPpLmixiGunjV6u79JDU_zzfoxpp-pIrLcmM/edit

### Tech Stack:
| Technology | Version |
|--|--|
| **Java** | 11.0.3-2018-01-14 |
| **Spring Boot** | 2.5.0 |
| **Spring JPA Data** | 2.5.0 |
| **Project Lombok** | 1.18.20 |
| **JUnit 4** | 4.1.5 |
| **Mockito** | 2.0.9 |
| **OpenAPI** | 1.5.9 |
| **MySQL** | 8.0.20 |
| **Docker** | 20.10.4 |
| **EC2** |  |
| **RDS** |  |

### Acessing Swagger | Open API:
http://ec2-3-140-196-168.us-east-2.compute.amazonaws.com/swagger-ui/index.html?configUrl=/v3/api-docs/swagger-config

### Docker:
Exists a Dockerfile prepared to download a OpenJDK 11 Slim and install the application.

- Run the command: `docker build -t imperatives/exercise:release .`
- Run the command: `docker run -p port:port <IMG_ID>`
- Example: `docker run -p 8080:8080 8fb870f41548`
- Optionally download the image `docker pull samueldnc/samuelcatalano:imperatives`

### How To Run The Application:
> IDE (IntelliJ, Eclipse, NetBeans):
- Importing the project as Maven project on your favourite IDE.
- Build project using Java 11.
- Run/Debug project from Main Application Class :: ExerciseApplication.

> Terminal:
- `mvn spring-boot:run`


### APIs:

Basic URL path if you're runninh locally is: http://localhost:8080/  
Basic URL path if you're runninh locally is: http://ec2-3-140-196-168.us-east-2.compute.amazonaws.com/

#### Example:
* GET: http://ec2-3-140-196-168.us-east-2.compute.amazonaws.com/providers  
* GET: http://ec2-3-140-196-168.us-east-2.compute.amazonaws.com/providers/2  
* GET: http://ec2-3-140-196-168.us-east-2.compute.amazonaws.com/locations  
* GET: http://ec2-3-140-196-168.us-east-2.compute.amazonaws.com/locations/4  
* GET: http://ec2-3-140-196-168.us-east-2.compute.amazonaws.com/billings  
* GET: http://ec2-3-140-196-168.us-east-2.compute.amazonaws.com/billings/3

> For the **POST** and **PUT** APIs, see the open API documentation for a JSON body example.

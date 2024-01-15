
<h3 align="center">Spring-boot Rest API </h3>

<p> This documentation is both oriented to information to describe the functionalites of the projet and also oriented to understading, 
to explain the tools and models behind it in form of discursive and visual explanation. This documentation does not cover How-to guides or tutorials </p>

<div align="center">


</div>

---

## 📝 Table of Contents
- [About](#about)
- [Getting Started](#getting_started)
- [Functionalities](#functionalities)
- [Layout](#layout)
- [Documentation](#documentation)
- [Built Using](#built_using)
- [Tests](#tests)
- [Authors](#authors)


## 💻 About <a name = "about"></a>
 Voll.med is a fictional medical clinic that needs an application for appointment management. 
 The application should have features that allow the registration of doctors and patients, as well as scheduling and canceling appointments.

## 🏁 Getting Started and Installation <a name = "getting_started"></a>
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 
### IntelliJ IDEA

1. Open IntelliJ IDEA and select _File > Open..._.
2. Choose the java-maven-starter-project directory and click _OK_.
3. Select _File > Project Structure..._ and ensure that the Project SDK and language level are set to use Java 17.
4. Open the Maven view with _View > Tool Windows > Maven_.
5. In the Maven view, under _Plugins > dependency_, double-click the `dependency:unpack` goal. This will unpack the native libraries into $USER_HOME/.arcgis.
6. In the Maven view, run the `compile` phase under _Lifecycle_ and then the `exec:java` goal to run the app.

### Eclipse

1. Open Eclipse and select _File > Import_.
2. In the import wizard, choose _Maven > Existing Maven Projects_, then click _Next_.
3. Select the java-maven-starter-project as the project root directory.
4. Click _Finish_ to complete the import.
5. Select _Project > Properties_ . In _Java Build Path_, ensure that under the Libraries tab, _Modulepath_ is set to JRE System Library (JavaSE-11). In _Java Compiler_, ensure that the _Use compliance from execution environment 'JavaSE-11' on the 'Java Build Path'_ checkbox is selected.
6. Right-click the project in the Project Explorer or Package Explorer and choose _Run As > Maven Build..._. In the _Edit Configuration_ dialog, create a new configuration with name `unpack`. In the _Goals_ field, enter `dependency:unpack`. Click _Run_ to run the goal. This will unpack the native libraries into $USER_HOME/.arcgis.
7. Again, create a new run configuration with name `run`. In the _Goals_ field, enter `compile exec:java`. Click _Run_ to run the goal. The app should compile and launch the JavaFX window.

### Command Line

1. `cd` into the project's root directory.
2. Run `./mvnw dependency:unpack` on Linux/Mac or `mvnw.cmd dependency:unpack` on Windows to unpack the native libraries to $USER_HOME/.arcgis.
3. Run `./mvnw compile exec:java` on Linux/Mac or `mvnw.cmd compile exec:java` on Windows to run the app.

### Prerequisites
See the Java Maps SDK [system requirements](https://developers.arcgis.com/java/reference/system-requirements/).


## Functionalities <a name = "functionalities"></a>

- [x] CRUD de doctors;
- [x] CRUD de pacients;
- [x] Scheduling of appointments;
- [x] Canceling of appointments.

### 🎨 Layout <a name = "layout"></a>

The layout of the mobile application is available at this link: <a href="https://www.figma.com/file/N4CgpJqsg7gjbKuDmra3EV/Voll.med">Figma</a>

---

## 📄 Documentação <a name = "documentation"></a>

The documentation for this application can be accessed here: <a href="https://trello.com/b/O0lGCsKb/api-voll-med">Trello</a>

---

## 🔧 Running the tests <a name = "tests"></a>
On ``` /src/test ``` run selected package

### Break down into the tests
These tests ensure that the ConsultaController behaves correctly in different scenarios, handling both invalid and valid input. The use of Spring's testing annotations and features like @WithMockUser, @AutoConfigureMockMvc, and @AutoConfigureJsonTesters helps set up the necessary environment for testing Spring MVC controllers and JSON serialization, and also ensures that the MedicoRepository correctly queries the database and returns the expected results when checking the availability of doctors for consultations on specific dates and times.


## ⛏️ Built Using <a name = "built_using"></a>
- **[Java 17](https://www.oracle.com/java)**
- **[Spring Boot 3](https://spring.io/projects/spring-boot)**
- **[Maven](https://maven.apache.org)**
- **[MySQL](https://www.mysql.com)**
- **[Hibernate](https://hibernate.org)**
- **[Flyway](https://flywaydb.org)**
- **[Lombok](https://projectlombok.org)**

## ✍️ Authors <a name = "authors"></a>
- [@andredias]([https://github.com/kylelobo](https://github.com/andre-diass)) - Idea & Initial work


# Phoenix Automation Framework

- Java 11
- Maven 3.92
- TestNG 7.7
- Rest Assured


## Features

- Performs  API Automated Tests for both Inwarranty Flow 
- Integrated with Jenkins CI for Continious Testing for UI and API Component 
- Categorizing the Tests in  TestNG 
- Performs Parallel Testing and Isolated Tests


## Tech

Framework uses a number of dependencies to work properly:

- Selenium WebDriver
- TestNG
- Rest Assured
- JsonSchemaValidator
- Java-Faker
- Gson

## Adding New Dependencies

New Dependencies can be added in pom.xml at root level under dependencies tag

Example
```
<dependency>
			<groupId>io.rest-assured</groupId>
			<artifactId>rest-assured</artifactId>
			<version>5.1.1</version>
			<scope>test</scope>
		</dependency>
```



## Plugins

Maven Plugins used in the Project
<table>
  <tr><th>Plugin</th><th>README</th></tr>
  <tr><td>Maven SureFire Plugin- </td><td>https://maven.apache.org/surefire/maven-surefire-plugin </td></tr>
    <tr><td> Exec Maven Plugin -</td><td>https://www.mojohaus.org/exec-maven-plugin/ </td></tr>
</table>




### To Run the Automated Test for TestNG from cli...

```sh
mvn -Dexec.classpathScope=test  -Dexec.arguments="api,sanity" test-compile  exec:java -Dexec.cleanupDaemonThreads=false -X
```


ALlure report (recorded)

Logging log4j (recorded)

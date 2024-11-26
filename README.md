# qa-api-automation-
Requires Java and Maven versions openjdk 20  Apache Maven 3.9.1

    Install Java
    Install Maven

Install dependencies:

$ mvn clean install -DskipTests

Run tests
Cucumber tests

$ mvn test -Dtest=CukeRunner -Dcucumber.filter.tags=@<your-tag>

TestNG tests

$ mvn clean test -Dtest=<TestNG-Test-Class>
# Example:
$ mvn clean test -Dtest=CreateBookingApiTests

Reporting

# Install Allure for TestNG Allure reports and run below command after test exectuion:
$ allure serve
# Cucumber reports are generated with this file location: target/cucumber-report.html

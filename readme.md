# XSS Presentation #

A presentation and sample app on XSS defense and mitigation.

## [Getting started as a participant](readme-participant.md)

## [Getting started as a facilitator](readme-facilitator.md)

## Requirements ##
- Java 7
- Chrome
- Chrome Driver

## Setting up ##
- Make sure Java 8 is first on your classpath.
- Chrome Driver can be installed by brew with `brew install chromedriver`

## Running ##

### Running the Application ###
From the root directory `./gradlew xss-demo-app:run`

### Running the XSS Presentation ###
From the root directory open presentation/xss.html in your browser.

### Running the Test Suites ###
In order to get the tests to work, please edit your /etc/hosts file to contain the line
`127.0.0.1   example.com`

From the root directory:
- `./gradlew xss-demo-app:test` runs the unit tests
- `./gradlew xss-demo-app:intTest` runs the integration tests
- `./gradlew xss-demo-app:uaTest` runs the user acceptance tests
- `./gradlew xss-demo-app:appSecTest` runs the security tests

Hints for appSecTests:
[OWASP Injection Cheatsheet](https://www.owasp.org/index.php/Input_Validation_Cheat_Sheet)

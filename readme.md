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

### Fix XSS ###

1. Get your basic tests running

In order to get the tests to work, please edit your /etc/hosts file to contain the line at the end.
`127.0.0.1   example.com`

From the root directory:
- `./gradlew xss-demo-app:test` runs the unit tests
- `./gradlew xss-demo-app:intTest` runs the integration tests
- `./gradlew xss-demo-app:uaTest` runs the user acceptance tests

All these tests should pass.

2. Run the failing Application Security tests

`./gradlew xss-demo-app:appSecTest` runs the security tests

And now fix them! :)

Hints for appSecTests:
[OWASP Input Validation Cheatsheet](https://www.owasp.org/index.php/Input_Validation_Cheat_Sheet)
[OWASP XSS Prevention Cheatsheat](https://www.owasp.org/index.php/XSS_%28Cross_Site_Scripting%29_Prevention_Cheat_Sheet)

3. Remove the mapping to example.com from your /etc/hosts file

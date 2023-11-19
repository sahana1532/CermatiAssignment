# CermatiAssignment
ebay assignment
# Selenium Test(TDD framework) Script for eBay

## Overview
This project contains Selenium test scripts along with TDD framework to automate scenarios on eBay.

## Prerequisites
- [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/javase-downloads.html)
- [Eclipse IDE](https://www.eclipse.org/downloads/)
- [WebDriverManager](https://github.com/bonigarcia/webdrivermanager)
- [Selenium WebDriver](https://www.selenium.dev/downloads/)
- [TestNG](https://testng.org/doc/download.html)

## Setup
1. Install Java and set up the `JAVA_HOME` environment variable.
2. Download and install Eclipse IDE.
3. Create a new Java project in Eclipse.
4. Add WebDriverManager, Selenium WebDriver, and TestNG dependencies to your project.

    ```xml
    <!-- WebDriverManager -->
    <dependency>
        <groupId>io.github.bonigarcia</groupId>
        <artifactId>webdrivermanager</artifactId>
        <version>5.0.3</version>
    </dependency>

    <!-- Selenium WebDriver -->
    <dependency>
        <groupId>org.seleniumhq.selenium</groupId>
        <artifactId>selenium-java</artifactId>
        <version>3.141.59</version>
    </dependency>

    <!-- TestNG -->
    <dependency>
        <groupId>org.testng</groupId>
        <artifactId>testng</artifactId>
        <version>7.4.0</version>
    </dependency>
    ```

5. Install TestNG plugin for Eclipse.

6. Test Execution
* Open Eclipse and import the project.
* Run `testng.xml` as a TestNG suite to execute both scenarios.

## Scenarios
### Scenario 1: Access a Product via category after applying multiple filters
- Navigate to eBay.com
- Navigate to Search by category > Electronics > Cell Phones & accessories
- Click Cell Phones & Smartphones
- Click All Filters
- Add 3 filters - Condition, Price, and Item location
- Click Apply
- Verify that the filter tags are applied.

### Scenario 2: Access a Product via Search
- Navigate to eBay.com
- Type a search string in the search bar (e.g., MacBook)
- Change the Search category (e.g., Computers/Tablets & Networking) and click Search
- Verify that the page loads completely
- Verify that the first result name matches the search string.

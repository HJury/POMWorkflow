## POMWorkflow repository

This project shows the test automation workflow using **POM** as a framework and adding a new layer took from **Screenplay**.

![Maven Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0b/Maven_logo.svg/340px-Maven_logo.svg.png) ![Selenium Logo](https://github.com/HJury/ReadmePictures/blob/master/Selenium.png) ![Cucumber Logo](https://github.com/HJury/ReadmePictures/blob/master/Cucumber.png) ![TestNG Logo](https://github.com/HJury/ReadmePictures/blob/master/TestNG.png)

Currently, this project allows its integration to a **CD** or **CI** cycle, recognize the current OS and using different configuration parameter in order to run in both Windows and Linux machines, in this case, the tool that was used for the **CI** and **CD** was **circleCi**.

In order to run your tests, you will need: 

* Java 1.8

![Java Logo](https://github.com/HJury/ReadmePictures/blob/master/Java.png) 

* Chrome 83.0.4103.xx

![Cucumber Logo](https://github.com/HJury/ReadmePictures/blob/master/Chrome.png)

#Running the tests

For the tests to be executed all the new scenario within the features should have the tag **"@EXECUTE"** and you should enter the command: 
      `mvn test` in order to run the scenarios within the features.
      
The former command will run the tests and generates a report using the ExtentReports library, this report will keep the gherkin syntax of the scenarios as well as the respective result of each one. The report will be generated on the directory: `../test-output/HtmlReport/AutomationExtentHtml.html`

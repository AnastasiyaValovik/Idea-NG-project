# Automation framework for testing microservice 'Идея' of 'NordGold' project
___
## About Testing Framework

The testing framework was created for [TEST environment](https://hr-services-stg.nordgold.com) of microservice 'Идея' of the 'NordGold' project. 

This framework based on Cypress. It's an E2E testing tool based on JavaScript. To learn more about Cypress, read its [documentation](https://cypress.io/).

## How to navigate in the Project
To find test specs in the project open 'cypress/e2e/..'.  Specs are named by the name of testing page or functionality.

To find methods used in tests, open 'cypress/support/PageObjects/..'.  PageObject files are named according to the pages or elements of pages it was created for.


## Requirements before using project
    Node.js should be installed on your machine (above the 14 version).

    NPM should be installed on your machine. To upload the latest version, run in the terminal :

    npm install npm@latest -g
    
## Installation
    Download project or clone repository. Run the following commands in the root folder of the project:

    npm install
    npm install cypress --save-dev

## Run tests in browser 
    cypress open
    (or) npx cypress open

 
## Run tests in terminal
#### Run all tests:
    cypress run
    (or) npx cypress run

#### Run specific spec file:
    cypress run --spec 'cypress/e2e/nameOfSpec'

####
#### Run tests in specific browser
    cypress run --browser 'browserName'


## Reports and tracking failed tests 
#### Mochawesome reports 
    The Mochawesome report generates after each test run. 

    Go to 'cypress/mochawesome-report/..' and open html file.


#### Default Cypress functionality to catch failures and help with debugging process

    Cypress makes screenshots of failed tests for last tests run. To check it, open 'cyress/screenshots/..'
    
    Cypress makes video of every last test run. To check it, open 'cypress/videos/..'

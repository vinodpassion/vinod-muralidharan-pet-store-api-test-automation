# Test Framework

This Automation testing framework primarily uses **Jest** as test runner and below are the support modules:

  - got - http lib
  - jest-html-reporter - to create html report


## Installation
### Prerequisite 

- Requires [Node.js](https://nodejs.org/) to run.
- Require Yarn for package manager (npm install -g yarn)

### Setup

Install the dependencies and devDependencies

```sh
$ yarn
```

### Code Quality

To check the code written follows javascript and es6 convention

```sh
$ yarn lint
```


### Running Test

```sh
$ yarn test
```
To Run a specific test file, example:

```sh
$ yarn test ./src/test/store.api.test.js
```

### Report
Once test is run, the result will be reported in console and also as HTML reporter in "output/report" folder

## Approach:
All the automated testcases reside in “src/test”. I have added 3 different test files for services such as pet, user and store respectively. 

## About tech stack:
- I have used nodejs from the programming language as it is comfortable language for me and in comparison to java it is lighter and has my modern library supporting nodejs. 
- I have used Jest as test runner. Simply because it is easily configurable and it provides lots of inbuild features such as assertion lib support, configuration support and reporting
- I have used jest html reporter, you can find the report generated in “./output/report” folder
- I have used Winston as logging library 

## Test cases
| S.No | Service | Test cases Automated                        |
|------|---------|---------------------------------------------|
| 1    | Pet     | Verify find pet by valid status = available |
| 2    |         | Verify find pet by valid status = pending   |
| 3    |         | Verify find pet by valid status = sold      |
| 4    |         | Verify find pet by tag = tag1               |
| 5    |         | Verify find pet by tag = tag2               |
| 6    |         | Verify find pet by tag = tag3               |
| 7    |         | Verify find pet by id = 1                   |
| 8    |         | Verify find pet by id = 2                   |
| 9    |         | Verify find pet by id = 3                   |
| 10   |         | Verify updating pet information             |
| 11   |         | Verify creating new pet information         |
| 12   |         | Verify posting pet using form data          |
| 13   |         | Verify deleting a pet                       |
| 14   |         | Verify upload image of pet                  |
| 15   | Order   | Verify get inventory function               |
| 16   |         | Verify add new order function               |
| 17   |         | Verify get order function                   |
| 18   |         | Verify delete order function                |
| 19   |         | Verify user creation function               |
| 20   | User    | Verify create users with list function      |
| 21   |         | Verify successful login                     |
| 22   |         | Verify successful logout                    |
| 23   |         | Verify get user information                 |
| 24   |         | Verify update user information              |
| 25   |         | Verify delete user                          |

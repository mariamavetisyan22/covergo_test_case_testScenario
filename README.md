# covergo_test_case_test_scenario


The task of CoverGO, includes test cases written in Gherkin language and in a standard template, and bug reports of the login page.////

- This is the test documentation of the task [GoverGo](https://www.example.com) which includes a test document file of the Sign Up/Login pages, you can find the test cases and bug reports, also test environment parameters, requirements, and possible test scenarios, test data (in one table for easy use).

  There are the scenarios of the documented file.
- The [Geex-Arts Test Cases.md](https://github.com/mariamavetisyan22/eyeb-web-test-case-bug-report-task/blob/main/Geex-Arts%20Test%20Cases.md) file indicates test cases for the following scenarios.
  
  1. Check Sign Up using a valid email.
  2. Check Sign Up using a valid phone.
  3. Check Sign Up using a Google Account.
  4. Check Sign In using a valid existing phone/email.

## **Test Objective**
 
Testing the page [Geex-Arts](https://eyeb-web-git-dev-eyeb.vercel.app/feed) aims to ensure that all the essential functionalities and features work as intended and provide a seamless user experience during the sign-up and login process.

## **Test Environment**
Parameters | Values | 
--- | --- |
Operating System | Windows 11 Home, 22H2, 22621.1928 |
Browser | Chrome: 114.0.5735.199 (Official Build) (64-bit) |
Screen Resolution | 1920x1080 pixels |

## **Requirements**

- **Password:** field must be filled with English alphabet letters and include three character types: lowercase letters, uppercase letters and numbers. You also have the option to use any of these special characters: # [ ] ( ) @ $ & * ! ? | , . ^ / \ + _ -
   - At least 8 characters
   - At least one uppercase letter (ABC...)
   - At least one lowercase letter (abc...)
   - At least one number (123...)


## **Test Data**
#### _Valid Test Data_
  - **Email:** mar.test.avetis@gmail.com
  - **Phone** +13022814650;
  - **Password:** Testuser1!;
#### _Invalid Test Data_
  - **Email:** m@mailinator.com; test#gmail.com; test
  - **Phone** +3197010526431;
  - **Password:** test; 123; !"£$; TEST; 

## **Test Execution Results**

- The [Geex-Arts Bug Reports.md](https://github.com/mariamavetisyan22/eyeb-web-test-case-bug-report-task/blob/main/Geex-Arts%20Bug%20Reports.md) file indicates buf reports found bugs of introduced test scenarios.

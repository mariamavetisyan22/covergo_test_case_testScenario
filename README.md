# covergo_test_case_test_scenario


The task of CoverGO, includes test cases written in Gherkin language and in a standard template, and bug reports of the login page.

- This is the compact test document file of the tested page, you can find the test environment parameters, requirements, test scenarios, test data (in one table for easy use), test cases, and bug report(s).

  There are the scenarios of the documented file written in _**Gherkin language**_.
- The [GoverGo](https://www.example.com) file indicates test cases for the following scenarios.
  
## **Test Scenarios**
#### Feature: User Login

As a registered user  
I want to be able to log in  
So that I can access my account  

#### Scenario: Successful login with valid username and password

_Given_ I am on the login page  
_When_ I enter valid credentials (username and password)  
_And_ I click the login button  
_Then_ I should be redirected to the home page  
_And_ I should successfully log in with my credentials  

#### Scenario: Unsuccessful login with invalid username and password

_Given_ I am on the login page  
_When_ I enter an invalid username  
_And_ I enter an invalid password  
_And_ I click the login button  
_Then_ I should see an error message "Invalid username or password"  

#### Scenario: Unsuccessful login with a valid username and invalid password

_Given_ I am on the login page  
_When_ I enter a valid username  
_And_ I enter an invalid password  
_And_ I click the login button  
_Then_ I should see an error message "Invalid username or password"  

#### Scenario: Unsuccessful login with unknown username (not authorized)

_Given_ I am on the login page  
_When_ I enter an unknown username  
_And_ I enter a password  
_And_ I click the login button  
_Then_ I should see an error message "Username not found"  

#### Scenario: Unsuccessful login without entries (username and password)

_Given_ I am on the login page  
_When_ I click the login button without entering credentials  
_Then_ I should see an error message "Missing username and password"  

#### Scenario: Successful login for users with account balance over $100

_Given_ I am on the login page  
_When_ I enter a valid username with an account balance over $100  
_And_ I enter a valid password  
_And_ I click the login button  
_Then_ I should be redirected to the home page  
_And_ I should see an ad on the page  


## **Test Objective**
 
The objective of testing the page is to ensure that all the key functionalities and features work as intended and provide a seamless user experience during the registration process.

## **Test Environment**
Parameters | Values | 
--- | --- |
Operating System | Windows 11 Home, 22H2, 22621.1992 |
Browser | Chrome: 115.0.5790.102 (Official Build) (64-bit) |
Screen Resolution | 1920x1080 pixels |

## **Requirements**

- **Username:** The field should allow only entered login containing lower letters and numbers without space. 
- **Password:** The field must be filled with English alphabet letters and include three character types: lowercase letters, uppercase letters, and numbers. You also have the option to use any of these special     - At least 8 characters
   - At least one uppercase letter (ABC...)
   - At least one lowercase letter (abc...)
   - At least one number (123...)


## **Test Data**
#### _Valid Test Data_
  - **UserName/Password:**
    - validuser/Validuser1!
    - memberuser/Memberuser2@
    - handleruser/Handleruser3#
    - userwithbalance/Validuser1! (user with 100$ on account balance)
    - admin/Admin1234!

#### _Invalid Test Data_
  - **UserName/Password:**
    - empty fields
    - invaliduser/invaliduser (the user who isn’t authorized)
    - User12!@/User12!@
    - user/user
    - 123/123
    - !”£$%^/”£$£$£
    - userwithoutpermissions/Perms123# (a user who hasn’t any permissions)

## **Test Execution Results**
Parameters | Values | 
--- | --- |
**Total** | **$${\color{black}8}$$** |
Passed | $${\color{green}3}$$ |
Failed | $${\color{red}5}$$ |

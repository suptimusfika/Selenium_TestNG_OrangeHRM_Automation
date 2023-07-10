![image](https://github.com/suptimusfika/Selenium_TestNG_OrangeHRM_Automation/assets/48064134/e3ad512e-e9c9-45c3-b9f9-5e3571076760)# Selenium_TestNG_OrangeHRM_Automation
I have created a selenium testNG project for automating OrangeHRM website and asserting the expected message after successfull activities.

## Scenario
- Login as a admin to https://opensource-demo.orangehrmlive.com/
- Go to PIM menu and create a new employee. Save the employee firstname, lastname, employeeid, username and password into JSONArray file. Generate random password which meets following criteria:
For a strong password, please use a hard to guess combination of text with upper and lower case characters, symbols and numbers. Assert if employee is created successfully.

- Now go to the dashboard again and search by the employee id to check if the employee is found
- Now go to the Directory menu and search by employee name and check if the employee is found
- Logout the session.
- Now login with the newly created employee creds
- Assert your full name is showing besides the profile icon.
- Go to my info
- Scroll down and select Gender and Blood Type as O+ and save it. Then logout the user.
- Create a smoke suite configuration which will run only following features (positive cases only):

    - Login to admin
    - search by the employee id if found
    - logout admin and login to the employee id you created last
    - Update the blood Group as AB-
    - Logout the user
 
## How to run this project
- clone this project
- To run Master suite (regression testing) hit this command ```gradle clean test -PsuiteFile="MasterSuite.xml"```
- To run SmokeMaster suite (smoke testing) hit this command ```gradle clean test -PsuiteFile="SmokeMasterSuite.xml"```
- To generate allure report hit these command  
  ```allure generate allure-results --clean -output```  
  ```allure serve allure-results```

## Test Cases
https://docs.google.com/spreadsheets/d/1Fx1iinGV8W9k7XcMf4buPH9NmLR50T4GVCwwjjAB72I/edit?usp=sharing

## Tools Used
- Intellij
- Jdk-11
- Selenium
- Allure
  
## Framework used:
- TestNG

## Video Recording of automation output:
https://github.com/suptimusfika/Selenium_TestNG_OrangeHRM_Automation/assets/48064134/2d6a6c99-3087-4cc5-b9c6-e1cf9024ac04

## Allure Report Image: 
![1](https://github.com/suptimusfika/Selenium_TestNG_OrangeHRM_Automation/assets/48064134/6d7e6472-a83d-44ef-be56-13ca33091f40)

![2](https://github.com/suptimusfika/Selenium_TestNG_OrangeHRM_Automation/assets/48064134/f4997108-81b8-43c5-a4a2-3094d1a258cc)

## Test Summary: 
![3](https://github.com/suptimusfika/Selenium_TestNG_OrangeHRM_Automation/assets/48064134/f283a6a6-4ebd-499e-bace-e6eb8fd23d01)


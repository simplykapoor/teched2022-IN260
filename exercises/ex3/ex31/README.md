# Exercise 3.1 - Add a new employee

In this exercise, you will be adding a new employee in the SuccessFactors demo instance.
Please do note that this instance has been provided only for the TechEd exercise. 
A SAP partner can request for demo system via [link](https://hxmcloudops.successfactors.com/home/index)

Login details of the SAP SuccessFactors system will be provided in the Document available as part of the prebuilt integration package *Teched 2022 IN260 - SOL* in SAP Integration Suite.

## Exercise steps

Run through the following steps
1. Search for ADD NEW EMPLOYEE and select *Add New Employee* action listed
<br><img src="/exercises/ex3/images/img1.jpg" width=50% height=50%>

<br>2. In *Identity* section, enter details as given below:

<br> Hire Date: Change it to any date of preference.

Company: Select anyone from the drop down list available. Eg: BestRun(10000)

Event Reason: New Hire (HIRNEW)

First Name and Last Name can be any information.

Date of Birth: Select any date. Eg: Apr 04, 2000

Country of Birth : Enter any country. Eg: United States

Person Id: Enter the same as the topic name created in Confluent Kafka (IN260_XX, where XX is the participant number assigned to you)

User Name: same as Person Id.
<br><img src="/exercises/ex3/images/img2.jpg" width=50% height=50%>

<br>3. Select Continue. 

Note: A duplicate check dialog box may appear. Click on ignore matches.

<br>4. In *Personal Information* section, enter details as given below:

Gender: select either male or female

Preferred Language: Select any, eg: English(US)

Nationality: Select any, eg: United States

Email Information: 

a. Email Type: Select *Business*

b. Email Address: Enter any email id that you can access to see the mail generated as part of employee onboarding in SAP SuccessFactors

c. isPrimary: Select *Yes*
<br><img src="/exercises/ex3/images/img3.jpg" width=50% height=50%>

<br>5. Select Continue. 

<br>6. In *Job Information* section, enter details as given below:

Select Position: any one from the drop-down

In Organizational Information, select *No data* as Cost Center from the drop down

In Employment Details, set the First Date Worked

<br>7. Select Continue

<br>8. Select Submit


    


## Summary

You should have been able to onboard a new employee successfully in SAP SuccessFactors

Continue to - [Exercise 3.2](/exercises/ex3/ex32)

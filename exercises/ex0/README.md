# Create Kafka topic

As a prerequisite to run through the exercises, you need to create an own topic in Kafka. 
A topic is a log of events. For this hands-on you will be publishing SuccessFactors New Hire event to Kafka topics and real-time integrations will be triggered to inform as well as guide the newly onboarded employee and the hiring manager on next steps.

## Exercise steps

Run through the following steps
1. Logon to the Kafka environment **https://confluent.cloud/login/sso/sap-is-ias** with the user **userXX** with **XX** the participant number assigned to you and the password provided to you

    <br><img src="/exercises/ex0/images/00-0001.png" width=80% height=80%>

2. In some cases, you may get the following questionaire screen. If not, proceed to exercise step **4**. Otherwise, select link *Skip* from the upper right of the screen

    <br><img src="/exercises/ex0/images/00-0001a.png" width=80% height=80%>

3. On the next screen, either collapse the getting started section or select the *Leave tutorial* link to get the getting started section closed

    <br><img src="/exercises/ex0/images/00-0001b.png" width=80% height=80%>

4. Switch to the *Environments* page and select the *default* environment

    <br><img src="/exercises/ex0/images/00-0005.png" width=80% height=80%>

5. In the *Teched2022_IN260* cluster, select the *Topics* link to navigate to the topics

    <br><img src="/exercises/ex0/images/00-0006.png" width=50% height=50%>

6. In the *Topics* page, create a new topic by selecting the *Add topic* button

    <br><img src="/exercises/ex0/images/00-0007.png" width=80% height=80%>

7. Maintain the Topic name **IN260_XX** with **XX** the participant number assigned to you
8. When done, select the *Create with defaults* button

    <br><img src="/exercises/ex0/images/00-0009.png" width=80% height=80%>

9. The new topic should have been created. If you navigate back, you should see the new topic in the list of topics

    <br><img src="/exercises/ex0/images/00-0011.png" width=80% height=80%>

## Summary

You should have created a new topic.

Now, we start creating the first integration flow subscribing to this topic. Continue to - [Exercise 1](/exercises/ex1)

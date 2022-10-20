# Exercise 4.1 - Produce message using Confluent Kafka

In the following exercise, you will replay this New Hire event using Confluent Kafka.

While you have so far observed the scenario execution end-to-end, there may be cases where the sender application may have resent the message multiple times, and from the execution point of view you want to control and ensure that the message is processed at the receiver system exactly once. This exercise will focus on how exactly-once scenario gets handled by SAP Integration Suite - Cloud Integration capability

## Exercise steps

Run through the following steps
1. Login to [Confluent Kafka](https://confluent.cloud/login/sso/sap-is-ias)

2. Access the topic you had created earlier - **IN260_XX** with **XX** the participant number assigned to you

3. Open *Messages* in the topic

4. Select the option to *Produce a new message to this topic*

    <br><img src="/exercises/ex3/images/img318.jpg" width=70%>
    
5. In the text space provided, replace the value on the screen with the message payload previously copied into your notepad or downloaded from monitoring view in [Exercise 3.3](/exercises/ex3/ex33)

    <br><img src="/exercises/ex4/images/img401.png" width=90%>

6. Click *Produce*. 


## Summary

You should have replayed the hire event with this exercise

Continue to - [Exercise 4.2](/exercises/ex4/ex42)

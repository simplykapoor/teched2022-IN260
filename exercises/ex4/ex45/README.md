# [Optional] Exercise 4.5 - Reproduce event with trace switched on

This exercise is optional. You may rerun the message event with tracing the message processing in Cloud Integration to better understand the exactly once delivery behaviour.

## Exercise steps

Run through the following steps
1. Let's first swich on the trace before rerunning the scenario. Select *Monitor -> Integrations* from the left navigation pane, and click on the *All* tile below the *Manage Integration Content* section

    <br><img src="/exercises/ex4/images/img404.png" width=50%>

2. Select your integration flow **SAP SFSF New Hire Onboarding Process Automation using SPA - XX** with **XX** the participant number assigned to you, and change the Log Level to *Trace* 

    <br><img src="/exercises/ex4/images/img405.png" width=80%> 

3.  Confirm the upcoming dialog by selecting *Change* 

    <br><img src="/exercises/ex4/images/img406.png" width=40%> 

4.  The trace will be switched on for 10 minutes

    <br><img src="/exercises/ex4/images/img407.png" width=100%> 

5.  Like you did before, replay the event by producing a new message in your Kafka topic, see [Exercise 4.1](/exercises/ex4/ex41)
5.  Once the message has been reproduced, enter the Cloud Integration monitor again, adn from your *Trace* 

    <br><img src="/exercises/ex4/images/img408.png" width=100%> 

6.  to *Trace* 

    <br><img src="/exercises/ex4/images/img409.png" width=100%> 

7.  to *Trace* 

    <br><img src="/exercises/ex4/images/img410.png" width=100%> 

8.  to *Trace* 

    <br><img src="/exercises/ex4/images/img411.png" width=100%> 

## Summary

Continue to - [Exercise 4.3](/exercises/ex4/ex43)
Congratulations, this concludes the overall exercise. Navigate back to - [Exercise overview page](/README.md)

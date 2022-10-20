# Exercise 4.2 - Monitor messages in Cloud Integration

In the following, you will be redoing the steps that you are already familiarized with [Exercise 3.3](/exercises/ex3/ex33). You may observe some changes in the experience though.

## Exercise steps

Run through the following steps
1. Select the *Monitor -> Integrations* from the left navigation pane, and click on the tile to look at *All Integration Flows*

    <br><img src="/exercises/ex4/images/img402.png" width=60%>

2. Filter through the multiple messages that could have been processed in the last one hour, you can use the employee ID of the new hire, i.e., **IN260_XX** where **XX** is the participant number assigned to you. You should see two new messages which have been processed

    <br><img src="/exercises/ex4/images/img403.png" width=100%> 

    **Note**: Both the integration flows which subscribe to the event topic in Kafka should have been retriggered with this replay of New Hire event. If the status is not reflecting as completed, please contact one of the hands-on session moderator.

## Summary

Continue to - [Exercise 4.3](/exercises/ex4/ex43)

# Exercise 4.2 - Monitor messages in Cloud Integration

In the following, you will be redoing the steps that you are already familiarized with [Exercise 3.3](/exercises/ex3/ex33). You may observe some changes in the experience though.

## Exercise steps

Run through the following steps
1. Select the *Monitor -> Integrations* from the left navigation pane.
    <br><img src="/exercises/ex3/images/img310.jpg" width=30% height=30%>

2. You can see the multiple tiles that provides rich variety of monitoring options. For this exercise we will monitor messages that have been processed. Click on the tile to look at *All Integration Flows*.

    <br><img src="/exercises/ex3/images/img311.jpg" width=50% height=50%>

3. In this view, you can filter integrations that are deployed by you by using the ID field. 

Here, to filter through the multiple messages that could have been processed in the last one hour, you can use the topic name created in Confluent Kafka (IN260_XX, where XX is the participant number assigned to you). 
    <br><img src="/exercises/ex3/images/img319.jpg" width=50% height=50%>
    
Note: Both the integration flows which subscribe to the event topic in Kafka should have been retriggered with this replay of New Hire event. If the status is not reflecting as completed, please contact one of the hands-on session moderator.

## Summary

Continue to - [Exercise 4.3](/exercises/ex4/ex43)

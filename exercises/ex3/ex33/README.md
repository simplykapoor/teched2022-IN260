# Exercise 3.3 - Monitor in Cloud Integration

In the following exercise, you will be able to monitor integrations. 

## Exercise steps

Run through the following steps
1. Select the *Monitor -> Integrations* from the left navigation pane. (Hint: By clicking on the burger icon on the top left corner, you can expand the navigation pane.)
    <br><img src="/exercises/ex3/images/img310.jpg" width=30% height=30%>

2. You can see the multiple tiles that provides rich variety of monitoring options. For this exercise we will monitor messages that have been processed. Click on the tile to look at *All Integration Flows*.

    <br><img src="/exercises/ex3/images/img311.jpg" width=50% height=50%>

3. In this view, you can filter integrations that are deployed by you by using the ID field. 

Here, to filter through the multiple messages that could have been processed in the last one hour, you can use the topic name created in Confluent Kafka (IN260_XX, where XX is the participant number assigned to you). (Additional information: This is possible due to the message mapping step explained in [Excercise 2.4](/exercises/ex2/ex24) where an SAP_ApplicationID header is set)
    <br><img src="/exercises/ex3/images/img312.jpg" width=50% height=50%>
    
Note: If the status is not reflecting as completed across the three integration flows, please contact one of the hands-on session moderator.

4. Select the *Publish SAP SFSF New Hire Event to Confluent Kafka - SOL* Integration Flow 

5. Navigate to *Attachments* section. 

    <br><img src="/exercises/ex3/images/img316.jpg" width=50% height=50%>
 
6. Click to view the *Payload*

7. Either copy this payload into a notepad (Hint: CtrlA to select the full text works in this text view) or download the payload (.txt file). This step is necessary for the Exercise 4 - *Replay the Hire Event to check exactly once scenario execution*.

    <br><img src="/exercises/ex3/images/img317.jpg" width=50% height=50%>
    

## Summary

You should have now some familiarity with the standard monitoring that is availble as part of SAP Integration Suite. 

In addition, this following blog [Monitoring tools for Cloud Integration Capability of SAP Integration Suite](https://blogs.sap.com/2021/10/28/monitoring-tools-for-cloud-integration-capability-of-sap-integration-suite/) will be of interest to participants who want to learn more about this topic and how SAP supports monitoring. 

Continue to - [Exercise 3.3](/exercises/ex3/ex34)

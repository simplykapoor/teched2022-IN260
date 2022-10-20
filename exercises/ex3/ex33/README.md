# Exercise 3.3 - Monitor in Cloud Integration

In the following exercise, you will be able to monitor integrations. 

## Exercise steps

Run through the following steps
1. Open the SAP Integration Suite landing page, and select *Monitor -> Integrations* from the left navigation pane. (**Hint**: By clicking on the burger icon on the top left corner, you can expand the navigation pane.)

    <br><img src="/exercises/ex3/images/img310.jpg" width=25%>

2. You can see the multiple tiles providing a rich variety of monitoring options. For this exercise we will monitor messages that have been processed. Click on the tile to look at *All Integration Flows*

    <br><img src="/exercises/ex3/images/img311.png" width=70%>

3. In this view, you can filter integrations that are deployed by you by using the ID field. Here, to filter through the multiple messages that could have been processed in the last one hour, you can use the employee ID of the new hire, i.e., **IN260_XX**, where **XX** is the participant number assigned to you. (**Additional information**: This is possible due to the message mapping step explained in [Excercise 2.4](/exercises/ex2/ex24) where an *SAP_ApplicationID* header is set)

    <br><img src="/exercises/ex3/images/img312.png" width=100%>
    
    **Note**: If the status is not reflecting as completed across the three integration flows, please contact one of the hands-on session moderators

4. Let's copy the payload of the event. Note, this step is necessary for *Exercise 4* where we replay the event to check the exactly once scenario execution
    1. Select the *Publish SAP SFSF New Hire Event to Confluent Kafka - SOL* integration flow
    2. Navigate to the *Attachments* section
    3. Click to view the *Payload*
    
    <br><img src="/exercises/ex3/images/img316.png" width=100%>
 
5. Either copy this payload into a notepad (**Hint**: Ctrl-A to select the full text works in this text view) or download the payload (.txt file)

    <br><img src="/exercises/ex3/images/img317.png" width=60%>

## Summary

You should have now some familiarity with the standard monitoring that is availble as part of SAP Integration Suite. 

In addition, this following blog [Monitoring tools for Cloud Integration Capability of SAP Integration Suite](https://blogs.sap.com/2021/10/28/monitoring-tools-for-cloud-integration-capability-of-sap-integration-suite/) will be of interest to participants who want to learn more about this topic and how SAP supports monitoring. 

Continue to - [Exercise 3.3](/exercises/ex3/ex34)

# Integration Flow to publish events to Kafka

In order to publish the event to your Kafka topic once the new hire has been created, we have provided and deployed an integration flow on the Cloud Integration tenant. In order to better understand the overall integration scenario, let's quickly go through the integration flow model.

**Note**: This chapter is for information only, there is no configuration from your side required.

## Integration flow model

The integration flow consists of the following steps:
1. Events from SAP SuccessFactors are sent to the HTTP end point of the integration flow
2. For monitoring purposes, the Groovy script *Log New Hire Event Payload* adds the event payload as attachment to the Message Processing Log
3. The first content modifier step *Save Original JSON Payload* stores the original JSON payload of the event in an exchange property
4. Next, the converter step *JSON to XML Converter* converts the JSON message into XML format since this is more covenient to fetch data from the message body
5. In the second content modifier step *Extract Employee ID as Topic Name and set JSON payload*, the following settings are done:
    1. The employee ID is fetched via an xpath expression from the XML payload and stored in the exchange property *topicName*
    2. The employee ID is also stored in the *SAP_ApplicationID* header. This allows us to search for the messages in the message monitor based on payload data, see [Use Custom Header Properties to Search for Message Processing Logs](https://help.sap.com/docs/CLOUD_INTEGRATION/368c481cd6954bdfa5d0435479fd4eaf/d4b5839670ce4866a770f7cadac063db.html)
    3. Furthermore, the original JSON payload is written back into the message body to ensure that the original event content is posted to the Kafka topic
6. Finally, the event is written into a Kafka topic using the Kafka adapter whereas the topic name is dynamically defined based on the exchange property *topicName* holding the employee ID

<br><img src="/intro/images/intro-03-0001.png">

Now that you have gone through all introduction chapters, you should have a clear picture of the overall integration scenario, and could start with the actual exercises.

Navigate back to - [Exercise overview page](/README.md)

# Integration Flow to publish events to Kafka

In order to publish the event to your Kafka topic once the new hire has been created, we have provided and deployed an integration flow on the Cloud Integration tenant. In order to better understand the overall integration scenario, let's quickly go through the integration flow model.

**Note**: This chapter is for information only, there is no configuration from your side required.

## Integration flow model

The integration flow consists of the following steps:
1. Events from SAP SuccessFactors are sent to the HTTP end point of the integration flow
2. In the first content modifier step, the original payload of the event in JSON format is kept in an exchange property
3. Next, the JSON message is converted into XML format since this is more covenient to fetch data from the message body
4. In the second content modifier, the employee ID is fetched via an xpath expression from the XML payload and stored in an exchange property. Furthermore, the original JSON payload is written back into the message body to ensure that the original event content is posted to the Kafka topic
5. Finally, the event is written into a Kafka topic using the Kafka adapter whereas the topic name is dynamically defined based on the exchange property holding the employee ID

    <br><img src="/intro/images/intro-03-0001.png">

Now that you have gone through all introduction chapters, you should have a clear picture of the overall integration scenario, and could start with the actual exercises.

Navigate back to - [Exercise overview page](/README.md)

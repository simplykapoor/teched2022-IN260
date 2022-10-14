# Exercise 2.2 - Maintain the connection to your Kafka topic

Now that we have created the integration flow stub in the previous exercise, we will start with modeling the integration flow steps by maintaining the sender adapter of type Kafka to connect to your Kafka topic.

## Exercise steps

Run through the following steps

1. If you select the *Sender* component, the quick menu appears. From the quick menu, select the *Connector* icon ...

    <br><img src="/exercises/ex2/images/02-0009a.png" width=30%>

2. ... and drag it on the *Start Message* event

    <br><img src="/exercises/ex2/images/02-0010.png" width=35%>

3. A dialog comes up where you need to select the adapter type. In our case, select the entry *Kafka*

    <br><img src="/exercises/ex2/images/02-0011.png" width=50%>

4. In the properties of the Kafka connection, switch to tab *Connection*
5. In the *HOST DETAILS* section, select the *Add* button
6. Maintain the host and port of the Confluent Kafka system provided to you by the instructors
7. Finally, as Credential Name enter **Confluent_Kafka** (Note, the respective security artifact has been already deployed on the Cloud Integration tenant)

    <br><img src="/exercises/ex2/images/02-0012.png" width=100%>

8. Switch to the *Processing* tab, and enter your previously created Kafka topic **IN260_XX** with **XX** the participant number assigned to you

    <br><img src="/exercises/ex2/images/02-0013.png" width=50%>

## Summary

You should have configured the connection to the Kafka system to fetch the events from your Kafka topic.

Next, we will add and configure a content modifier. Continue to - [Exercise 2.3](/exercises/ex2/ex23)

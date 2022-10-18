# Exercise 2 - Process Automation

In the second part of the exercise, you will create and model a new integration flow that subscribes to your Kafka topic and triggers a process where the manager can decide the equipment and training required for the new hire created in SAP SuccessFactors. 
To achieve this, we will be using SAP Build Process Automation, the AI-powered, intuitive, and no-code solution for workflow management and RPA availble on the SAP Business Technology Platform. 

In this exercise, you will design the integration flow as an exactly once scenario to ensure that duplicate messages are avoided.

## Exercise steps

Run through the exercise steps in the given order.

[Create a new integration flow](ex21)

[Maintain the Kafka connection](ex22)

[Maintain the Content Modifier](ex23)

[Maintain the Message Mapping](ex24)

[Model the exactly once connectivity to SPA](ex25)

[Deploy your integration flow](ex26)


## Summary

At the end of the second part of the tutorial, you should have deployed an integration flow to trigger a workflow supporting exactly once delivery.

Next we will test the integration scenario by creating a new hire in SAP SuccessFactors. Continue to - [Exercise 3](/exercises/ex3)

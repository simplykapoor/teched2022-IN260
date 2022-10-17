# Exercise 2.5 - Model the Exactly Once connectivity to SAP Process Automation

In the following, we will configure the connection to SAP Process Automation in such a way that the workflow is triggered only once. This is achieved by placing the actual connection in a so called idempotent process. With an idempotent process call, you can check if a local integration process has been already processed for one and the same message. In case of a duplicate detected, the processing of this message can be skipped. This way, you can avoid duplicate messages sent to a receiver which is not idempotent, i.e., which is not able to identify duplicates.

## Exercise steps

Run through the following steps
1. Open ...

2. Switch ...

    <br><img src="/exercises/ex4/images/04-0001.png" width=50% height=50%>

3. In ..., select button *Create*


## Summary

You should have ...

Continue to - [Exercise 2.6](/exercises/ex2/ex26)

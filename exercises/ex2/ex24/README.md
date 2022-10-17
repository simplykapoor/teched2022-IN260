# Exercise 2.4 - Maintain the Message Mapping

In the following, we need to map to the format that is required to trigger the workflow in SAP Process Automation. For your convenience, we have provided a reusable message mapping artifact which maps the JSON format of the SAP SuccessFactors event to the JSON format of the particular workflow. Furthermore, the message mapping the employee ID of the incoming event is mapped to an exchange property which is needed for the configuration of the exactly once delivery.

## Exercise steps

Run through the following steps

1. First of all, we need to add the reusable message mapping to the resources of your integration flow. In the Properties of your integration flow, switch to the Resources tab
2. Below the Resources tab, switch to the References tab
3. From the Add References menu at the right, select the Message Mapping entry

    <br><img src="/exercises/ex2/images/02-0028.png" width=100%>

1. If you select the *Content Modifier* step of the *Integration Process* pool, the quick menu appears. Select the *Plus* icon of the quick menu

    <br><img src="/exercises/ex2/images/02-0023b.png" width=50%>

2. In the upcoming menu, search for *mapping*, then select the *Message Mapping* entry

    <br><img src="/exercises/ex2/images/02-0024.png" width=40%>

3. A Message Mapping step has been added to your integration flow model right after the *Content Modifier* step. Select the flow step

    <br><img src="/exercises/ex2/images/02-0024a.png" width=40%>

3. In ..., select button *Create*


## Summary

You should have created a Message Mapping step to your integration flow and assigned the provided reusable Message Mapping.

Continue to - [Exercise 2.5](/exercises/ex2/ex25)

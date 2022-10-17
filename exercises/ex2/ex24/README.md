# Exercise 2.4 - Maintain the Message Mapping

In the following, we need to map to the format that is required to trigger the workflow in SAP Process Automation. For your convenience, we have provided a reusable message mapping artifact which maps the JSON format of the SAP SuccessFactors event to the JSON format of the particular workflow. Furthermore, the message mapping fetches the employee ID of the incoming event and stores it in an exchange property which is at the end needed for the configuration of the exactly once delivery.

## Exercise steps

Run through the following steps

1. First of all, we need to add the reusable message mapping to the resources of your integration flow. In the properties of your integration flow, switch to the *Resources* tab
2. Below the *Resources* tab, switch to the *References* tab
3. From the *Add References* menu at the right, select the *Message Mapping* entry

    <br><img src="/exercises/ex2/images/02-0028.png" width=100%>

4. In the upcoming dialog, select source as *Integration Flow* and the package **Teched 2022 IN260 - SOL** from the drop down menu

    <br><img src="/exercises/ex2/images/02-0030.png" width=50%>

5. The resuable artifact is shown. Select the message mapping **Map SFSF JSON to SPA JSON - SOL** and select the *OK* button

    <br><img src="/exercises/ex2/images/02-0031.png" width=50%>

6. As you can see from the figure below, the mapping has been added to the resources of your integration flow as reference

    <br><img src="/exercises/ex2/images/02-0032.png" width=100%>

7. Let's now use the mapping in your integration flow model. If you select the *Content Modifier* step of the *Integration Process* pool, the quick menu appears. Select the *Plus* icon of the quick menu

    <br><img src="/exercises/ex2/images/02-0023b.png" width=40%>

8. In the upcoming menu, search for *mapping*, then select the *Message Mapping* entry

    <br><img src="/exercises/ex2/images/02-0024.png" width=40%>

9. A Message Mapping step has been added to your integration flow model right after the *Content Modifier* step. Select the flow step

    <br><img src="/exercises/ex2/images/02-0024a.png" width=40%>

10. In the properties of the message mapping step, switch to the *Processing* tab, then select the *Select* button

    <br><img src="/exercises/ex2/images/02-0033.png" width=40%>

11. In the upcoming dialog, switch to the *Referenced Resources* tab
12. From the list of Resources, select the beforehand added message mapping **Map_SFSF_JSON_to_SPA_JSON_SOL**, then select *OK*

    <br><img src="/exercises/ex2/images/02-0034.png" width=40%>

13. As you can see from the figure below, the mapping has been added 

    <br><img src="/exercises/ex2/images/02-0034a.png" width=40%>

## Summary

You should have created a Message Mapping step in your integration flow and assigned the provided reusable Message Mapping.

Next, we will configure the connection to the SAP Process Automation. Continue to - [Exercise 2.5](/exercises/ex2/ex25)

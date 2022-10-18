# Exercise 2.5 - Model the Exactly Once connectivity to SAP Build Process Automation

In the following, we will configure the connection to SAP Build Process Automation in such a way that the workflow is triggered only once. This is achieved by placing the actual connection in a so called idempotent process. With an idempotent process call, you can check if a local integration process has been already processed for one and the same message. In case of a duplicate detected, the processing of this message can be skipped. This way, you can avoid duplicate messages sent to a receiver which is not idempotent, i.e., which is not able to identify duplicates.

## Exercise steps

Run through the following steps
1. First, we will model the connection to SAP Build Process Automation within a subprocess. From the palette, select the entry *Local Integration Process* below the *Process* menu

    <br><img src="/exercises/ex2/images/02-0014.png" width=50%>

2. Place the new *Local Integration Process* below the *Receiver* component

    <br><img src="/exercises/ex2/images/02-0015a.png" width=70%>

3. Select the *Start* event of the *Local Integration Process*. From the quick menu, select the *Plus* icon

    <br><img src="/exercises/ex2/images/02-0016.png" width=50%>

4. In the upcoming menu, enter the search term *request*, then select the *Request Reply* entry

    <br><img src="/exercises/ex2/images/02-0017.png" width=30%>

5. From the quick menu of the just added *Request Reply* step, select the *Connector* icon ...

    <br><img src="/exercises/ex2/images/02-0018.png" width=20%>

6. ... and drag it on the *Receiver* component

    <br><img src="/exercises/ex2/images/02-0019.png" width=35%>

7. If you release the connection, a dialog comes up where you need to select the adapter type. In our case, select the entry *HTTP*

    <br><img src="/exercises/ex2/images/02-0020.png" width=30%>

8. Your local integration process flow should look like in figure below. Select the connection between the *Request Reply* step and the *Receiver*

    <br><img src="/exercises/ex2/images/02-0021a.png" width=50%>

9. In the properties of the *HTTP* connection, switch to tab *Connection* and maintain the connection details as follows: 
    1. Address: **https://spa-api-gateway-bpi-us-prod.cfapps.us10.hana.ondemand.com/workflow/rest/v1/workflow-instances**
    2. Authentication: Select *OAuth2 Client Credentials* from the drop down menu
    3. Credential Name: **SPA_OAuth2** (Note, the respective security artifact has been already deployed on the Cloud Integration tenant)

    <br><img src="/exercises/ex2/images/02-0021.png" width=80%>

10. Let's now call the local integration process right after the message mapping step within the main integration process. If you select the *Message Mapping* step of the Integration Process pool, the quick menu appears. Select the *Plus* icon of the quick menu

    <br><img src="/exercises/ex2/images/02-0025a.png" width=50%>

11. In the upcoming menu, search for *idempotent*, then select the *Idempotent Process Call* entry

    <br><img src="/exercises/ex2/images/02-0025.png" width=50%>

12. An *Idempotent Process Call* step has been added to your integration flow model right after the *Message Mapping* step. Select the flow step

    <br><img src="/exercises/ex2/images/02-0025b.png" width=80%>

13. In the properties of the *Idempotent Process Call*, switch to the *Processing* tab and select the *Select* button

    <br><img src="/exercises/ex2/images/02-0035.png" width=50%>

14. From the upcoming dialog, select your previously created *Local Integration Process*

    <br><img src="/exercises/ex2/images/02-0036.png" width=50%>

15. Finally, maintain the idempotent conditions details as follows:
    1. Set *Message ID* to **${property.employeeId}**
    2. Keep the *Skip Process Call for Duplicates* flag *selected*

    <br><img src="/exercises/ex2/images/02-0037.png" width=50%>

## Summary

You should have configured the exactly once delivery to SAP Build Process Automation.

With this, the model is complete. You can save and deploy the same. Continue to - [Exercise 2.6](/exercises/ex2/ex26)

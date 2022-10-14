# Exercise 2.3 - Maintain the Content Modifier

In the following, you will add a Content Modifier to the main process to define the content type of the event sent to SAP Process Automation as well as the email of the manager which needs to approve your workflow task.

## Exercise steps

Run through the following steps

1. If you select the *Start Message* event of the *Integration Process* pool, the quick menu appears. Select the *Plus* icon of the quick menu

    <br><img src="/exercises/ex2/images/02-0022.png" width=50%>

2. In the upcoming menu, select the *Content Modifier* entry

    <br><img src="/exercises/ex2/images/02-0023.png" width=40%>

3. A Content Modifier step has been added to your integration flow model right after the *Start Message* event. Select the flow step

    <br><img src="/exercises/ex2/images/02-0023a.png" width=40%>

4. In the properties of your Content Modifier step, switch to the *Message Header* tab
5. Select the *Add* button to add a new entry
6. Maintain the new entry as follows:
    1. Action: **Create**
    2. Name: **Content-Type**
    3. Source Type: **Constant**
    4. Source Value: **application/json**

    <br><img src="/exercises/ex2/images/02-0026.png" width=100%>

7. Switch to the *Exchange Property* tab
8. Select the *Add* button to add a new entry
9. Maintain the new entry as follows:
    1. Action: **Create**
    2. Name: **managerEmail**
    3. Source Type: **Constant**
    4. Source Value: **userXX@techedusers.com** (with **XX** the participant number assigned to you)

    <br><img src="/exercises/ex2/images/02-0027.png" width=100%>

**Note**: the exchange property *managerEmail* is used in the message mapping to map to the event sent to SAP Process Automation.

## Summary

You should have created and configured the Content Modifier step.

Next, we will add the message mapping to map from the format of the SAP SuccessFactors event to the format that is required to trigger the workflow in SAP Process Automation. Continue to - [Exercise 2.4](/exercises/ex2/ex24)

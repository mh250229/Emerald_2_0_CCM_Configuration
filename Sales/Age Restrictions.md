## Age Restrictions

**Age Restrictions** comprise of a set of restrictions based on the date and time items are sold, the customers age, and user age. There is no relation between the different restrictions.  
For example, you can define Age Restricted policies to:

* Restrict the sale of alcohol or DVDs to customers under 18. If a customer under 18 tries to purchase one of the items the sale is prohibited.
* Prohibit the sale of age restricted items on the 25.8.2012. If a customer tries to purchase one of the items on the 25.8.2012, the sale is prohibited. However, the items can be purchased from the 26.8.2012.

In addition, once a transaction is saved and then recalled, the restricted items require approval even if they were already approved before saving the transaction.

Age Restrictions can be configured to trigger after the customer has scanned all their items at the Self Checkout (SCO) and selects OK to pay for the items. The restrictions are prompted and the attendant solves each restriction as required.

Currently, this is configured via the PUT/emerald/selling-service/selling-configuration/v1/business-rules-settings/age-restrictions/{ruleId} in the Selling Configuration Services.


### Configuring an Age Restriction

This example describes how to set up an Age Restriction Rule to prevent cigarette purchases to individuals under the age of 18.

1. Browse to Sales/Rules/Age Restrictions.
2. Click **+ Add Policy**. The **New Age Restricted Policy** screen is displayed.
3. In the **Policy ID** field, enter the Id of the policy. It is a unique identifier.
4. From the **Location** drop-down list, select the store(s) in which the policy is supported.

    a. To search for a store, in the Type to Search field, enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.

    Or

    From the left pane, select the checkboxes next to each store linked to the data pattern.  
    All stores selected are displayed in the Selections in the right pane.

    b. Click **Save** to save the selected stores.

5. From the **Touchpoint Groups** drop-down list, select the touchpoint group to which the age restriction is associated, e.g., Main Lane.
6. (Optional) Define each of the following according to your requirements:  

    **Policy Members**  

    a. In the **Select Products** field, click the + icon. See details on how to search for items in Browse or Look Up Item Screen  
    Select the item on which you are defining the age restriction.

    Or  

    From the **Select Category** drop-down list, select the Category of items on which you are linking the age restriction.

    Or  

    From the **Select Groups** drop-down list, select the Group to which you are linking the age restriction.  

    b. Click **Save**.  

    The Included Locations field displays the locations selected, i.e., the rule applies to these locations.  
    The Excluded Locations field displays the locations excluded, i.e., the rule does not apply to these locations.  

    **Date TIme**  

    a. Define the date and time during which the Age Restriction policy is active.  

    b. From the **Action Type** drop-down list, select the action to take when the age restriction policy is triggered, e.g., Prohibit or Approval Required.  

    c. From the **Days of the Week** drop-down list, select the checkboxes next to each day of the week on which the Age Restriction is active.

    ![Date Time Form](/Images/datetimeform.png)

    d. In the **Start Date** and **End Date** fields, enter the dates to define the period during which the policy is valid.  
    Click the calendar icon to use the calendar to assist you in selecting the dates.  
    If you select the **No end date** to indicate that the policy runs with no effective end date, the End Date field is greyed out.  

    e. To add an additional date between which the policy runs, click **Add Another Date**.  

    f. In the **Start Time** and **End Time** fields, click the clock icon and select the time from which the policy is active.  
    If you select the **No end date** to indicate that the policy runs with no effective end date, the End Date field is greyed out.

   ![Date Time Prohibit Form](/Images/DateTimeProhibitForm.png)

    g. From the **Message** drop-down list, select the Age Restriction message you want to prompt when the policy is triggered.  

    h. If you selected the **Action Type** ‘Approval Required’, the **Roles** field is enabled.  
    From the **Roles** drop-down list, select the role with the privileges required by the person who is approving the activity.  
    **Note:** The **Roles** field is not supported in this version.

    You can view the messages after linking it to the policy, create a new message on the fly, or edit an existing message. For details on Messages, see Messages.  

    **Customer Age**

    From the **Age Confirmation Action Type** drop-down list, select the relevant option:  
    * Approve/Reject  
    * Enter Date Of Birth  
    * Enter DoB/Approve/Reject


    **Approve/Reject Option**

    a. In the **Customer Age is less than** field, enter the maximum customer age.  

    b. From the Message drop-down list, select the message. For details on Messages, see Messages  

    c. (Optional) From the **Reject Reason Codes** drop-down list, select the reasons for rejecting the sale of the item. If selected, when the Age Restriction policy is triggered on the POS, the cashier can select a reason from the list of reason codes.  

    ![Customer Age Form](/Images/CustomerAgeForm.png)

    **Enter Date Of Birth Option**

    a. In the **Customer Age is less than** field, enter the maximum customer age.

    b. From the **Message** drop-down list, select the message. For details on Messages, see Messages

    ![Customer Age Confirmation Acion Type Form](/Images/CustomerAgeConfirmationActionTypeForm.png)  

    **Enter Date Of Birth/Approve/Reject Option**

    a. In the **Customer Age is less than** field, enter the maximum customer age.

    b. From the **Message** drop-down list, select the message. For details on Messages, see Messages.

    c. (Optional) From the **Reject Reason Codes** drop-down list, select the reasons for rejecting the sale of the item. If selected, when the Age Restriction policy is triggered on the POS, the cashier can select a reason from the list of reason codes.  

7. Select **Save**.

### Configuring an Age Restriction 18

This example describes how to set up an Age Restriction Rule to prevent beer purchases to individuals under the age of 18.  

1. Browse to Sales/Rules/Age Restrictions.
1. Click **+ Add Policy**. The **New Age Restricted Polic**y screen is displayed.
1. In the **Policy ID** field, enter the Id of the policy, e.g., AgeRestriction18.
1. From the **Location** drop-down list, select Root.
1. Click the arrow in the **Policy Members** options. 
1. In the **Products** field, enter Goldstar beer, Carlsberg beer, and Heineken beer. 
1. Click the arrow in the **Customer Age** options. 
1. In the **Age Confirmation Action Type** dropdown menu, select Enter DoB / Approve / Reject.
1. In the **Customer Age is less than...**  field, enter 18.
1. In the **Message** drop down menu, select UnderAge18Message.
1. Click **Save**.

### Configuring an Age Restriction 21

This example describes how to set up an Age Restriction Rule to prevent beer purchases to individuals under the age of 21.  

1. Browse to Sales/Rules/Age Restrictions.
1. Click **+ Add Policy**. The **New Age Restricted Policy** screen is displayed.
1. In the **Policy ID** field, enter the Id of the policy, e.g., AgeRestriction21.
1. From the **Location** drop-down list, select Root.
1. Click the arrow in the **Policy Members** options. 
1. In the **Products** field, enter Goldstar beer, Carlsberg beer, and Heineken beer. 
1. Click the arrow in the **Customer Age** options. 
1. In the **Age Confirmation Action Type** dropdown menu, select Enter DoB / Approve / Reject.
1. In the **Customer Age is less than...**  field, enter 21.
1. In the **Message** drop down menu, select UnderAge21Message.
1. Click **Save**.
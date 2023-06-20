## Return Policies

**Return Policies** determine how to handle items returned to the store by customers.  

Return Policy types include:

* **Non Receipted** - to define general refund policy details for all transactions in which items are returned without a receipt.
* **Transaction Based** - to define general refund policy details for all transactions in which items are returned with a receipt.
* **Bottle Deposi**t - to define a refund policy when empty bottles are returned to refund the deposit amount.  

**Note:** Currently in the Restrictions only Sellable ID, Group, and Hierarchy are supported by the UI.

### Configuring a Non-Receipted Return Policy (NRR)

1. Browse to Sales/Return/Return Policies.
2. Click **+ Add Return Policy**. The **New Return Policy** screen is displayed.
3. In the **Policy Name** field, enter **NRR**.
4. From the **Location** drop-down list, select the store(s) in which the Return Policy is supported.  

    a. To search for a store, in the Type to Search field, enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.  

    Or  

    From the left pane, select the checkboxes next to each store linked to the data pattern.  
    All stores selected are displayed in the Selections in the right pane.  

    b. Click **Save** to save the selected stores.

5. From the **Return Policy Type** drop-down list, select Non Receipted.

6. In the **Start Date** and **End Date** fields, enter the dates to define the period during which the return policy is valid.  
Click the calendar icon to use the calendar to assist you in selecting the dates.
7. In the **Start Time** and **End Time** fields, click the clock icon and select the time from which the return policy is active.
8. Select the **Details** tab, click **Basic Definitions**.
9. (Optional) In the **Prompt for Reason Codes** option, select **Never**.

    Or  

    Select **For Each Item**.
    * From the **Select Reason Codes** drop-down list, select the reason codes, e.g., defective item, wrong color, etc.  
    * In the **Select Products** field, click the + icon, then select the products that if returned, prompt the cashier to select the reason for returning the item.
    * From the **Select Categories** drop-down list, select a category that if an item associated to the selected category is returned, the POS prompts the cashier to select the reason for returning the item.
10. Click **Non Receipted Tenders**.
11. (Optional) From the **Refund Tender** drop-down list, select the tender used to refund money to the customer.
12. (Optional) In the **Up to Amount** field, enter the amount up to which the tender can be used to reimburse the customer.
13. (Optional) From the **Allowed Roles to Switch** drop-down list, select the roles authorized to override the recommended refund tender.
14. (Optional) From the **Message** field, select the message displayed to prompt for authorization when the refund tender is switched.
15. (Optional) Select the **Restrictions** tab.
16. Click **+ Add Restriction**.
17. In the **Restriction Name** field, enter the name of the restriction.  

    a. From the **Select Attribute** drop-down list, select the relevant option, e.g., Product, Group, or Category.  

    b. From the **Product/Groups/Category** drop-down list, select the option for which you are defining the restriction. For example, you may define a restriction on all dairy products.  

    c. Set the **Include** slider to Yes or No:

    * **Yes** – indicates that the Product/Group/Category is included, i.e., restricted.  
    * **No** – indicates that the Product/Group/Category is not included, i.e., not restricted, but all other Products/Groups/Categories are restricted.

    d. Click **Add Attribute**.  

    e. From the **Select Action Type** drop-down list, select the action required if the item being returned falls within the defined restriction, e.g., if the item belongs to a Dairy category, prohibit the return. You can define multiple restrictions, i.e., one to request manager approval if an item is being returned due to a damaged box or expiration date, and another restriction to prohibit the return of an item.

    f. Click **Save**.

18. Click **Save as Draft** to save the restriction policy you just defined for later use.  

    Or

    Click **Publish** to activate the new return policy.

### Configuring a Transaction Based Return Policy (TBR)

**Note:** There is no Base Configuration for Recommended Refund Tenders.

1. Browse to Sales/Return/Return Policies.
2. Click **+ Add Return Policy**. The **New Return Policy** screen is displayed.
3. In the **Policy Name** field, enter **NRR**.
4. From the **Location** drop-down list, select the store(s) in which the Return Policy is supported.

    a. To search for a store, in the Type to Search field, enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.  

    Or  

    From the left pane, select the checkboxes next to each store linked to the data pattern.
    All stores selected are displayed in the Selections in the right pane.  

    b. Click **Save** to save the selected stores.

5. From the **Return Policy Type** drop-down list, select Transaction Based.  
6. In the **Start Date** and **End Date** fields enter the dates to define the period during which the return policy is valid.
Click the calendar icon to use the calendar to assist you in selecting the dates.  
7. In the **Start Time** and **End Time** fields click the clock icon and select the time from which the return policy is active.  
8. (Optional) Select the **Details** tab, click **Basic Definitions**.  
9. In the **Return Best For** option select Retailer or Customer, based on your store policy.  
    * **Retailer** - indicates that the retailer is favored  
    * **Customer** - indicates that the customer is favored  
10. In the **Prompt for Reason Codes** option, select **Never**.

    Or  

    Select **For Each Item**.  

    * From the **Select Reason Codes** drop-down list, select the reason codes, e.g., defective item, wrong color, etc.  
    * In the **Select Products** field, click the + icon, then select the products that if returned, prompt the cashier to select the reason for returning the item.  
    * From the **Select Categories** drop-down list, select a category that if an item associated to the selected category is returned, the POS prompts the cashier to select the reason for returning the item.

11. In the **Receipt Search Time Frame** field, enter the number of days up to which the system searches for the original receipt.  
12. Click **Recommended Tenders**.  
13. (Optional) From the **Paid Tender** drop-down list, select the tender used to pay for the item in the original sale transaction.  
14. (Optional) From the **Refund Tender** drop-down list, select the tender used to refund money to the customer.  
15. (Optional) In the **Up to Amount** field, enter the amount up to which the tender can be used to reimburse the customer.  
16. (Optional) In the **Priority** field, enter the priority by which the refund tenders are used to reimburse the customer when there is more than one paid tender in a transaction.  
17. (Optional) From the **Allowed Roles to Switch** drop-down list, select the roles authorized to override the recommended refund tender.  
18. (Optional) From the **Message** field, select the message displayed to prompt for authorization when the refund tender is switched.  
19. (Optional) Select the **Restrictions** tab.  
20. Click **+ Add Restriction**.  
21. In the **Restriction Name** field, enter the name of the restriction.  

    a. From the **Select Attribute** drop-down list, select the relevant option, e.g., Product, Group, or Category.  

    b. From the **Product/Groups/Category** drop-down list, select the option for which you are defining the restriction. For example, you may define a restriction on all dairy products.  

    c. Set the **Include** slider to Yes or No:  
        * **Yes** – indicates that the Product/Group/Category is included, i.e., restricted.  
        * **No** – indicates that the Product/Group/Category is not included, i.e., not restricted, but all other Products/Groups/Categories are restricted.

    d. Click **Add Attribute**.  

    e. From the **Select Action Type** drop-down list, select the action required if the item being returned falls within the defined restriction, e.g., if the item belongs to a Dairy category, prohibit the return. You can define multiple restrictions, i.e., one to request manager approval if an item is being returned due to a damaged box or expiration date, and another restriction to prohibit the return of an item.  

    f. Click **Save**.

22. Click **Save as Draft** to save the restriction policy you just defined for later use.

    Or

    Click **Publish** to activate the new return policy.

### Configuring a Bottle Deposit Return Policy (BDR)

1. Browse to Sales/Return/Return Policies.  
2. Click **+ Add Return Policy**. The **New Return Policy** screen is displayed.  
3. In the **Policy Name** field, enter **Bottle Deposit**.  
4. From the **Location** drop-down list, select the store(s) in which the Return Policy is supported.  

    a. To search for a store, in the **Type to Search** field, enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.

    Or  

    From the left pane, select the checkboxes next to each store linked to the data pattern.
    All stores selected are displayed in the Selections in the right pane.

    b. Click **Save** to save the selected stores.

5. From the **Return Policy Type** drop-down list, select Non Receipted.
6. In the **Start Date** and **End Date** fields enter the dates to define the period during which the return policy is valid.
Click the calendar icon to use the calendar to assist you in selecting the dates.
7. In the **Start Time** and **End Time** fields click the clock icon and select the time from which the return policy is active.
8. (Optional) Select the **Restrictions** tab.
9. Click **+ Add Restriction**.
10. In the **Restriction Name** field, enter the name of the restriction.

    a. From the **Select Attribute** drop-down list, select the relevant option, e.g., Product, Group, or Category.

    b. From the **Product/Groups/Category** drop-down list, select the option for which you are defining the restriction. For example, you may define a restriction on all dairy products.
  
    c. Set the **Include** slider to Yes or No:  
        * **Yes** – indicates that the Product/Group/Category is included, i.e., restricted.  
        * **No** – indicates that the Product/Group/Category is not included, i.e., not restricted, but all other Products/Groups/Categories are restricted.  

    d. Click **Add Attribute**.  

    e. From the **Select Action Type** drop-down list, select the action required if the item being returned falls within the defined restriction, e.g., if the item belongs to a Dairy category, prohibit the return. You can define multiple restrictions, i.e., one to request manager approval if an item is being returned due to a damaged box or expiration date, and another restriction to prohibit the return of an item.

    f. Click **Save**.

11. Click **Save as Draft** to save the restriction policy you just defined for later use.

    Or

    Click **Publish** to activate the new return policy.

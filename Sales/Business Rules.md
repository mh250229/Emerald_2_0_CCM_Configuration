## Business Rules

The following Business Rules can be triggered at the POS:
* Price Override
* Quantitative Limit
* Void Item
* Void Transaction
* Price Override
* Product

**Note:** currently, the ‘Scope’ option is only supported via API. Automation Rejection Messages are only supported by the API. Roles is not supported.

Business Rules can be configured to trigger after the customer has scanned all their items at the Self Checkout (SCO) and selects OK to pay for the items. The restrictions are then prompted and the attendant solves each restriction as required.

Currently, this is configured via the Selling Configuration Services only.

Delayed approval is supported for the following Business Rules:

* **Price Override**  
PUT/emerald/selling-service/selling-configuration/v1/business-rules-settings/price-overrides/{ruleId}
* **Quantitative Limit**  
PUT/emerald/selling-service/selling-configuration/v1/business-rules-settings/quantities/{ruleId}
* **Void Item**  
PUT/emerald/selling-service/selling-configuration/v1/business-rules-settings/void-limits/{ruleId}
* **Product**  
PUT/emerald/selling-service/selling-configuration/v1/business-rules-settings/product-sales/{ruleId}


### Configuring a Price Override BRM

The **Price Override** rule controls the option of overriding the price of an item during a transaction. If a transaction includes an item for which the price is overridden, you can prevent/allow cashiers to override the item price by a defined percentage.  
**Note:** The rule is triggered once the actual product price exceeds the defined limits before any promotions or taxes are calculated on the product’s price.  
This scenario describes how to set up a Prohibit Price Override Business Rule.

1. Browse to Sales/Rules/Business Rules

2. Click **+ Add Business Rule**. The New Business Rule screen is displayed.

3. In the **Name** field, enter Price Override.

4. From the **Type** drop-down list, select **Price Override**.

5. In the **Maximum Discount Amount** field, enter a percentage indicating the maximum percent amount by which the price can be reduced, e.g., 20%

6. (Optional) define each of the following according to your requirements:

    **Location Condition**

    a. In the Included Locations field, click the + sign.  

    b. In the left pane of the form, in the **Search** field, search for the location that you are including by entering the name of the full or partial name of the location and press Enter. The location is listed in the left pane.

    Or

    From the left pane, select the checkbox of the Root to include all locations, or select the checkboxes next to the locations you wish to include.  
    The selected locations are displayed in the right pane under the Included Selections.  
    The Locations not included are displayed in the Excluded Selections  

    c. Click **Save**.  
    The Included Locations field displays the locations selected, i.e., the rule applies to these locations.
    The Excluded Locations field displays the locations excluded, i.e., the rule does not apply to these locations.  

    **Touchpoint Groups Condition**

    From the Touchpoint Groups, select the relevant option:  
    * To apply the business rule to all touchpoint groups, select **Apply to All**.  

        Or

    * To apply the business rule to a specific touchpoint group, select **Selected Groups**.  
    From the **Included Groups** drop-down list, select the groups you wish to apply the business rule.  

    **Product Condition**

    a. From the **Apply To** drop-down list, select Sale item only.

    b. From the **Groups** drop-down list, select the item groups to which you are associating the Business Rule.

    c. From the **Category** drop-down list, select the categories to which are associating the Business Rule.

    d. From the **Products** field, click the **+** sign. The Browse or Look Up Item form is displayed.

    e. Search for the product as follows:
        i. In the **Item** field, enter the full or partial name of the item.
        ii. Select the **Exact Match** option to indicate that the system must retrieve the exact name of the item entered.  
        Or  
        Search by **Category**, from the Category drop-down list, select a category.  
        iii. Click **Search**.  
        The items that match the search criteria are displayed in the grid by Code, Additional Codes, and Description.  
        iv. From the **Selection** section, select the item.  
        v. Click **Save**.


    **Customer Order Condition**

    **Note:** The Customer Order Condition fields are not supported in this version.

    a. In the **Transaction Maximums** section, in the **Amount** field, enter the maximum transaction amount allowed in the customer order. If exceeded, the business rule is triggered.

    b. In the **Quantity** field, enter the maximum number of items allowed in the customer order. If exceeded, the business rule is triggered.

    c. In the Loyalty Card Exists section from the **Includes Loyalty Card** drop-down list, select the relevant option:

    * Includes / Excludes Loyalty Card – indicates that a notification is always prompted on the POS regardless if a loyalty card was added to the transaction. 

    * Includes Loyalty Card – indicates that a notification is only prompted on the POS if a loyalty card was added to the transaction. 

    * Excludes Loyalty Card – indicates that a notification is only prompted on the POS if no loyalty card was added to the transaction.

7. Select the **Actions Tab**.

8. From the **Action Type** drop-down list, select Prohibit.

9. From the **Message** drop-down list, select the Prohibit Price Override message.

    You can view the messages after linking it to the BRM, create a new message on the fly, or edit an existing message. For details on Messages, see Messages

10. Click **Save** to save the Business Rule.

### Configuring a Quantitative Limit BRM

The **Quantitative Limit** rule evaluates the total quantity/weight/amount of a transaction in order to be able to control the maximum or minimum quantity, weight, or amount of a transaction.

This scenario describes how to set up a Quantitative Limit Business Rule with a Notification Message.

1. Browse to Sales Rules/Business Rules

2. Click **+ Add Business Rule**. The New Business Rule screen is displayed.

3. In the **Name** field, enter Quantitative Limit.

4. From the **Type** drop-down list, select **Quantitative Limit**.

5. In the **Aggregate on** section, from the **Type** drop-down list, select the relevant option:

    * **Quantity** - to specify that the minimum/maximum amount is based on the item quantity purchased.

    * **Weight** - to specify that the minimum/maximum amount is based on the item weight purchased.

    * **Amount** – to specify that the minimum/maximum amount is based on the item amount (price) purchased.

6. From the **Max/Min** drop-down list, select the Max or Min to specify that the value in the **Enter Number** field is the minimum or maximum value.

7. In the **Enter Number** field, enter the value applied to the selected Type and Min/Max options.

8. (Optional) define each of the following according to your requirements:

    **Location Condition**

    a. In the Included Locations field, click the + sign.

    b. In the left pane of the form, in the Search field, search for the location that you are including by entering the name of the full or partial name of the location and press Enter. The location is listed in the left pane.

    Or

    From the left pane, select the checkbox of the Root to include all locations, or select the checkboxes next to the locations you wish to include.

    The selected locations are displayed in the right pane under the Included Selections.

    The Locations not included are displayed in the Excluded Selections

    c. Click **Save**.

    The Included Locations field displays the locations selected, i.e., the rule applies to these locations.

    The Excluded Locations field displays the locations excluded, i.e., the rule does not apply to these locations.

    **Touchpoint Groups Condition**

    From the Touchpoint Groups, select the relevant option:

    * To apply the business rule to all touchpoint groups, select **Apply to All**.

        Or

    * To apply the business rule to a specific touchpoint group, select **Selected Groups**.

    From the **Included Groups** drop-down list, select the groups you wish to apply the business rule.

    **Product Condition**

    a. From the **Apply To** drop-down list, select Sale item only.

    b. From the **Groups** drop-down list, select the item groups to which you are associating the Business Rule.

    c. From the **Category** drop-down list, select the categories to which are associating the Business Rule.

    d. From the **Products** field, click the + sign. The Browse or Look Up Item form is displayed.

    e. Search for the product as follows:  
        i. In the **Item** field, enter the full   or partial name of the item.  
        ii. Select the **Exact Match** option to indicate that the system must retrieve the exact name of the item entered.  
        Or  
        Search by Category, from the **Category** drop-down list, select a category.  
        i. Click **Search**.  
        The items that match the search criteria are displayed in the grid by Code, Additional Codes, and Description.  
        ii. From the **Selection** section, select the item.  
        iii. Click **Save**.

    **Customer Order Condition**

    **Note:** The Customer Order Condition fields are not supported in this version.

    a. In the **Transaction Maximums** section, in the **Amount** field, enter the maximum transaction amount allowed in the customer order. If exceeded, the business rule is triggered.

    b. In the **Quantity** field, enter the maximum number of items allowed in the customer order. If exceeded, the business rule is triggered.

    c. In the Loyalty Card Exists section from the **Includes Loyalty Card** drop-down list, select the relevant option:

    * Includes / Excludes Loyalty Card – indicates that a notification is always prompted on the POS regardless if a loyalty card was added to the transaction.

    * Includes Loyalty Card – indicates that a notification is only prompted on the POS if a loyalty card was added to the transaction.

    * Excludes Loyalty Card – indicates that a notification is only prompted on the POS if no loyalty card was added to the transaction.

9. Select the **Actions Tab**.

10. From the **Action Type** drop-down list, select **Notification**.

11. From the **Message** drop-down list, select the **NotificationMinimumWeight** message.
    You can view the messages after linking it to the BRM, create a new message on the fly, or edit an existing message. For details on Messages, see Messages.

12. From the **Scope** drop-down list, select the relevant options:

    * **Per Line** – to specify that the business rule is always triggered.

    * **Cart** – to specify that the business rule is only triggered once per transaction.  

        **Note:** The **Scope** field is not supported in this version.

13. Click **Save** to save the Business Rule.

## Configuring a Void Item BRM

The **Void Item** rule evaluates the items voided in a transaction. This enables the manager to monitor cancelled items performed by a cashier and prevent fraud.

This scenario describes how to set up a Void Item Business Rule with Manager Approval.

1. Browse to Sales Rules/Business Rules

2. Click **+ Add Business Rule**. The New Business Rule screen is displayed.

3. In the **Name** field, enter Void Item.

4. From the **Type** drop-down list, select **Void Item**.

5. From the **Limit Value Type** drop-down list, select the relevant option:

    * **Max allowed per Transaction** – to specify that the Limit Value Amount is the maximum amount that can be voided per transaction.

    * **Max allowed per Line** - to specify that the Limit Value Amount is the maximum amount that can be voided per item.

6. In the **Limit Value Amount** field, enter the maximum amount value, e.g., 100

7. (Optional) define each of the following according to your requirements:

    **Location Condition**

    a. In the Included Locations field, click the + sign. 

    b. In the left pane of the form, in the Search field, search for the location that you are including by entering the name of the full or partial name of the location and press Enter. The location is listed in the left pane.

    Or

    From the left pane, select the checkbox of the Root to include all locations, or select the checkboxes next to the locations you wish to include.

    The selected locations are displayed in the right pane under the Included Selections.
    The Locations not included are displayed in the Excluded Selections

    c. Click **Save**.

    The Included Locations field displays the locations selected, i.e., the rule applies to these locations.

    The Excluded Locations field displays the locations excluded, i.e., the rule does not apply to these locations.

    **Touchpoint Groups Condition**

    From the Touchpoint Groups, select the relevant option:

    * To apply the business rule to all touchpoint groups, select **Apply to All**.

        Or

    * To apply the business rule to a specific touchpoint group, select **Selected Groups**.

    From the **Included Groups** drop-down list, select the groups you wish to apply the business rule.

    **Product Condition**

    a. From the **Apply To** drop-down list, select Sale item only.

    b. From the **Groups** drop-down list, select the item groups to which you are associating the Business Rule.

    c. From the **Category** drop-down list, select the categories to which are associating the Business Rule.

    d. From the **Products** field, click the + sign. The Browse or Look Up Item form is displayed.

    e. Search for the product as follows:  
        i. In the **Item** field, enter the full or partial name of the item.  
        ii. Select the **Exact Match** option to indicate that the system must retrieve the exact name of the item entered.  
        Or  
        Search by Category, from the **Category** drop-down list, select a category.  
        i. Click **Search**.  
        The items that match the search criteria are displayed in the grid by Code, Additional Codes, and Description.  
        ii. From the **Selection** section, select the item.  
        iii. Click **Save**.  

    **Customer Order Condition**

    **Note:** The Customer Order Condition fields are not supported in this version.

    a. In the **Transaction Maximums** section, in the **Amount** field, enter the maximum transaction amount allowed in the customer order. If exceeded, the business rule is triggered.

    b. In the **Quantity** field, enter the maximum number of items allowed in the customer order. If exceeded, the business rule is triggered.

    c. In the Loyalty Card Exists section from the **Includes Loyalty Card** drop-down list, select the relevant option:

    * Includes / Excludes Loyalty Card – indicates that a notification is always prompted on the POS regardless if a loyalty card was added to the transaction.

    * Includes Loyalty Card – indicates that a notification is only prompted on the POS if a loyalty card was added to the transaction.

    * Excludes Loyalty Card – indicates that a notification is only prompted on the POS if no loyalty card was added to the transaction.

8. Select the **Actions Tab**.

9. From the **Action Type** drop-down list, select Approval Required.

10. From the **Message** drop-down list, select the Manager Approval message.

    You can view the messages after linking it to the BRM, create a new message on the fly, or edit an existing message. For details on Messages, see Messages

11. From the **Roles** drop-down list, select the role with the privileges required by the person who is approving the activity.
**Note:** The **Roles** field is not supported in this version.

12. From the **Scope** drop-down list, select the relevant options:

    * **Per Line** – to specify that the business rule is always triggered.

    * **Cart** – to specify that the business rule is only triggered once per transaction.

        **Note:** The **Scope** field is not supported in this version.

13. Click **Save** to save the Business Rule.

### Configuring a Void Transaction BRM

The **Void Transaction** rule evaluates voided transactions.

This scenario describes how to set up a Void Transaction Business Rule with Manager Approval.

1. Browse to Sales Rules/Business Rules

2. Click **+ Add Business Rule**. The New Business Rule screen is displayed.

3. In the **Name** field enter Void Transaction.

4. From the **Type** drop-down list, select **Void Transaction**.

5. Click the **Apply only if transaction contains authorized online** option if you want to apply the business rule only to transactions that include authorized online items.

6. (Optional) define each of the following according to your requirements:

    **Location Condition**

    a. In the Included Locations field click the + sign.

    b. In the left pane of the form, in the Search field, search for the location that you are including by entering the name of the full or partial name of the location and press Enter. The location is listed in the left pane.

    Or

    From the left pane, select the checkbox of the Root to include all locations, or select the checkboxes next to the locations you wish to include.

    The selected locations are displayed in the right pane under the Included Selections.

    The Locations not included are displayed in the Excluded Selections

    c. Click **Save**.

    The Included Locations field displays the locations selected, i.e., the rule applies to these locations.

    The Excluded Locations field displays the locations excluded, i.e., the rule does not apply to these locations.

    **Touchpoint Groups Condition**

    From the Touchpoint Groups, select the relevant option:

    * To apply the business rule to all touchpoint groups, select A**pply to All**.

        Or

    * To apply the business rule to a specific touchpoint group, select **Selected Groups**.

    From the **Included Groups** drop-down list, select the groups you wish to apply the business rule.

    **Product Condition**

    a. From the **Apply To** drop-down list, select Sale item only.

    b. From the **Groups** drop-down list, select the item groups to which you are associating the Business Rule.

    c. From the **Category** drop-down list, select the categories to which are associating the Business Rule.

    d. From the **Products** field, click the + sign. The Browse or Look Up Item form is displayed.

    e. Search for the product as follows:  
        i. In the **Item** field, enter the full or partial name of the item.  
        ii. Select the **Exact Match** option to indicate that the system must retrieve the exact name of the item entered.  
        Or  
        Search by Category, from the **Category** drop-down list, select a category.  
        iii. Click **Search**.  
        The items that match the search criteria are displayed in the grid by Code, Additional Codes, and Description.  
        iv. From the **Selection** section, select the item.  
        v. Click **Save**.  

    **Customer Order Condition**

    **Note:** The Customer Order Condition fields are not supported in this version.

    a. In the **Transaction Maximums** section, in the **Amount** field enter the maximum transaction amount allowed in the customer order. If exceeded, the business rule is triggered.

    b. In the Quantity field enter the maximum number of items allowed in the customer order. If exceeded, the business rule is triggered.

    c. In the Loyalty Card Exists section from the **Includes Loyalty Card** drop-down list, select the relevant option:

    * Includes / Excludes Loyalty Card – indicates that a notification is always prompted on the POS regardless if a loyalty card was added to the transaction.

    * Includes Loyalty Card – indicates that a notification is only prompted on the POS if a loyalty card was added to the transaction.

    * Excludes Loyalty Card – indicates that a notification is only prompted on the POS if no loyalty card was added to the transaction.

7. Select the **Actions Tab**.

8. From the **Action Type** drop-down list, select Approval Required.

9. From the **Message** drop-down list, select the Manager Approval message.
You can view the messages after linking it to the BRM, create a new message on the fly, or edit an existing message. For details on Messages, see Messages.

10. From the **Scope** drop-down list, select the relevant options:

* **Per Line** – to specify that the business rule is always triggered.

* **Cart** – to specify that the business rule is only triggered once per transaction.

    **Note:** The **Scope** field is not supported in this version.

11. Click **Save** to save the Business Rule.

### Configuring a Product BRM

The **Product** rule evaluates the sale of products during a transaction.

**This scenario describes how to set up a Product Business Rule.**

1. Browse to Sales Rules/Business Rules

2. Click **+ Add Business Rule**. The *New Business Rule* screen is displayed.

3. In the **Name** field enter Product.

4. From the **Type** drop-down list, select **Product**.

5. Click the arrow to open the Product Condition.

    a. From the **Apply To** drop-down list, select Sale item only.

    b. From the **Groups** drop-down list, select the item groups to which you are associating the Business Rule.

    c. From the **Category** drop-down list, select the categories to which are associating the Business Rule.

    d. From the **Products** field, click the **+** sign. The Browse or Look Up Item form is displayed.

    e. Search for the product as follows:
        i. In the **Item** field enter the full or partial name of the item.  
        ii. Select the **Exact Match** option to indicate that the system must retrieve the exact name of the item entered.  
        Or  
        Search by Category, from the **Category** drop-down list, select a category.  
        iii. Click **Search**.  
        The items that match the search criteria are displayed in the grid by Code, Additional Codes, and Description.  
        iv. From the **Selection** section, select the item.  
        v. Click **Save**.  

6. (Optional) define each of the following according to your requirements:

    **Location Condition**

    a. In the Included Locations field click the + sign.

    b. In the left pane of the form, in the Search field, search for the location that you are including by entering the name of the full or partial name of the location and press Enter. The location is listed in the left pane.

    Or

    From the left pane, select the checkbox of the Root to include all locations, or select the checkboxes next to the locations you wish to include.

    The selected locations are displayed in the right pane under the Included Selections.

    The Locations not included are displayed in the Excluded Selections

    c. Click Save.

    The Included Locations field displays the locations selected, i.e., the rule applies to these locations.

    The Excluded Locations field displays the locations excluded, i.e., the rule does not apply to these locations.

    **Touchpoint Groups Condition**

    From the Touchpoint Groups, select the relevant option:

    * To apply the business rule to all touchpoint groups, select **Apply to All**.

        Or

    * To apply the business rule to a specific touchpoint group, select **Selected Groups**.

    From the **Included Groups** drop-down list, select the groups you wish to apply the business rule.

    **Customer Order Condition**

    **Note:** The Customer Order Condition fields are not supported in this version.

    a. In the **Transaction Maximums** section, in the **Amount** field enter the maximum transaction amount allowed in the customer order. If exceeded, the business rule is triggered.

    b. In the Quantity field enter the maximum number of items allowed in the customer order. If exceeded, the business rule is triggered.

    c. In the Loyalty Card Exists section from the **Includes Loyalty Card** drop-down list, select the relevant option:

    * Includes / Excludes Loyalty Card – indicates that a notification is always prompted on the POS regardless if a loyalty card was added to the transaction.

    * Includes Loyalty Card – indicates that a notification is only prompted on the POS if a loyalty card was added to the transaction.

    * Excludes Loyalty Card – indicates that a notification is only prompted on the POS if no loyalty card was added to the transaction.

7. Select the **Actions Tab**.

8. From the **Action Type** drop-down list, select **Prompt for Confirmation**.

9. From the Message drop-down list, select the ConfirmationRequest message.

    You can view the messages after linking it to the BRM, create a new message on the fly, or edit an existing message. For details on Messages, see Messages.

10. From the **Scope** drop-down list, select the relevant options:

* **Per Line** – to specify that the business rule is always triggered.
* **Cart** – to specify that the business rule is only triggered once per transaction.

    **Note:** The **Scope** field is not supported in this version.

11. Click **Save** to save the Business Rule.

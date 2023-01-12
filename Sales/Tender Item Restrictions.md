## Tender Item Restrictions

**Note:** Currently, you can only define a Tender Item Restriction in the CCM UI with the Display tender Balance on set to None. Other options are available by the API.

**Tender Item Restrictions** configure an item eligibility policy to:

* Prohibit paying for selected items or item hierarchies using a specific tender, e.g., vouchers cannot be used to purchase cigarettes and alcohol.

* Allow paying for selected items using a specific tender, e.g., Starbucks gift card can be used to purchase Starbucks items only.

The link between tenders and items should be a many-to-many relationship.

### Configuring a Tender Item Restriction

The following example shows how to set up a Tender Item Restriction that prohibits the customer to purchase specific items with an EBT tender.

1. Browse to Sales/Tendering/Tender Item Restrictions.
2. Click **+Add Tender Item Restriction**.
3. In the **Name** enter the name of the Tender Item Restriction.
4. From the **Location** drop-down list, select the store(s) in which the Tender item restriction is supported.  

    a. To search for a store, in the Type to Search field enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.  

    Or  

    From the left pane, select the checkboxes next to each store linked to the data pattern.

    All stores selected are displayed in the Selections in the right pane.

    b. Click **Save** to save the selected stores.

5. From the Touchpoint Groups drop-down list, select the Touchpoint group to which the tender item restriction is associated.
6. In the **Display Tender Balance On Total** select None.
7. From the **Tenders** drop-down list, select the tender(s) you are restricting. E.g., select the EBT tender to indicate that it cannot be used to purchase specific items.
8. Select the **ProhibitTenderFor** option.
9. In the **Select Products** field, click the + icon and select the products that cannot be paid for with the selected tender.
10. Click **Save**.

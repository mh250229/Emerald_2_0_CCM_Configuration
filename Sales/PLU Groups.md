## PLU Groups

**PLU Groups** comprise of items that are grouped for easy selection and recognition, e.g., heavy items, items with no barcodes, fruit, vegetables, bakery products and so on.  For example, a customer purchases a carton of Diet Cokes. The carton is too big to pick up to enable the cashier to scan the barcode, therefore, the cashier can select the item from the relevant PLU Group. Sub groups can be defined within PLU Groups, and add items to the sub groups.  

When a PLU Group is selected at a touchpoint, e.g., POS, Self Checkout, etc., a screen with buttons is displayed. Each button represents a PLU Group, and displays the PLU Group name as well as an image to symbolize the PLU Group.  

PLU Groups are set up for specific locations and then linked to different PLU Menus.

**Note:** Currently you can create the PLU Groups in the UI, but only add your PLU Groups to PLU Menus via the Emerald API.  

The following flows show examples of how to set up PLU Groups, PLU Groups with Sub Groups, and Add items to PLU Groups.

### Configuring PLU Groups

1. Browse to Sales/Items/PLU Groups.
2. Click **+ Add New PLU Group**. The New PLU Groups screen is displayed.
3. In the **Name** field, enter the name of the PLU Group, for example, Fruits.
4. In the **Description** field, enter a description of the PLU Group.
5. (Currently not supported) Click the Globe Icon to add the description of the group in additional languages.  

    a. From the **Language** drop-down list, select the relevant language/culture.

    b. In the **Value** field, enter a description in the select language.

    c. Click **Save**.

6. Click **Add Image** ![Add Image Button](/Images/addimagebutton.png).
7. Browse to the folder in which you save all your PLU Group images.
8. Select an image. The image is displayed.

    ![Fruit Group Image](/Images/FruitGroupImage.png)

9. From the **Location** drop-down list, select the store(s) in which the PLU Groups is supported.

    a. To search for a store, in the Type to Search field, enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.

    Or

    From the left pane, select the checkboxes next to each store linked to the data pattern.
    All stores selected are displayed in the Selections in the right pane.

    b. Click **Save** to save the selected stores.

You can add items to the PLU Group, or Sub Groups and Items to the PLU Group.

### Configuring PLU Groups with PLU Sub Groups

1. Create a PLU Group, see Configuring PLU Groups above.

    Or

    From the PLU Groups screen, click the pencil icon in the line of the PLU Group to which you are adding a Sub Group.

    ![Fruit Group Image](/Images/FruitGroupImage.png)

2. Click **PLU Groups**. The **Add New PLU Subgroup** form is displayed.

    ![Add New PLU Sub Group Form](/Images/addnewplusubgroupform.png)

    **To add an existing PLU Group as a Sub Group to the PLU Group:**  
    a. Select the **Existing PLU Group** option.

    b. From the PLU Groups, select the PLU Groups you adding as Sub Groups.

    ![Add New PLU Sub Group Form Selected](/Images/addnewplusubgroupformselected.png)  
    c. Click **Add**. The Sub Group is added to the PLU Group you are creating.

    ![Add New PLU Sub Group Form Selected](/Images/addplugroupform.png)  
    d. Repeat the steps above to add additional existing PLU Groups to the Sub Group.

    **To add a new PLU Group as a Sub Group to the PLU Group:**  
    a. Select the **New PLU Group** option.

    ![Add New PLU Sub Group Form Selected](/Images/newplugroupoption.png)  
    b. From the **Location** drop-down list, select the store(s) in which the PLU Groups is supported.

    c. In the **Name** field, enter the name of the Sub Group.

    d. Click **Add Image** ![Add New PLU Sub Group Form Selected](/Images/addimagebutton.png).

    e. Browse to the folder in which you save all your PLU Group images.  
    f. Select an image. The image is displayed.

    g. (Currently not supported) Click the **Globe** icon to add the description of the group in additional languages.  
        i. From the **Language** drop-down list, select the relevant language/culture  
        ii. In the **Value** field, enter a description in the select language.
  
    h. Click **Add**.

    ![Add New PLU Group Screen](/Images/addnewplugroupscreen.png)

3. To add additional **Sub Groups**, click ![Add New PLU Group Button](/Images/addnewplugroupbutton.png).

    ![Add New PLU Group Existing PLU Group](/Images/AddNewPLUSubgroupExistingpluGroup.png)

4. Repeat the steps above to add each Sub Group.  
    For example:

    ![PLU Sub Group Screen](/Images/plusubgroupsscreen.png)

### Adding Items to PLU Groups / Sub Groups

1. Create a PLU Group and/or Sub Groups. See Configuring PLU Groups and Configuring PLU Groups with PLU Sub Groups above.

    Or

    Open the PLU Groups screen, click the pencil icon in the line of the PLU Group or PLU Sub Group to which you are adding a Sub Group.

    ![PLU Group Screen](/Images/plugroupsscreen.png)

2. Click **PLU Items**. The **Browse or Look Up Item** screen is displayed.  
    a. Search for the items you are adding to the PLU Group. See Browse or Look Up Item Screen for details on how to use this form.

    ![Browse Or Look Up Item Screen](/Images/browseorlookupitemscreen.png)  
    b. Select the items:

    ![Browse Or Look Up Item Selected Screen](/Images/browseorlookupitemselectedscreen.png)  
    c. Click **Save**. The items are added to the PLU Group as follows:

     ![PLU Group Items Added Screen](/Images/plugroupitemsaddedscreen.png)

3. To select the Additional Code for the item, click the pencil icon in the line.

    ![Additional Codes Screen](/Images/additionalcodesscreen.png)

4. From the drop-down list, select the Additional Code.

5. Click ![Save Icon](/Images/saveicon.png) to save the Additional Code.

6. Click **Save**.
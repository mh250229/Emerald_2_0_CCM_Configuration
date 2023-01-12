# WIC CVB Product Mapping

**Note:** There is no Base Configuration for WIC CVB Product Mapping.

This process describes how to map a CVB item imported into the store in an APL file, to an item in the store catalog. 

## Mapping a CVB Item

For example, Fresh Raspberries included in the APL list are mapped to the ID code of Raspberries Fresh from Farm in the store catalog. When a customer purchases ‘Raspberries Fresh from Farm’, the system identifies the item, and then matches the Item Code to the item in the APL list, and validates that the item is eligible for WIC.

Scenario:

The following APL products are defined for the Agency ‘Virginia’:

|**Product Code**|**Product Name**|**Mapped Catalog Barcode**|**Mapped Product Name**
|-----|-------|-------|------|
|000000000003000|APPLES Alkmene | | |
|000000000004734|PUMPKIN Mini | | |
|000075030157800|Fresh RASPBERRIES|123456789012345|RASPBERRIES Fresh from Farm|

1. Browse to Sales/US WIC Tendering/WIC CVB Product Mapping.

2. From the **Agency** drop-down list, select the WIC agency responsible for the business unit, e.g., Virginia. The APL products defined for the Agency ‘Virginia’ are displayed in the grid.  

    a. Select **Show All** to show all the items defined for the Agency Virginia.  

    b. Select **Mapped** to only show the item mapped for the Agency Virginia. 

    c. Select **Unmapped** to only show the items that are not mapped for the Agency Virginia.  

    By default **Show All** is selected. In the APL Products section view all the items defined for the Agency Virginia. (Optional) From the Sub-category drop-down list, select the item sub-category of the item you want to map.

3. Optional) In the **Item Code or Description** field, enter the full or partial item code or description of the item you want to map.  
    In this scenario, the Fresh Raspberries have a badge **‘Mapped’** next to the item indicating that they are mapped.  
    If there are more than 500 products, the system prompts an error:  
    *‘Displaying only the first 500 products of search results.*  
    *Please refine the criteria to see more results.’*

4. In the **APL Products** panel select an APL Product line for example, select the Fresh Raspberries line, it is highlighted with a purple background. In the **Mapped Catalog Products** panel on the right-side of the screen view the product details, e.g., **Barcode** and **Product Name**. If the **Checkbox** is selected, it indicates that this product is mapped.  
To remove the mapping, in the **Mapped Catalog Products** section select the **X** at the end of the row. The system prompts: There are currently no products that have been mapped to the selected APL product.  
The **Mapped** badge in the APL Products panel next to the Fresh Raspberries is removed.

5. To add a product, from the **APL Products** panel, select the line of the product you are mapping, e.g., select the PUMPKIN Mini line.

6. Select **Add Product**. Select the catalog items you are mapping to the PUMPKIN Mini APL item. The selected products are displayed under the **Mapped Catalog Products** section.

7. Select **Save**.  
If an item you selected is already mapped, the system prompts an error: ‘Product nnnnnn + name is already mapped.  
The Pumpkin Mini line in the **APL Products** panel is displayed with the **Mapped** badge indicating that it is mapped to catalog items.

8. Repeat to map additional catalog items to the APL item.

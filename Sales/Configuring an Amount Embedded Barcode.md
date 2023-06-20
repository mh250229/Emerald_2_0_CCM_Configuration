### Configuring an Amount Embedded Barcode

The following example shows how to set up an Amount Embedded Barcode:120000221000 for a weight item.

1. Browse to Sales/Barcodes/Data Pattern.
2. Click **+ Add Data Pattern**. The **New Data Patterns** screen is displayed.
3. In the **ID** field, enter the Data Pattern ID.
4. In the **Description** field, enter the name of the data pattern, e.g., Amount Embedded
5. From the **Location** drop-down list, select the store(s) in which the data pattern is supported.  

    a. To search for a store, in the Type to Search field, enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.

    Or

    From the left pane, select the checkboxes next to each store linked to the data pattern.

    All stores selected are displayed in the Selections in the right pane.

    b. Click **Save** to save the selected stores.

6. From the **Type** drop-down list, select the data pattern type, e.g., **Item**.
7. In the **General** tab, select the **Prefix Length** option (displayed by default).
8. In the **Length** field, enter the total length of the data pattern, e.g., 12.
9. In the **Decoded Prefix Ranges** section click **+Add New Prefix**.  
 In the **Fixed Amount** field, enter 2.
10. Click the **Validators** option.
11. In the **Check Digit** option click **+ Add New**.

    a. Click **+ Add New Check Digit**.

    b. In the **Offset** field, enter 12.

    c. From the **Algorithm** drop-down list, select UPC.

    d. In the **Position** field, enter the starting position of the range of digits in the data pattern used to calculate the check digit. This check digit validates the item, e.g., 1.

    e. In the **Length** field, enter the number of check digits in the check digit range, e.g., enter 11

12. Select the **Content** tab. The parameters relevant to define an Item barcode are displayed in the Select Parameters section.

    a. From the left pane, click the **Item Code** option. The **Item Code** section is displayed in the right pane, define the parameters:

    * Select **Manipulated**
    * In the **Position** - enter 1
    * In the **Length** – enter 6
    * In the **Suffix** – enter 00000
    * Set the **Strip Leading Zeros** slider to No.

    b. From the left pane, click the **Item Amount** option. The **Item Amount** section is displayed in the right pane, define the parameters:

    * **Position** field – enter 7  
    * **Length** field – enter 5  
    * **Decimals** field – enter 2

13. Click **Save**.

### Configuring an EAN13 Barcode

The following example shows how to set up an Amount Embedded Barcode: 1300029910000  
Fixed Prefix - 13  
Item Code – 299  

1. Browse to Sales/Barcodes/Data Pattern.
2. Click **+ Add Data Pattern**. The **New Data Patterns** screen is displayed.
3. In the **ID** field, enter the Data Pattern ID.
4. In the **Description** field, enter the name of the data pattern, e.g., Amount Embedded
5. From the **Location** drop-down list, select the store(s) in which the data pattern is supported.  

    a. To search for a store, in the Type to Search field, enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.  

    Or  

    From the left pane, select the checkboxes next to each store linked to the data pattern.  
    All stores selected are displayed in the Selections in the right pane.  

    b. Click **Save** to save the selected stores.

6. From the **Type** drop-down list, select the data pattern type, e.g., **Item**.
7. In the **General** tab, select the **Prefix Length** option (displayed by default). 
8. In the **Length** field, enter the total length of the data pattern, e.g., 13.
9. In the **Decoded Prefix Ranges** section add a few options:

    a. Click **+Add New Prefix**. In the **From** field, enter 00 and in the **To** field enter the prefix 01.

    b. Click **+Add New Prefix**. In the **From** field, enter 03 and in the **To** field enter the prefix 19.

    c. Click **+Add New Prefix**. In the **From** field, enter 30 and in the **To** field enter the prefix 97.

10. In the **Check Digit** option click **+ Add New**:

    a. Click **+ Add New Check Digit**.

    b. In the **Offset** field, enter 13.

    c. From the **Algorithm** drop-down list, select UPC.

    d. In the **Position** field, enter the starting position of the range of digits in the data pattern used to calculate the check digit. This check digit validates the item, e.g., 11.

    e. In the **Length** field, enter the number of check digits in the check digit range, enter 12.

11. Select the **Content** tab. The parameters relevant to define an Item barcode are displayed in the Select Parameters section.  
a. From the left pane, click the **Item Code** option. The **Item Code** section is displayed in the right pane, define the parameters:
    * Select **Position Length**
    * In the **Position** - enter 1
    * In the **Length** – enter 12
    * Set the **Strip Leading Zeros** slide to Yes.
12. Click **Save**.

### Configuring a UPCA Barcode

The following example shows how to set up a UPCA barcode.  
For example:  
**042100005264**  
Entity Type – Item  
DataPattern ID – UPCA   
Key = Code, Value=**4210000526**  

1. Browse to Sales/Barcodes/Data Pattern.
2. Click **+ Add Data Pattern**. The **New Data Patterns** screen is displayed.
3. In the **ID** field, enter the Data Pattern ID.
4. In the **Description** field, enter the name of the data pattern, e.g., UPCA.
5. From the **Location** drop-down list, select the store(s) in which the data pattern is supported.

    a. To search for a store, in the Type to Search field, enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.

    Or

    From the left pane, select the checkboxes next to each store linked to the data pattern.
    All stores selected are displayed in the Selections in the right pane.

    b. Click **Save** to save the selected stores.

6. From the **Type** drop-down list, select the data pattern type, e.g., **Item**.
7. In the **General** tab, select the Prefix Length option (displayed by default).
8. In the **Length** field, enter the total length of the data pattern, e.g., 12.
9. In the **Decoded Prefix Ranges** section click **+Add New Prefix**.  
In the **From** field, enter 6 and in the **To** field, enter 8.
10. In the **Check Digit** option, click **+ Add New**

    a. Click **+ Add New Check Digit**.

    b. In the **Offset** field, enter 12.

    c. From the **Algorithm** drop-down list, select UPC.

    d. In the **Position** field, enter the starting position of the range of digits in the data pattern used to calculate the check digit. This check digit validates the item, e.g., 1.

    e. In the **Length** field, enter the number of check digits in the check digit range, e.g., 11

11. Select the **Content** tab. The parameters relevant to define an Item barcode are displayed in the Select Parameters section.  
a. From the left pane, click the **Item Code** option. The **Item Code** section is displayed in the right pane, define the parameters:
    * Select the **Position Length** option.
    * In the **Position** - enter 1
    * In the **Length** – enter 11
    * Set the **Strip Leading Zeros** slider to Yes.
13. Click **Save**.

#### Configuring a Coupon UPC Type Data Pattern

The following example shows how to set up a Coupon UPC type data pattern.

1. Browse to Sales/Barcodes/Data Pattern.
2. Click **+ Add Data Pattern**. The **New Data Patterns** screen is displayed.
3. In the **ID** field, enter the Data Pattern ID.
4. In the **Description** field, enter the name of the data pattern, e.g., Coupons.
5. From the **Location** drop-down list, select the store(s) in which the data pattern is supported.  

    a. To search for a store, in the Type to Search field, enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.  

    Or

    From the left pane, select the checkboxes next to each store linked to the data pattern.  
    All stores selected are displayed in the Selections in the right pane.  

    b. Click **Save** to save the selected stores.

6. From the **Type** drop-down list, select the data pattern type, e.g., **Coupon**.
7. In the **General** tab, select the **Prefix Length** option (displayed by default).
8. In the **Length** field, enter the total length of the data pattern, e.g., 12.
9. In the **Decoded Prefix Ranges** section click **+Add New Prefix**.
10. In the **Fixed** field, enter a fixed prefix, e.g., 5.
11. In the **Validators** section in the **Check Digit** option click **+ Add New**

    a. Click **+ Add New Check Digit**.

    b. In the **Offset** field, enter 12.

    c. From the **Algorithm** drop-down list, select UPC.

    d. In the **Position** field, enter 1.  

    e. In the **Length** field, enter 11.
  
12. Select the **Content** tab. The parameters relevant to define a Coupon barcode are displayed in the Select Parameters section.
13. Define the following parameters:  

    a. From the left pane, click the **Coupon Prefix** option. The **Coupon Prefix** section is displayed in the right pane, define the parameters:

    * **Position** field – enter 1
    * **Length** field – enter 1
    * Set the **Strip Leading Zeros** slider to No  

    b. From the left pane, click the **Manufacturer Number** option. The Manufacturer Number section is displayed in the right pane, define the parameters:

    * **Position** field – enter 2.
    * **Length** field – enter 5
    * Set the **Strip Leading Zeros** slider to No.

    c. From the left pane, click the **Family Code** option. The **Family Code** section is displayed in the right pane, define the parameters.
  
    * **Position** field – enter 7.
    * **Length** field – enter 3
    * Set the **Strip Leading Zeros** slider to No.

    d. From the left pane, click the **Value Code** option. The **Value Code** section is displayed in the right pane, define the parameters.

    * **Position** field – enter 10.
    * **Length** field – enter 2
    * Set the **Strip Leading Zeros** slider to No.

    e. From the left pane, click the **Tender ID** option. The **Tender ID** section is displayed in the right pane, define the parameter.

    * **Fixed Value** – enter 60.

    f. From the left pane, click the **Coupon Type** option. The **Coupon Type** section is displayed in the right pane, define the parameter.

    * **Fixed Value** – enter Vendor.
14. Click **Save**.

### Configuring a Tender Type Data Pattern

The following example shows how to set up a Tender type data pattern.

1. Browse to Sales/Barcodes/Data Pattern.
2. Click **+ Add Data Pattern**. The **New Data Patterns** screen is displayed.
3. In the **ID** field, enter the Data Pattern ID.
4. In the **Description** field, enter the name of the data pattern, e.g., Credit Card.
5. From the **Location** drop-down list, select the store(s) in which the data pattern is supported.  

    a. To search for a store, in the Type to Search field, enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.

    Or

    From the left pane, select the checkboxes next to each store linked to the data pattern.  
    All stores selected are displayed in the Selections in the right pane.

    b. Click **Save** to save the selected stores.

6. From the **Type** drop-down list, select the data pattern type, e.g., **Tender**.
7. In the **General** tab, select the **Prefix Length** option (displayed by default).
8. In the **Length** field, enter the total length of the data pattern, e.g., 16.
9. In the **Decoded Prefix Ranges** section click **+Add New Prefix**.
10. In the **Fixed** field, enter a fixed prefix, e.g., 12. All data patterns linked to this data pattern group start will the same prefix.
11. Select the **Content** tab. The parameters relevant to define a Tender barcode are displayed in the Select Parameters section.
12. Define the following parameters:  

    a. From the left pane, click the **Card ID** option. The **Card ID** section is displayed in the right pane, define the parameters.

    * **Fixed Value** field – enter EPS_GiftCard.

    b. From the left pane, click the **Loyalty Account** option. The **Loyalty Account** section is displayed in the right pane, define the parameters.

    * **Position** field – enter 4
    * **Length** field – enter 13

    c. From the left pane, click the **Tender Code** option. The **Tender Code** section is displayed in the right pane, define the parameters.

    * **Fixed Value** field – enter 20

13. Click **Save**.

### Configuring a Driver License Barcode

This process describes how to set up a Regex data pattern to support scanning Driver Licenses to verify a customer’s age when validating Age Restriction rules.  

Drivers Licenses must comply with the American Association of Motor Vehicle Administrators (AAMVA) 2D barcode standards (from 2000). These Driver Licenses comprise a mandatory PDF417, 2D Barcode, which includes a data element containing the drivers date of birth.  

Date formats in Driver’s Licenses differ according to the state/country in which the license was issued. For example, the date format in Drivers licenses issued in the USA is MMDDCCYY, and the date format for Drivers Licenses issued in Canada is CCYYMMDD.  

Both date formats are supported. On scanning a Driver’s License after an Age Restriction rule is triggered in a transaction, the system identifies and extracts the date of birth and inserts the date in the correct format.
If the Date of Birth is not verified, an error message is displayed, and the item is not added to the transaction.  

The following example shows how to set up a driver license barcode.

1. Browse to Sales/Barcodes/Data Pattern.
2. Click **+ Add Data Pattern**. The New Data Patterns screen is displayed.
3. In the **ID** field, enter the Data Pattern ID.
4. In the **Description** field, enter the name of the data pattern, e.g., Driver License.
5. From the **Location** drop-down list, select the store(s) in which the data pattern is supported.  

    a. To search for a store, in the Type to Search field, enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.

    Or

    From the left pane, select the checkboxes next to each store linked to the data pattern.
    All stores selected are displayed in the Selections in the right pane.

    b. Click **Save** to save the selected stores.

6. From the **Type** drop-down list, select the data pattern type, e.g., **DriverLicense**.
7. In the **General** tab, select the **Regular Expression** option (displayed by default).
8. In the Regular Expression field, enter @ANSI*
9. Click **Save**.

### Configuring a Transaction Type Data Pattern

The following example shows how to set up a transaction type barcode.

1. Browse to Sales/Barcodes/Data Pattern.  
2. Click **+ Add Data Pattern**. The New Data Patterns screen is displayed.  
3. In the **ID** field, enter the Data Pattern ID.
4. In the **Description** field, enter the name of the data pattern, e.g., Transaction.
5. From the **Location** drop-down list, select the store(s) in which the data pattern is supported.  

    a. To search for a store, in the Type to Search field, enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.

    Or

    From the left pane, select the checkboxes next to each store linked to the data pattern.  
    All stores selected are displayed in the Selections in the right pane.

    b. Click **Save** to save the selected stores.

6. From the **Type** drop-down list, select the data pattern type, e.g., **Transaction**.
7. In the **General** tab, select the **Prefix Length** option (displayed by default).
8. In the **Length** field, enter the total length of the data pattern, e.g., 22.
9. In the **Decoded Prefix Ranges** section click **+Add New Prefix**.
10. In the **Fixed** field, enter a fixed prefix, e.g., 629. All data patterns linked to this data pattern group start will the same prefix.
11. In the **Encoding Prefix Ranges** section click **+ Add New Prefix**.
12. In the **Prefix** field, enter 629. 
13. In the **Requesting Service** enter **SaveTransaction**.
14. Select the **Content** tab. The parameters relevant to define a Transaction barcode are displayed in the Select Parameters section.
15. Define the following parameters:

    a. From the left pane, click the **Store Code** option. The **Store Code** section is displayed in the right pane, define the parameters.

    * **Position** field – enter 4
    * **Length** field – enter 5
    * Set the **Strip Leading Zeros** slider to Yes.

    b. From the left pane, click the **POS ID** option. The **POS ID** section is displayed in the right pane, define the parameters.

    * **Position** field – enter 8
    * **Length** field – enter 3
    * Set the **Strip Leading Zeros** slider to Yes

    c. From the left pane, click the **Transaction ID** option. The **Transaction ID** section is displayed in the right pane, define the parameters.

    * **Position** field – enter 11
    * **Length** field – enter 4
    * Set the **Strip Leading Zeros** slider to No

    d. From the left pane, click the **Originating Date** option. The **Originating Date** section is displayed in the right pane, define the parameters.

    * **Position** field – enter 15
    * **Type** field – enter MMDDYYYY
    * Set the **Strip Leading Zeros** slider to No.

16. Once you have defined all the relevant parameters, click **Save**.

### Configuring a Tax Exemption Type Data Pattern

The following example shows how to set up a Tax Exemption type barcode.

1. Browse to Sales/Barcodes/Data Pattern.
1. Click **+ Add Data Pattern**. The **New Data Patterns** screen is displayed.
1. In the **ID** field, enter the Data Pattern ID.
1. In the **Description** field, enter the name of the data pattern, e.g., Tax Exemption.
1. From the **Location** drop-down list, select the store(s) in which the data pattern is supported.  
a. To search for a store, in the **Type to Search** field, enter the full or partial name of the store. The stores that meet the criteria are displayed in the left pane.  
Or  
From the left pane, select the checkboxes next to each store linked to the data pattern.  
All stores selected are displayed in the Selections in the right pane.  
b. Click **Save** to save the selected stores.
1. In the **General** tab, select the **Prefix Length** option.
1. In the **Length** field, enter the total length of the data pattern, e.g., 19.
1. In the **Decoded Prefix Ranges** section click **+Add New Prefix**.
1. In the **Fixed** field, enter a fixed prefix, e.g., 298. All data patterns linked to this data pattern group start will the same prefix.
1. Select the **Content** tab. The parameters relevant to define a Transaction barcode are displayed in the Select Parameters section.
1. Define the following parameters:  
a. From the left pane, click the **Tax Exempt ID** option. The **Tax Exempt ID** section is displayed in the right pane, define the parameters.  
-- **Position** field – enter 4  
-- **Length** field – enter 8  
-- Set the **Strip Leading Zeros** slider to On  
b. From the left pane, click the **Expiry Date** option. The **Expiry Date** section is displayed in the right pane, define the parameters.  
-- **Position** field – enter 12  
-- **DateTimeFormat** field – yyyyMMdd
1. Once you have defined all the relevant parameters, click **Save**. 




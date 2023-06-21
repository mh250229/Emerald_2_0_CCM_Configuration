## Tendering

Tenders are methods of payment used in the stores. The following tender types are supported Cash, Credit/Debit, Vouchers, Checks, Gift Card, and eWIC.

Tenders are defined centrally. On creating a new tender, you can define a range of different tender criteria, and specify any relevant exceptions.

Tender Exceptions can also be defined to modify specific tender attributes in specific locations, and touchpoint groups. For example, specify that the drawer is always opened when paying with a Cash tender at the POS in one store and doesn't open in another store.

For a description of the fields, see the NCR Emerald 2.0 CCM Dictionary Version 1.4.0.

**Known Limitation-ULP:**  
The Promotion Engine only supports Tender Codes/Ids up to 2 digits. If a transaction contains a Tender configured with a Tender Code/Id greater than 2 digits, any promotions in the transaction are removed.

### Configuring a Cash Tender

#### Configuring a Cash Tender with an Open Amount

In this example, the cashier must enter the amount of cash given by the customer at the POS.

1. Browse to Sales/Tendering/Tender.
2. Click **+Add Tender**.
3. In the **Tender Code** enter the Tender Code Id.
4. In the **Tender Name** enter the name of the tender, e.g., Cash.
5. From the **Tender Type** drop-down list, select **Cash**.
6. Click the arrow in the **Basic Definitions** options.
7. In the **Open drawer**, select the **Always** option.
8. In the **Tendering amount required** option, select the **Open Amount** option.
9. Set the **Block Partial Payment** slider to Off.
10. In the **Payment Priority** field enter 0.
11. Click the arrow in the **Change Definitions** option.
12. Set the **Consolidate On Change** slider to Yes.
13. Set the **Disable Automatic Void** slider to No.
14. In the **Priority** field, enter 1.
15. From the **Tender / Select Tender** drop-down list, select **Cash**.
16. In the **Up to Amount** field, enter 100.
17. Click **Save**.

#### Configuring a Cash Tender with Suggested Amounts

In this example, different cash buttons are displayed at the POS, according to suggested options, for example, if you defined four suggested values, i.e., 1.00, 5.00, 10.00, and 20.00, and the balance due is $5.00, the options displayed are 5.00, 10.00, 15.00, 20.00. If the balance due is $15.00, the options displayed are 15.00, and 20.00.

1. Browse to Sales/Tendering/Tender.
2. Click **+Add Tender**.
3. In the **Tender Code** enter the Tender Code Id.
4. In the **Tender Name** enter the name of the tender, e.g., Cash Suggested Amounts.
5. From the **Tender Type** drop-down list, select **Cash**.
6. Click the arrow in the **Basic Definitions** options.
7. In the **Open drawer**, select the **Always** option.
8. In the **Tendering amount required** option, select the **Open Amount with Suggested Options** option.
9. In the grid, in row # 3, in the Value field, enter 1 and click in the field. The row is added to the grid.
10. In the grid, in row # 4, in the Value field, enter 5 and click in the field. The row is added to the grid.
11. In the grid, in row # 5, in the Value field, enter 10 and click in the field. The row is added to the grid.
12. In the grid, in row # 6, in the Value field, enter 20 and click in the field. The row is added to the grid.
13. Set the **Block Partial Payment** slider to No.
14. In the **Payment Priority** field enter 0.
15. Click the arrow in the **Change Definitions** option.
16. Set the **Consolidate On Change** slider to Yes.
17. Set the **Disable Automatic Void** slider to No.
18. In the Priority field, enter 1.
19. From the **Tender / Select Tender** drop-down list, select **Cash**.
20. In the **Up to Amount** field enter 100.
21. Click **Save**.

### Configuring a Check Tender

#### Configuring a Non ECC Check Tender

This scenario describes how to set up a Non ECC Check Tender.

In this example, the Non ECC tender is configured for the Check/Cheque tender. The check tender is a based on the non ECC authorization type.

1. Browse to Sales/Tendering/Tender.
2. Click **+Add Tender**.
3. In the **Tender Code** enter the Tender Code Id.
4. In the **Tender Name** enter the name of the tender, e.g., Non ECC North America Check.
5. From the **Tender Type** drop-down list, select **Check**.
6. Click the arrow in the **Basic Definitions** options.
7. In the **Open drawer**, select the **Always** option.
8. In the **Tendering amount required** option, select the I**mmediate Closing, Balance Due as Default** option.
9. Set the **Block Partial Payment** slider to No.
10. Leave the **Payment Priority** field blank.
11. Click the arrow in the **Tender Authorization** option.
12. From the **MICR Validator** drop-down list, select **NorthAmericaStandardCheckValidator**.
13. Click the arrow in the **Change Definitions** option.
14. Set the **Consolidate On Change** slider to No
15. Set the **Disable Automatic Void** slider to No.
16. In the **Priority** field enter 1.
17. From the **Tender** drop-down list, select **Cash**.
18. In the **Up to** field, enter 25.
19. Click **Save**.

#### Configuring a Personal Check Tender

1. Browse to Sales/Tendering/Tender.
2. Click **+Add Tender**.
3. In the **Tender Code** enter the Tender Code Id.
4. In the **Tender Name** enter the name of the tender, e.g., Personal Check.
5. From the **Tender Type** drop-down list, select **Check**.
6. Click the arrow in the **Basic Definitions** options.
7. In the **Open drawer**, select the **Always** option.
8. In the **Tendering amount required** option, select the **Open Amount, Balance Due as Default** option.
9. Set the **Block Partial Payment** slider to No.
10. In the **Payment Priority** field enter 0.
11. Click the arrow in the **Tender Authorization** option.
12. From the MICR Validator drop-down list select **Default Reward Tender** slider to No.
13. From the **MICR Validator** drop-down list, select **NorthAmericaStandardCheckValidator**.
14. Click the arrow in the **Change Definitions** option.
15. Set the **Consolidate On Change** slider to Yes.
16. Set the **Disable Automatic Void** slider to No.
17. In the **Priority** field enter 1.
18. From the **Tender** drop-down list, select **Cash**.
19. In the **Up to** field, enter 25.
20. Click **Save**.

### Configuring a Credit/Debit Tender

#### Configuring a Gift Card Tender

1. Browse to Sales/Tendering/Tender.
2. Click **+Add Tender**.
3. In the **Tender Code** enter the Tender Code Id.
4. In the **Tender Name** enter the name of the tender, e.g., Gift Card.
5. From the **Tender Type** drop-down list, select **Credit/Debit**.
6. Click the arrow in the **Basic Definitions** options.
7. In the **Open drawer**, select the **Never** option.
8. In the **Tendering amount required** option, select the **Immediate Closing Balance Dues as Default** option.
9. Set the **Block Partial Payment** slider to No.
10. In the **Payment Priority** field enter 1.
11. Click the arrow in the **Tender Authorization** option.
12. In the **Authorization Method** options, Process with EPS is selected by default.
13. In the **Tender EPS Reference**, enter **EPS_Giftcard** and click Enter.
14. Enter **GC** and click **Enter**.
15. Click the arrow in the **Specific Definitions** option.
16. Set the **Barcode Required** slider to Yes.
17. Click **Save**.

#### Configuring a Mastercard Tender

1. Browse to Sales/Tendering/Tender.
2. Click **+ Add Tender**.
3. In the **Tender Code** enter the Tender Code Id.
4. In the **Tender Name** enter the name of the tender, e.g., Mastercard.
5. From the **Tender Type** drop-down list, select **Credit/Debit**.
6. Click the arrow in the **Basic Definitions** options.
7. In the **Open drawer**, select the **Never** option.
8. In the **Tendering amount required** option, select the **Immediate Closing, Balance Due as Default** option.
9. Set the **Block Partial Payment** slider to No.
10. In the **Payment Priority** field enter 0.
11. Click the arrow in the **Tender Authorization** option.
12. In the **Authorization Method** options, Process with EPS is selected by default.
13. In the T**ender EPS Reference**, enter **EPS_Mastercard** and click **Enter**.
14. Enter **MC** and click **Enter**.
15. Click the arrow in the **Specific Definitions** option.
16. Set the **Barcode Required** slider to No.
17. Click **Save**.

#### Configuring an EBT Cash Tender

EBT (Electronic Benefits Tender).

1. Browse to Sales/Tendering/Tender.
2. Click **+Add Tender**.
3. In the **Tender Code** enter the Tender Code Id.
4. In the **Tender Name** enter the name of the tender, e.g., EBT Cash.
5. From the **Tender Type** drop-down list, select **Credit/Debit**.
6. Click the arrow in the **Basic Definitions** options.
7. In the **Open drawer**, select the **Never** option.
8. In the **Tendering amount required** option, select the **Immediate Closing, Balance Due as Default** option.
9. Set the **Block Partial Payment** slider to No.
10. In the **Payment Priority** field enter 78.
11. Click **Save**.

#### Configuring an EBT Food Stamps Tender

1. Browse to Sales/Tendering/Tender.
2. Click **+Add Tender**.
3. In the **Tender Code** enter the Tender Code Id.
4. In the **Tender Name** enter the name of the tender, e.g., EBT Food Stamps.
5. From the **Tender Type** drop-down list, select **Credit/Debit**.
6. Click the arrow in the **Basic Definitions** options.
7. In the **Open drawer**, select the **Never** option.
8. In the **Tendering amount required** option, select the **Immediate Closing, Balance Due as Default** option.
9. Set the **Block Partial Payment** slider to No.
10. In the **Payment Priority** field enter 79.
11. Click the arrow in the **Specific Definitions** option.
12. Set the **Barcode Required** slider to No.
13. Click **Save**.

#### Configuring an InComm Tender

1. Browse to Sales/Tendering/Tender.
2. Click **+Add Tender**.
3. In the **Tender Code** enter the Tender Code Id.
4. In the **Tender Name** enter the name of the tender, e.g., InComm OTC.
5. From the **Tender Type** drop-down list, select **CreditDebit**.
6. Click the arrow in the **Basic Definitions** options.
7. In the **Open drawer**, select the **Never** option.
8. In the **Tender amount required**, select the **Immediate Closing, Balance Due as Default** option.
9. In the **Payment Priority** field enter 99.
10. Click the arrow in the **Tender Authorization** option.
11. In the **Authorization Method** options, **Process with EPS** is selected by default.
12. In the **Tender EPS Reference**, enter **InComm** and click Enter.
13. Click the arrow in the **Specific Definition** option.
14. From the **Customer Program Type** drop-down list, select **InComm**.
15. Click **Save**.


### Configuring a Reward Tender

#### Configuring a Digital Coupon Tender

1. Browse to Sales/Tendering/Tender.
2. Click **+Add Tender**.
3. In the **Tender Code** enter the Tender Code Id.
4. In the **Tender Name** enter the name of the tender, e.g., Digital Coupon.
5. From the **Tender Type** drop-down list, select **Reward**.
6. Click the arrow in the **Basic Definitions** options.
7. In the **Open drawer**, select the **Never** option.
8. In the **Tender amount required**, select the **Immediate Closing, Balance Due as Default** option.
9. In the **Payment Priority** field enter 0.
10. Click the arrow in the **Specific Definition** option.
11. In the **Reward Type Mapping** field, enter DIGITAL_MANUFACTURER_COUPON and DIGITAL_STORE_COUPON.
12. Click **Save**.

#### Configuring a Manufacturer Coupon Tender

1. Browse to Sales/Tendering/Tender.
2. Click **+Add Tender**.
3. In the **Tender Code** enter the Tender Code Id.
4. In the **Tender Name** enter the name of the tender, e.g., MFR Coupon.
5. From the **Tender Type** drop-down list, select **Reward**.
6. Click the arrow in the **Basic Definitions** options.
7. In the **Open drawer**, select the **Always** option.
8. In the **Tender amount required**, select the **Immediate Closing, Balance Due as Default** option.
9. In the **Payment Priority** field enter 0.
10. Click the arrow in the **Specific Definition** option.
11. Set the **Default Reward Tender** slider to Yes.
12. In the **Reward Type Mapping** field, enter GS1_MANUFACTURER_COUPON and UPC5_COUPON.
13. Click **Save**.


### Configuring an eWIC Tender

#### Configuring an eWIC Tender 

1. Browse to Sales/Tendering/Tender.
2. Click **+Add Tender**.
3. In the **Tender Code** enter the Tender Code Id.
4. In the **Tender Name** enter the name of the tender, e.g., eWIC.
5. From the **Tender Type** drop-down list, select **eWIC**.
6. Click the arrow in the **Basic Definitions** options.
7. In the **Open drawer**, select the **Never** option.
8. Set the **Block Partial Payment** slider to No.
9. In the **Payment Priority** field enter 110.
10. Click the arrow in the **Tender Authorization** option.
11. In the **Authorization Method** options, **Process with EPS** is selected by default.
12. In the **Tender EPS Reference**, enter **EWIC** and click **Enter**.
13. Enter **EWeWic** and click **Enter**.
14. Click **Save**.


### Configuring a Voucher Tender

#### Configuring a Coinstar Voucher Tender 

1. Browse to Sales/Tendering/Tender.
2. Click **+Add Tender**.
3. In the **Tender Code** enter the Tender Code Id.
4. In the **Tender Name** enter the name of the tender, e.g., Coinstar Voucher.
5. From the **Tender Type** drop-down list, select **Voucher**.
6. Click the arrow in the **Basic Definitions** options.
7. In the **Open drawer**, select the **Always** option.
8. In the **Tender amount required**, select the **Open Amount, Balance Due as Default** option.
9. In the **Payment Priority** field enter 0.
10. Click the arrow in the **Specific Definition** option.
11. Set the **Barcode Required** slider to Yes.
12. Set the **Request for tendering** slider to Yes.
13. Click **Save**.

## Command Menu

**Note:** The following processes show examples of how to set up and edit Command Menus.

**Command Menus** defines the command menus which comprise the functions performed at the touchpoints. Each button at the touchpoint is a command. For example, Void, Refund, Cashback, Enter, OK are all commands. All commands are predefined in the system and a command menu is defined for each touchpoint state, i.e., No Sale Mode, Sale Mode, Tender Mode, and so on.

### Out of the Box Configuration

The following list of commands/states are provided out-of-the-box:

#### General Menu 

      'ApplyTransactionTaxExemptionCommand',
      'ApplyItemTaxExemptionCommand',
      'CancelItemFromLineItemCommand',
      'CancelLineItemCommand',
      'CancelCouponLineCommand',
      'CancelManualPromotionLineCommand',
      'DepartmentSaleCommand',
      'DepartmentReturnCommand',
      'EFTAdminMenuCommand',
      'EnhancedPriceOverrideCommand',
      'InterventionListCommand',
      'GoToSaleModeCommand',
      'LoyaltyAddCommand',
      'LoyaltyBalanceInquiryCommand',
      'ManualWeightCommand',
      'ManualPromotionCommand',
      'ManualSegmentState',
      'MergeTransactionCommand',
      'ModifyTareCommand',
      'OpenCashDrawerCommand',
      'OnlineItemBalanceQueryCommand',
      'OwnBagSelectionCommand',
      'PaidInCommand',
      'PaidOutCommand',
      'PaybackTendersCommand'
      'PreSalePriceOverrideCommand',
      'PriceQueryCommand',
      'PriceOverrideCommand',
      'RetrieveSelfScanTransactionCommand',
      'ResumeTransactionCommand',
      'ReprintCommand',
      'RepeatCommand',
      'RemoveCustomerFromTransactionCommand',
      'SetGetItemToReturnStateCommand',
      'SuspendTransactionCommand',
      'SetCancelItemStateCommand',
      'SearchCustomerCommand',
      'TopUpCommand',
      'TenderExchangeCommand',
      'VoidTransactionCommand',
      'VoidAllCouponsCommand',
      'VoucherBarcodeCommand',
      'VoidTenderCommand',
      'VoidCustomerProgramCommand',

#### States

* SaleTransactionCommands – Commands displayed on the sidebar during an active sale transaction
* ReturnTransactionCommands – Commands displayed on the sidebar during an active return transaction
* CouponModeCommands – Commands displayed in the action window when a coupon is selected in the EJ
* ItemsPostSaleCommands – Commands displayed in the action window when an item with a unit of measure Each is selected in the EJ during a Sale Transaction
* ReturnTransactionItemsPostSaleCommands – Commands displayed in the action window when an item is selected in the EJ during a Transaction Based Return
* ItemWithTareCommands – Commands displayed in the action window when a weighted item is selected in the EJ
* NoSaleTransactionCommands – Commands displayed on the sidebar when no active sale is taking place
* TenderTransactionCommands – Commands displayed on the sidebar when the current transaction is in the tendering state
* TenderDetailsViewCommands – Commands displayed in the action window when a tender or refund is selected in the EJ
* ANY state is used for command menus not tied to state.

### Configuring a Command Menu

A range of out-of-the-box base configurations to provide a starting point for configuring the system and a reference for editing command menus is supported. Adding new commands requires uploading only the new command offerings to avoid erasing any permissions on commands as configured by the customer.

This flow shows an example of how to configure a command menu displayed in No Sale mode at the POS.

1. Browse to Sales/Touchpoint Behavior/Command Menu.
1. Click **+ Add New Command Menu**. The **Add New Command Menu** screen is displayed.
1. In the **Name** field, enter the name of the command menu.
1. From the **Location** drop-down list, select the location, e.g., Texas.
1. From the **Touchpoint Groups** drop-down list, select the touchpoint group, e.g., SelfCheckout.
1. From the **Touchpoint Application** drop-down list, select the touchpoint application, e.g., POS.
1. From the **Menu Type** drop-down list, select the menu type, e.g., User.  
On hovering over the field tooltip, a popup screen shows where this menu type appears on the POS.
1. Make sure the **Active** toggle is enabled if you wish for this command menu to take effect as soon as the configuration is saved.
1. From the **State** drop-down list, select the state to which the commands you are configuring is associated. , e.g., NoSaleTransactionCommands.
1. From the **Commands** pane, drag and drop the commands you wish to add to this menu.:  
The commands are displayed on the POS in the order they are entered into the command window.
1. Continue to add all the commands you want.
1. To add a Command Group, click **+ Add New Command Group**. The **New Command Group** screen is displayed.
1. In the **Name** field, enter the name of the command group.
1. In the **Description** field, enter the description of the command group.
1. From the **Commands** section, select the command you want to add to the Command Group and drag it to the right pane.
1. Continue to add all the commands you want.
1. Click **Save**.

### Configuring a Command Menu

This flow shows an example of how to configure a new Payback command menu.

The Payback menu (Negative PLU Menu) can be found in the PLU Menu, but can also be accessed by clicking the Payback Tender Command from the General Command Menu when configured.

The Payback menu is configured similarly to other command menus, but a specific command menu structure is required for items to display as designed.

Updates to the Payback Tender Menu are applied to the POS on the next login by a user.

Unlike other command menus, the Payback Tender Menu has a field for the menu’s description. This is the text that is displayed at the top level of the PLU Menu next to other first level tabs. This description field cannot be edited in the CCM and must be set manually via Postman. Alternatively, a localized resource can be configured with the key Payback_Tenders. If neither is set, the default text is Payback Tenders.

1. Browse to Sales/Touchpoint Behavior/Command Menu.
1. Click **+ Add New Command Menu**. The **Add New Command Menu** screen is displayed.
1. In the **Name** field, enter the name of the command menu, Payback.
1. From the **Location** drop-down list, select the location.
1. From the **Touchpoint Groups** drop-down list, select the touchpoint group.
1. From the **Touchpoint Application** drop-down list, select the touchpoint application, e.g., POS.
1. From the **Menu Type** drop-down list, select the menu type, e.g., Payback.  
On hovering over the field tooltip, a popup screen shows where this menu type appears on the POS.
1. Make sure the **Active** toggle is enabled if you wish for this command menu to take effect as soon as the configuration is saved.
1. From the **State** drop-down list, select the state to which the commands you are configuring is associated. , e.g., Payback Menu.  
On selecting the Payback State, the **Add Item** and **Add Tender** commands are visible under the Commands area of the editor.  
![Add New Command Menu Screen](/Images/addnewconfigurationscreen.png)  
For items or tenders to be visible in the Payback Menu, they must be defined in a command group. Any command not part of the command group will not be displayed.
1. Click **+ New Command Group** to create the new command group.
1. In the **Name** field, enter a name for the command group.
1. In the **Description** field, enter a description. The name is displayed in the CCM and the description is what is displayed on the POS.
1. Drag and drop the **Add Item** and **Add Tender** commands into the new command group.
![New Command Group Screen](/Images/newcommandgroupscreen.png)  
Items are displayed on the POS in the order they are entered into the command group – the topmost item will be displayed on the top left of the command menu, proceeding left to right and onto the next row or page appropriately.
1. To add the ItemCode parameter to the Add Item command, in the Add Item row click  ![edit](/Images/edit.png) .  
The Add Item command requires a parameter to be set for the item to be displayed.  
If the itemCode parameter is not provided for an Add Item command, the command is ignored by the POS.  
An icon is not required for this command, the product URL configured in the catalog is used.
1. In the **Edit Add Item** screen, click **+ Add Another Parameter**.  
a. In the **Parameter Name** field enter Item Code.  
b. In the **Value** for the parameter, enter the item code for the required item as set in the retailer’s catalog.  
This is the only required parameter for an Add Item Command.  
c. Click Save.
1. To add the Tender Id parameter to the Add Tender command, in the Add Tender row click  ![edit](/Images/edit.png) .
The Add Tender command can either be set with:  
 -- A pre-set value for the voucher’s redemption or prompt the cashier to enter an open amount. The parameter is the tender Id for the tender the cashier wishes to redeem. This Id can be viewed in the Tenders screen in the CCM in the Sales/Tendering/Tender module. The tender Id must correspond to a Voucher tender and be the numeric Tender Code value.  
If a preset tender is required, continue to Step 17.  
-- An Open Amount - If an open amount is required, click Save.  
1. In the **Edit Add Tender** screen, click **+ Add Another Parameter**.  
a. In the **Parameter Name** field enter Tender Id.  
b. In the **Value** for the parameter, enter the tender code for the Voucher tender.  
c. Click Save.
1. Click Save.

### Configuring Permissions on a Command 

1. Using POSTMAN, open the following API.  
PUT:  
{{pos-config-url}}command-menu/command-offering/:touchPointApplication/:commandId
1. In the body of the JSON data, scroll-down to the Command on which you are enforcing permissions.
1. Set the allowBypassApproval parameter to true.
1. Run the API.  
For example:  
![POSTMAN API example](/Images/postmanapiexample.png)  
![POSTMAN API example](/Images/postmanapiexample2.png)
1. On logging in to the POS and selecting the defined command, the Approval Required screen is displayed.  
For example:  
![Approval Required screen](/Images/approvalrequired.png)
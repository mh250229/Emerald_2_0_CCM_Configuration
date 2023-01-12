## Command Menu

**Note:** The following processes show examples of how to set up and edit Command Menus. Since Command Menus are customized, the flows are not included in the Base Configuration.  
**Command Menus** defines the command menus which comprise the functions performed at the touchpoints. Each button at the touchpoint is a command. For example, Void, Refund, Cashback, Enter, OK are all commands. All commands are predefined in the system and a command menu is defined for each touchpoint state, i.e., No Sale Mode, Sale Mode, Tender Mode, and so on.

### Configuring a Command Menu

This flow shows an example of how to configure a command menu displayed in No Sale mode at the POS.

1. Browse to Sales/Touchpoint Behavior/Command Menu.
2. Click **+ Add New Command Menu**. The **Add New Command Menu** screen is displayed.
3. In the **Name** field, enter the name of the command menu.
4. From the **Location** drop-down list, select the location, e.g., Texas.
5. From the **Touchpoint Groups** drop-down list, select the touchpoint group, e.g., SelfCheckout.
6. From the **Touchpoint Application** drop-down list, select the touchpoint application, e.g., POS.
7. From the **Menu Type** drop-down list, select the menu type, e.g., User.
8. From the **State** drop-down list, select the state, e.g., NoSaleTransactionCommands.
9. From the **Commands** section, select the command you want to add and drag it to the right pane.
10. Continue to add all the commands you want.
11. To add a Command Group, click **+ Add New Command Group**. The **New Command Group** screen is displayed.
12. In the **Name** field, enter the name of the command group.
13. In the **Description** field, enter the description of the command group.
14. From the **Commands** section, select the command you want to add to the Command Group and drag it to the right pane.
15. Continue to add all the commands you want.
16. Click **Save**.

### Editing Command Menus

1. Browse to Sales/Touchpoint Behavior/Command Menu.
2. In the grid, select the row of the command menu you want to edit, and click the edit icon. The **Edit Command Menu** is displayed showing the commands in the selected menu.
3. To add a new command, in the **Commands** selection area, select the command you want to add to the menu and drag and drop the command into the right pane.
4. To edit a command, for example add a Tender Correction parameter to the Tender Exchange command, in the right pane, select the command you want to edit and click the edit icon. The **Edit <command name>** screen is displayed.
5. Select **+ Add Another Parameter**.
6. In the **Parameter Name** field, enter Tender Correction, and in the **Value** field, enter the command value e.g., 1.  
![Tender Exchagne Command Form](/Images/TenderExchangeCommandForm.png)
7. Select **Save**.
8. To delete a command, in the **Commands** selection area, select the command you want to delete from the menu and click X.
9. Click **Save**.

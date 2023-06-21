## Messages

The **Create New Message** option is used to create new messages, view or revise the details of messages previously defined in the system.

New messages can be created only from the module in which you want to use the message. For example, if you want to define a message to be displayed when a BRM is triggered, you must access the **Create New Message** screen from the Business Rules module.  

Once a new message is saved, the message is displayed in the Messages module.  

Previously defined messages can be viewed or edited, by accessing the Message form from the Messages module. The Messages form accessed in the Message module, displays the message details, however, only the fields that can be edited are enabled.

**Note:** Currently, Multi Languages are not supported in the CCM UI.

### Configuring Messages

From the **Message** drop-down list, select the relevant message. 

You can view the messages after linking it to the BRM, create a new message on the fly, or edit an existing message.

**To View the Message**

Click **View**. The View Message form is displayed. You can verify the message that is prompted on the POS.

**To Edit the Message**

1. To edit the message, click **Edit**. The Edit Message form is displayed.
2. Edit the **Title** as required.
3. In the **Message Body or Instructions**, edit the text as required.  
a. To add a dynamic attribute, e.g., display the maximum percentage in the message, from the left panel, under **Add Content**, click **Price Override**. The dynamic attributes are displayed.  
b. Select the **MaxPercentChange** attribute and drag it to the Message Body or Instructions adding it to your message.
4. To add the message in a different language, click **+ Add Language**.  
a. From the **Language** Drop-down list, select the language you are adding.  
b. In the **Title** field, enter the title of the message.  
c. In the **Message Body or Instructions** section enter the message text.

**To Create a New Message**

1. From the Message drop-down list, click **+Create New Message**. The Create New Message form is displayed.<BR>![Create New Message Form](/Images/createnewmessageform.png)

2. In the **Message Name** field, enter the name of the message.
3. From the **Language** Drop-down list, select the language of the message you are adding.
4. In the **Title** field, enter the title of the message.
5. In the **Message Body or Instructions** section enter the message text. <BR>
a. To add a dynamic attribute, e.g., display the maximum percentage in the message, from the left panel, under **Add Content**, click **Price Override**. The dynamic attributes are displayed.<BR>
b. Select the **MaxPercentChange** attribute and drag it to the Message Body or Instructions adding it to your message.
6. To add the message in a different language, click **+ Add Language**.<BR>
a. From the **Language** Drop-down list, select the language you are adding.<BR>
b. In the **Title** field, enter the title of the message.<BR>
c. In the **Message Body or Instructions** section enter the message text.
7. Click **Save**.

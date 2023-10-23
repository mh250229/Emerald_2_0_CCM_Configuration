# Configuring Manual Coupons

The following steps are required to work with Manual Coupons.

||||
|---------|----------|----------|
|Step 1|Set up the Manual Coupon Command|CCM/Services|
|Step 2|Adding the Manual Coupon Command to the Menu|CCM|
|Step 3|Set up the Manual Coupon Policy|CCM|
|Step 4|Define the promotion type|Services|
|

## Step 1 – Set up the Manual Coupon Command

This step includes:
* Adding the command
* (Optional) assigning permissions to the command, i.e., a role

1. Open the following service.  
*emerald-configuration.command-menu.command-offering.POS.ManualCouponCommand.json*

2. Define the following:
* Enter the command name
* Enter the state name
* Verify enabled is set to true
* Enter the allowed role
* Set the allowBypassApproval to true to give permissions to the role

**Example:**
{  
  "commandName": "Manual Coupon",  
           "states": [  
                {  
                    "state": "SaleTransactionCommands",  
                    "enabled": true  
                }  
],  
  "permissions": {  
    "allowedRoles": [  
      "EMERALD_POS_LOGIN"  
    ],  
    "allowBypassApproval": true  
  }  
}  

## Step 2 – Adding the Manual Coupon Command to the Menu

## Step 3 – Set up the Manual Coupon Policy

## Step 4 – Define the Manual Coupon Promotion Type


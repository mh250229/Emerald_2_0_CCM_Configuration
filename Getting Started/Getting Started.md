# Getting Started

## Signing in to Emerald CCM

1. Enter the web address.  
The Emerald CCM Sign in page is displayed:

![Emerald CCM Sign In Screen](/Images/EmeraldCCMSignInScreen.png)

2. In the Username and Password fields, enter your user name and password.
3. In the Organization field, enter the organization to which you are associated.
4. Click Submit. The Dashboard is displayed.

![Dashboard Screen](/Images/DashboardScreen.png)

## Role Permissions

The following roles need to be configured in order to successfully log in to the CCM.  

Roles can be assigned to users via the POST //security/role-grants/user-grants) API.  
Roles are created in Marketplace and can be defined for CCM domains, menus, and sub menus. Roles are defined for all retailers and cannot be defined for a specific retailer.

### CCM Configurator Role

* SELLING_CONFIG_VIEWER
* IMAGE_VIEWER
* IMAGE_WRITER
* R1_CATALOG_ADMINISTRATOR
* R1_CATALOG_VIEWER
* SELLING_CONFIG_ADMINISTRATOR
* SELLING_RESOURCE_CONSUMER
* NEP_ORGANIZATION_VIEWER
* NEP_ENTERPRISE_VIEWER
* SITE_ENTERPRISE_SETTING_READ
* SITE_READ
* NEP_TOKEN_EXCHANGER

### CCM Admin Role

The CCM ADMIN role grants users permissions to access, view and perform actions in all the CCM modules.  
However, you can create different user roles for each CCM user. Each role can contain permissions to access, view, and perform actions in specific modules in the CCM.  
Each role contains the CCM domain/menu/sub menu the user assigned to the role can access, as well as the actions the user can perform, e.g., ADMIN, VIEWER   
Users assigned to an ADMIN role have permissions to create/edit/view the specific domain/menu/sub menu.  
Users assigned to a VIEWER role only have permissions to view the specific domain/menu/sub menu.  
For example, users assigned to the Business Rule Viewer role only have permissions to view Business Rules in the CCM. They cannot create new rules or save modified business rules, unless they have ADMIN role from a higher level in the hierarchy (for exp. user has Rules ADMIN role or Sales ADMIN role).  
Users can access a domain or a menu, even if they have no explicit role to the domain/menu, if the user has a role to access any screen underneath (i.e., a lower level in the hierarchy).

### Domain Roles

Each role includes the Menus/Sub Menus in the Domain. Users assigned to a domain role have permissions to access all the Menus/Sub menus in the Domain.  
The following shows a list of the roles and the domains assigned to each role.  
Template role is: CCM_< gate >_ADMIN/VIEWER  

|**Role**|**Domains**|
|--------|----------|
|CCM_ORGANIZATION_ADMIN/CCM_ORGANIZATION_VIEWER|Organization|
|CCM_SALES_ADMIN/CCM_SALES_VIEWER|Sales|
|CCM_OPERATIONS_ADMIN/CCM_OPERATIONS_VIEWER|Operations|
|CCM_UTILITIES_ADMIN/CCM_UTILITIES_VIEWER|Utilities|

### Menu Roles

Each role includes the Sub Menus in the Menu. Users assigned to a Menu role have permissions to access all the Sub menus (screens) in the Menu.  
The following shows a list of the roles and the Menus assigned to each role.  
Template role is: CCM_< gate >_< menu >_ADMIN/VIEWER

|**Role**|**Menus**|
|--------|----------|
|CCM_SALES_TOUCHPOINTBEHAVIOR_ADMIN/VIEWER|Sales/Touchpoint Behavior|
|CCM_SALES_BARCODES_ADMIN/VIEWER|Sales/Barcodes|
|CCM_SALES_ITEMS_ADMIN/VIEWER|Sales/Items|
|CCM_SALES_RETURN_ADMIN/VIEWER|Sales/Return|
|CCM_SALES_RULES_ADMIN/VIEWER|Sales/Rules|
|CCM_SALES_TAX_ADMIN/VIEWER|Sales/Tax|
|CCM_SALES_TENDERING_ADMIN/VIEWER|Sales/Tendering|
|CCM_SALES_USWICTENDERING_ADMIN/VIEWER|Sales/US WIC Tendering|
|CCM_ORGANIZATION_CHAINLOCATIONS_ADMIN/VIEWER|Organization/Chain Locations|
|CCM_ORGANIZATION_TOUCHPOINTDEVICES_ADMIN/VIEWER|Organization/Touchpoint Devices|
|CCM_ORGANIZATION_TOUCHPOINTCATEGORIES_ADMIN/VIEWER|Organization/Touchpoint Categories|
|CCM_ORGANIZATION_CULTURE_ADMIN/VIEWER|Organization/Culture|
|CCM_ORGANIZATION_GENERAL_ADMIN/VIEWER|Organization/General|
|CCM_ORGANIZATION_BUSINESSDAY_ADMIN/VIEWER|Organization/Business Day|

### Screen Roles

The following roles are defined for Screens.

Template role is: CCM_< gate >_< menu >_< sub-menu/screen >_ADMIN/VIEWER

|**Role**|**Screens**|
|--------|----------|
|CCM_SALES_TOUCHPOINTBEHAVIOR_TENDERMENU_ADMIN/VIEWER|Sales/Touchpoint Behavior/Tender Menu|
|CCM_SALES_TOUCHPOINTBEHAVIOR_TOUCHPOINTBRANDING_ ADMIN/VIEWER|Sales/Touchpoint Behavior/Branding|
|CCM_SALES_TOUCHPOINTBEHAVIOR_COMMANDMENU_ADMIN/VIEWER|Sales/Touchpoint Behavior/Command Menu|
|CCM_SALES_TOUCHPOINTBEHAVIOR_TOUCHPOINTPARAMETERS_ ADMIN/VIEWER|Sales/Touchpoint Behavior/Touchpoint Parameters|
|CCM_SALES_BARCODES_DATAPATTERN_ADMIN/VIEWER|Sales/Barcodes/Data Pattern|
|CCM_SALES_ITEMS_ONLINEPURCHASEPROFILE_ADMIN/VIEWER|Sales/Items/Online Purchase Profile|
|CCM_SALES_ITEMS_PLUGROUPS_ADMIN/VIEWER|Sales/Items/PLU Groups|
|CCM_SALES_ITEMS_PLUMENUS_ADMIN/VIEWER|Sales/Items/PLU Menus|
|CCM_SALES_RETURN_RETURNPOLICIES_ADMIN/VIEWER|Sales/Return/Return Policies|
|CCM_SALES_RULES_AGERESTRICTION_ADMIN/VIEWER|Sales/Rules/Age Restrictions|
|CCM_SALES_RULES_BUSINESSRULES_ADMIN/VIEWER|Sales/Rules/Business Rules|
|CCM_SALES_TAX_TAXAUTHORITIES_ADMIN/VIEWER|Sales/Tax/Tax Authorities|
|CCM_SALES_TAX_TAXBRACKETS_ADMIN/VIEWER|Sales/Tax/Tax Brackets|
|CCM_SALES_TAX_TAXPARAMETERS_ADMIN/VIEWER|Sales/Tax/Tax Exemption Parameters|
|CCM_SALES_TAX_TAXRATES_ADMIN/VIEWER|Sales / Tax / Tax Rates|
|CCM_SALES_TAX_TAXZONES_ADMIN/VIEWER|Sales/Tax/Tax Zones
|CCM_SALES_TENDERING_CURRENCY_ADMIN/VIEWER|Sales/Tendering/Currency|
|CCM_SALES_TENDERING_CURRENCYEXCHANGERATE_ADMIN/VIEWER|Sales/Tendering/Currency Exchange Rate|
|CCM_SALES_TENDERING_TENDER_ADMIN/VIEWER|Sales / Tendering / Tender|
|CCM_SALES_TENDERING_TENDEREXCHANGE_ADMIN/VIEWER|Sales/Tendering/Tender Exchange|
|CCM_SALES_TENDERING_TENDERFEEPOLICY_ADMIN/VIEWER|Sales/Tendering/Tender Fee Policy|
|CCM_SALES_TENDERING_TENDERITEMRESTRICTIONS_ADMIN/VIEWER|Sales/Tendering/Tender Item Restrictions|
|CCM_SALES_TENDERING_SHOPPERIDVERIFICATION_ADMIN/VIEWER|Sales / Tendering / Shopper Id Verification|
|CCM_SALES_USWICTENDERING_WICEBTPOLICY_ADMIN/VIEWER|Sales/US WIC Tendering/WIC EBT Policy|
|CCM_SALES_USWICTENDERING_WICEBTAGENCIES_ADMIN/VIEWER|Sales/US WIC Tendering/WIC EBT Agencies|
|CCM_SALES_USWICTENDERING_WICCVBMAPPING_ADMIN/VIEWER|Sales/US WIC Tendering WIC CVB Product Mapping|
|CCM_SALES_USWICTENDERING_WICPRODUCTEXCLUSIONS_ ADMIN/VIEWER|Sales/US WIC Tendering/WIC Product Exclusions|
|CCM_ORGANIZATION_CHAINLOCATIONS_STORES_ADMIN/VIEWER|Organization/Chain Locations/Stores|
|CCM_ORGANIZATION_CHAINLOCATIONS_TOUCHPOINTS_ ADMIN/VIEWER|Organization/Chain Locations/Touchpoints|
|CCM_ORGANIZATION_TOUCHPOINTDEVICES_DEVICETYPES_ ADMIN/VIEWER|Organization/Touchpoint Devices/Device Types|
|CCM_ORGANIZATION_TOUCHPOINTDEVICES_DEVICES_     ADMIN/VIEWER|Organization/Touchpoint Devices/Devices|
|CCM_ORGANIZATION_TOUCHPOINTCATEGORIES_ TOUCHPOINTAPPLICATIONS_ADMIN/VIEWER|Organization/Touchpoint Categories/Touchpoint Applications|
|CCM_ORGANIZATION_TOUCHPOINTCATEGORIES_ TOUCHPOINTGROUPS_ADMIN/VIEWER|Organization/Touchpoint Categories/Touchpoint Groups|
|CCM_ORGANIZATION_CULTURE_MESSAGES_ADMIN/VIEWER|Organization/Culture/Messages|
|CCM_ORGANIZATION_GENERAL_REASONCODES_ADMIN/VIEWER|Organization/General/Reason Codes|
|CCM_ORGANIZATION_BUSINESSDAY_BUSINESSDAYSCHEDULER_ ADMIN/VIEWER|Organization/Business Day/Business Day Scheduler|

## Session Expiry

A user logged in to the CCM becomes logged out when the user token expires after a predetermined time (i.e., 15 minutes). Users can also be logged out due to inactivity after a predefined time. (i.e., no mouse moves/clicks, no keyboard key presses). The user can extend the session to avoid being logged out.

### Token Timeout

When a session token is due to expire, a message is prompted to inform the user that the session is due to expire. The message remains on the screen until the user responds to the message or until the token has expired (whichever occurs first).

![Token Timeout Screen](/Images/tokentimeoutscreen.png)

The user selects Continue to extend the session token and remain logged in. If the user selects Logout, the user is immediately logged out.  
On closing the message without selecting one of the options, the message is closed and once the token expires, the user is logged out.  
When the session token is extended, a timer is displayed. The timer counts the remaining time until a response is received from the security-tokens_exchange API. Once the token is successfully extended, the timer stops, and the user can continue working. If the token expires before a response is received, the user is logged out immediately.  
The message can be configured to prompt at a specific time duration prior to session expiry via the CCM_OFFICE_BFF_REFRESH_POPUP_TIME parameter. The default is 120 seconds (two minutes).  
**Note:**
The token session length time is not configurable, it is received from the Business Security Layer (BSL).

### Session Inactivity

When a user is inactive for a predefined time, (i.e., no mouse moves/clicks, no keyboard key presses), the system triggers an inactivity message that the user is about to be logged out, and the user is then logged out. If the user continues working (i.e., by performing one of the above actions), the message is removed and the user is not logged out.

![Session Inactivity Screen](/Images/sessioninactivityscreen.png)

The message remains on the screen until the user becomes active or the inactivity time has expired and the user is logged out (whichever occurs first). Once the user is active, the inactivity counter is reset.  
The default time duration of inactivity until the user is logged out is 600 seconds (ten minutes). The inactivity duration is configured via the CCM_OFFICE_BFF_INACTIVITY_TIMER parameter.  
The default time duration prior to inactivity logout when a message is prompted notifying the user that they are inactive is 120 seconds (two minutes). The time duration prior to logout that the message is displayed is configured via the CCM_OFFICE_BFF_INACTIVITY_POPUP_TIME parameter.


## How to use Emerald CCM

Open each of the domains from the Dashboard, for example, click the Organization domain.

![Dashboard Screen](/Images/DashboardCCMScreen.png)

Each domain opens with a menu in the left panel with all the module options.  
A ‘Search’ option is available from every screen to search for a specific menu or sub menu. See ‘Searching for a Menu’ further on.  
Open each module to explore the configuration options.  
For example, click Touchpoint Groups. The Touchpoint Groups screen opens.  
The breadcrumbs at the top of the screen display the navigation path.

![Touchpoint Groups Screen](/Images/TouchpointGroupsScreen.png)

From each module, the following options are available:
* Add new entities via the + Add <Module Name> hyperlink
* Click the pencil icon ![Pencil Icon](/Images/PencilIcon.png)
to open the screen in edit mode  

Click the ![NCR Logo](/Images/NCRLogo.png)
logo to return to the Dashboard.

## Search Function

The ‘Search’ function enables users to search for a specific menu or menu entry in the CCM.  
The ‘Search’ option is available from all CCM screens.  
The Search field is activated by entering at least 3   characters. The system retrieves all menus that match the text entered.  
The following screen shows the Search option.

![Search Option Screen](/Images/SearchOptionScreen.png)

For example, to search for the Touchpoint Branding menu:
1. In the Search field start entering the first 3 characters, e.g., enter ‘Tou’. The system displays all the menus that match the criteria entered.

![Search Field Form](/Images/SearchFieldForm.png)

2. Enter additional characters to narrow down the search, the matching menus are displayed:

![Search Touchpoint Branding Form](/Images/SearchTouchpointBrandingForm.png)

3. Select the menu. The breadcrumbs indicate the menu level.

![Touchpoint Branding Screen](/Images/TouchpointBrandingScreen.png)
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

Roles are created in Marketplace, which is the NCR portal that provides self-service location and user management for customers and third parties interacting with NCR APIs.

Once roles have been placed into the BSL environments during setup, they will be shown in the MARKETPLACE, and can be associated to the users. A role can be a 'hierarchy' role in which a list of roles are appended.

Once MARKETPLACE is populated with Roles (during onboarding), users can be assigned to roles to allow them to view all screens and have access to all CCM capabilities.

Roles can also be assigned to a user via the POST //security/role-grants/user-grants) API.

For functional details on Roles, see the Emerald 2.0 Functional Highlights.

The following roles should be added to any CCM user, in order for them to view all screens and provide all current capabilities:

* CCM_SALES_ADMIN
* CCM_ORGANIZATION_ADMIN
* CCM_UTILITIES_ADMIN
* CCM_OPERATIONS_ADMIN

Users who do not have permissions and try accessing the CCM Menus will get the following prompt:

![Access Denied Screen Screen](/Images/AccessDeniedScreen.png)

### Supported CCM Roles:

* NEP_ENTERPRISE_UNIT_UPDATE
* NEP_ENTERPRISE_ADMINISTRATOR
* EMERALD_POS_LOGIN 
* ITEMS_STORAGE_CONTAINER_VIEWER
* IMAGE_VIEWER
* CCM_CONFIGURATOR
* NEP_ENTERPRISE_UNIT_CREATE
* NEP_ENTERPRISE_TYPE_CREATE
* R1_CATALOG_VIEWER
* SELLING_RESOURCE_CONSUMER
* R1_TDM_UPLOAD
* SELLING_INTERNAL_ADMIN
* NEP_ENTERPRISE_GRANT_VIEWER
* SITE_READ
* NEP_ORGANIZATION_VIEWER
* NEP_ENTERPRISE_TYPE_UPDATE
* ITEMS_STORAGE_STORAGE_ADMINISTRATOR
* ITEMS_STORAGE_OBJECT_VIEWER
* NEP_ENTERPRISE_TYPE_DELETE
* TDM_READ
* NEP_ENTERPRISE_VIEWER
* R1_CATALOG_ADMINISTRATOR
* SELLING_CONFIG_VIEWER
* CATALOG_MESSAGING_SUBSCRIBER
* NEP_ENTERPRISE_SUPER_VIEWER
* SITE_ENTERPRISE_SETTING_READ
* IMAGE_WRITER
* ITEMS_STORAGE_CONTAINER_ADMINISTRATOR
* R1_TDM_VIEWER
* ITEMS_STORAGE_OBJECT_MODIFIER
* SELLING_CONFIG_ADMINISTRATOR
* NEP_ENTERPRISE_SUPER_ADMINISTRATOR
* NEP_ROLEGRANT_GRANT_TO_GROUPS
* R1_CATALOG_APPLICATION
* NEP_ROLEGRANT_REVOKE_FROM_USERS
* R1_TDM_ADMIN
* NEP_ROLEGRANT_GRANT_TO_ORGANIZATION
* NEP_ROLEGRANT_GRANT_TO_USERS
* NEP_ROLEGRANT_REVOKE_FROM_GROUPS
* NEP_ROLEGRANT_ADMINISTRATOR
* NEP_ROLE_VIEWER
* NEP_ROLEGRANT_REVOKE_FROM_ORGANIZATION

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
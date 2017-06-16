# Magento 2 Custom Redirect Pro

## Overview
[Magento 2 Custom Redirect Pro](http://www.magepsycho.com/magento-2-custom-redirect-pro.html) extension allows customer group wise redirection to the custom page after login, logout, registration & newsletter subscription actions with many extra features.

In case you have a multi-store website (B2B store, wholesale/retail store etc.) with multiple customer groups. And you want to provide a more personalized shopping experience to your customers, for example by
* Allowing your customers to select their required customer group at registration, either by using group drop-down or group code.
* Redirecting your retail customer to the retail website after they login from any one of your available multi-store websites.
* Redirecting your customer to welcome page with customized success message and email template if they register as a wholesale customer.
* Redirecting your customer to coupon page after newsletter subscription.
In any one of these cases (or all of them), you can use this extension.

![Magento 2 Custom Redirect Pro Backend Demo](http://g.recordit.co/eAqUvOqFl6.gif)

## Key Features
### 1. Customer Group Wise Redirection After Login
You can redirect your customer to any custom page(for example: `{{referer}}`, `/`, `/checkout/cart` etc.) configured as per the customer group after login. If group wise redirection URL is empty, default login redirection URL (`/customer/account`) will be used.


### 2. Customer Group Wise Redirection After Logout
You can redirect your customer to custom page configured as per the customer group after they logout.
Also, you can remove the logout intermediate page that says "You have logged out and will be redirected to our homepage in 5 seconds." and redirect user directly to the configured page with the custom message.


### 3. Customer Group Wise Redirection After Registration
You can configure customer group wise redirection page for registration (for example: /thank-you-page, /terms-and-conditions etc.). 
Also, this extension provides extra features like customer group wise success message as bonus.
This, of course, will add more personalized shopping experience to your customer.

### 4. Redirection After Newsletter Subscription
This extension allows to redirect the user to custom page (for example: /subscription-coupon, /subscription-thank-you etc.) after newsletter subscription.

### 5. Customer Group Selector / Switcher
[Magento 2 Customer Group Selector / Switcher](http://www.magepsycho.com/magento2-customer-group-selector-switcher-pro.html) extension is bundled at FREE with this extension, Bingo!.

> Customer Group Selector / Switcher extension allows user to select their required customer group at registration, either by using group drop-down or group code.

### 6. Essential Module for B2B E-Commerce
This extension by default includes the [Magento 2 Customer Group Selector / Switcher](http://www.magepsycho.com/magento2-customer-group-selector-switcher-pro.html). 
And if combined with [Magento 2 Store Restriction Pro](http://www.magepsycho.com/magento-2-store-restriction-pro.html), it will give you the solid base for creating the B2B store.

### 7. Misc Features
This extension supports both relative and absolute redirection URL, which in itself can contain custom variables.
* You can redirect to referrer URL (previous page) using `{{referer}}` variable.
* You can redirect to any URL mentioned in the query param (`?rediect_to=[custom-url]`) using `{{redirect_to}}` variable.
* Other available variables than can be used in redirection URL are:
    * `{{ip}}` - IP Address
    * `{{country_code}}` - Country Code
    * `{{user_name}}` - User Full Name
    * `{{user_email}}` - User Email Address
    * `{{user_id}}` - User Id
    * `{{user_group_id}}` - User Group Id
    
    
## Installation
1. Download the extension .zip file and extract the files.
1. Copy the extension files from src/ folder to the {magento2-root-dir}/
1. Run the following series of command from SSH console of your server:

`php bin/magento module:enable MagePsycho_RedirectPro MagePsycho_GroupSwitcherPro --clear-static-content`

`php bin/magento setup:upgrade`

5. Flush the store cache
`php bin/magento cache:flush`
6. Go to Admin > Stores > Configuration > MagePsycho > Custom Redirect Pro > Configure your settings here...

## Live Demo:
* [View Frontend Demo](http://m2-custom-redirect-pro.mage-expo.com/customer/account/create/)  
* [View Backend Demo](http://m2-custom-redirect-pro.mage-expo.com/admin_m2demo)

## Changelog
**Version 1.0.0 (2017-05-29)**
    
* Initial Release.    

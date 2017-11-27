---
layout: post
title: "Using Wampum WooCommerce Plugin"
date: 2017-11-27 00:54:46
author: Russell
categories:
- blog
- WooCommerce
- plugin
- ecommerce
img: woocommerce.png
thumb: woo_thumb.png
canonical_url: 'http://cryptowampum.com/blog/wampum/using_wampum_woocommerce_plugin.html'
---

[WooCommerce](https://woocommerce.com/) is probably the easiest way to set up a storefront using [Wordpress](https://wordpress.com/).  It makes managing your business's store and payments simple.  Because so many of our customers choose to use WooCommerce it was the first third-party plugin that we provided.  It is called "woo-gateway-wampum-bitcoin."  

The plugin allows a store owner to leverage her Wampum Register© instance to accept Bitcoin payments as they would at the point of sale.  You can also leverage plugins like [woocommerce-payment-discounts](https://github.com/claudiosanches/woocommerce-payment-discounts) to offer discounts for Bitcoin payments without a discount code.

## Description ##

This plugin adds a Bitcoin payment method to your store.  It requires that you have access to a Wampum Register© instance or white-labeled service that supports Wampum's API.  The plugin automatically converts the price from the currency you use to Bitcoin, but only supports ONE CURRENCY.  The one that your Wampum Register© instance is configured to use.  Using Euros or Yen or anything is ok, but the setting will apply to all payments through your store.

The beautiful thing about this plugin is that it integrates so nicely into your existing workflow.  When the payment page is displayed, the system will send an email to the customer to make sure they can pay later if they don't currently have enough bitcoin available in his/her wallet.  You can also provide a link to the customer to purchase bitcoin from your favorite exchange or Bitcoin ATM.

A "cron" job checks the blockchain at 20-minute increments to see the status of the payment and sends the receipt to the customer and order notice to the store owner, assuming this is your standard workflow.

You can add the Bitcoin payment method to your store
Settings configured in the WooCommerce Checkout Tab:
Title: Title of the payment method, typically "Bitcoin."
Customer Message: What you want your store to say as a thank you, e.g., "Thank you for purchasing with Bitcoin with Wampum Register©."
Wampum URL: URL of your Wampum Register© instance
Wampum Username: User name of the remote API user
Wampum Password: Password of the remote API user

Note that this plugin has only been tested with WooCommerce 4.0 and later.


## Screenshots ##
	
### 1. Settings page. ###
You can configure the plugin via the WooCommerce settings pane.

![Settings page.](/assets/files/gateway-wampum-bitcoin/PluginSettings.png) 

### 2. Plugin in action on payment page. ###
You can see here that the Bitcoin payment method is here.  You can name it in the settings pane.

![Plugin in action.](/assets/files/gateway-wampum-bitcoin/PaymentMethodsPage.png)


### 3. Plugin in action on payment method checkout page. ###
Note that the payer can use the QR code or copy the payment request to the clipboard.

![Payment Page](/assets/files/gateway-wampum-bitcoin/PaymentPage.png)


[russell]: http://cryptowampum.com

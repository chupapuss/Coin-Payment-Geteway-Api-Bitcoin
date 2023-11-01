
# **CoinDrive for Omnipay**

<p align="center">
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway/advanced/">
        <img src="https://ps.w.org/woo-altcoin-payment-gateway/assets/icon-128x128.png" alt="codesolz.net"/>
    </a>
</p>

<p align="center">
    <img alt="undefined" src="https://img.shields.io/github/last-commit/tuhin18003/WooCommerce-AltCoin-Payment-Gateway.svg">
    <a href="https://codeclimate.com/github/tuhin18003/WooCommerce-AltCoin-Payment-Gateway">
        <img alt="undefined" src="https://api.codeclimate.com/v1/badges/53342611d39bf5044b5f/maintainability">
    </a>
    <img alt="undefined" src="https://img.shields.io/github/languages/code-size/tuhin18003/WooCommerce-AltCoin-Payment-Gateway.svg"> <br>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="undefined" src="https://img.shields.io/wordpress/plugin/wp-version/woo-altcoin-payment-gateway.svg">
    </a>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="undefined" src="https://img.shields.io/wordpress/plugin/tested/woo-altcoin-payment-gateway.svg">
    </a>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="undefined" src="https://img.shields.io/wordpress/plugin/v/woo-altcoin-payment-gateway.svg">
    </a>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="undefined" src="https://img.shields.io/wordpress/plugin/rating/woo-altcoin-payment-gateway.svg">
    </a>
    <br>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="undefined" src="https://img.shields.io/wordpress/plugin/dm/woo-altcoin-payment-gateway.svg">
    </a>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="undefined" src="https://img.shields.io/wordpress/plugin/dt/woo-altcoin-payment-gateway.svg">
    </a>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img alt="Wordpress Plugin Active Installs" src="https://img.shields.io/wordpress/plugin/installs/woo-altcoin-payment-gateway.svg">
    </a>
    <a href="https://wordpress.org/plugins/woo-altcoin-payment-gateway">
        <img src="https://hitcounter.pythonanywhere.com/count/tag.svg?url=https%3A%2F%2Fgithub.com%2FCodeSolz%2FWooCommerce-AltCoin-Payment-Gateway%2Fblob%2Fmaster%2FREADME.md" alt="Hits">
    </a>
    <br><br>
    <a href="https://codesolz.net">
        <img alt="undefined" src="https://img.shields.io/badge/Created%20By-M.Tuhin-brightgreen.svg">
    </a>
</p>
<h2 align="center">WooCommerce AltCoin Payment Gateway - Wordpress plugin</h2>



**Setting Up Your Platform**

1. Enroll for an account on the [Coinbase Commerce](https://commerce.coinbase.com/) platform.
2. Generate an API Key by navigating to the Settings section within the Coinbase Commerce dashboard.
3. Transfer the `coinbase/` directory to the designated `modules/` folder located in your Prestashop environment.
4. Access your Prestashop Back Office, locate the Modules tab, proceed to the "Installed Modules" segment, and initiate a search for "Coinbase Commerce". Once identified, engage the Install option to activate the plugin.
5. Select Configure to enter the plugin's settings page. Here, input the API Key and Shared Secret Key derived from the Coinbase Commerce Dashboard.
6. Extract the webhook URL from the settings page of the plugin and input it into the relevant section within the Coinbase Commerce Dashboard Settings.

**Please Take Note:** An option referred to as the "Unsafe" mode is accessible on the plugins settings page. It is imperative that this option remains disabled on any live website. Its sole purpose is to facilitate testing during developmental stages, as it suspends the validation of requests forwarded to the webhook. This enables developers to simulate POST requests to the webhook without the generation of the `X-CC-Webhook-Signature` header.


### Plugin Localization

Every textual elements, designations, and explanations embedded within the plugin are as follows:

### Overview

Coinbase Commerce serves as a digital payment platform, empowering merchants to embrace transactions conducted through an array of digital currencies including but not limited to Bitcoin, Bitcoin Cash, DAI, Ethereum, Litecoin, and USD Coin. These transactions seamlessly flow into the merchant's controlled wallet.

Characteristics:

* Rapid — Ready for deployment within minutes, not prolonged periods
* Complimentary — Zero charges for processing cryptocurrency payments
* Global Reach — Access an expansive international customer pool
* No Intermediaries — Assume the role of your financial institution
* Irreversible Nature — Bid farewell to the concept of chargebacks


**Prerequisites**
-------
* Plugin: Gravity Forms 2.0 or a more recent version. Obtainable at [Gravity Forms](https://www.gravityforms.com/).

### Establishing the Setup

In this section, we delineate the process of installing and configuring the Gravity Forms Coinbase Commerce Add-On. Ensure that you meticulously adhere to *all* the provided guidelines for the Add-On to function seamlessly.

### Prerequisites

Necessitates a minimum of WordPress 4.0, PHP 5.3, and [Gravity Forms](https://rocketgenius.pxf.io/c/1212782/445235/7938) 1.9.

### Operational Steps

1. Confirm the possession of your individual copy of [Gravity Forms](https://www.gravityforms.com/). Please note that this plugin does not incorporate Gravity Forms within it.

2. A Coinbase Commerce account is also mandatory. To initiate the registration process, access https://commerce.coinbase.com/

3. Download the zip archive from the [releases page](https://github.com/coinbase/coinbase-commerce-gravity-forms/releases) and then proceed to unzip it. Alternatively, clone the plugin and execute the `composer install` command within the cloned directory.

4. Integrate the plugin folder named "gf-coinbase-commerce" into the designated /wp-content/plugins directory of your WordPress site.

5. Navigate to the **Plugins** menu within your WordPress dashboard, identify `Coinbase Commerce Payments For Gravity Forms` within the list of plugins, and activate it by clicking the designated link.

6. Access the **Forms->Settings** menu, opt for the Coinbase Commerce Tab, and insert your API Key and Shared Secret Key obtained from the Coinbase Commerce Dashboard (https://commerce.coinbase.com/dashboard/settings).

7. Transfer the Webhook Notification URL from the Coinbase Commerce Tab to the Settings/Webhook subscription found at https://commerce.coinbase.com/dashboard/settings.

8. Forge a new Gravity form and incorporate the Coinbase Commerce Feed.

### Addressing Common Queries

**Is SSL a Prerequisite?**  
Indeed, SSL is indispensable for the receipt of webhook notifications.

**Does Coinbase Commerce seamlessly integrate with alternative e-commerce platforms?**  
Certainly, a comprehensive list of official integrations is accessible here: [Coinbase Commerce Integrations](https://commerce.coinbase.com/integrate).

### Version Evolution

**1.2.0**

* Inaugural release edition


# Checkout Web SDK server example

Test login: https://ca-test.adyen.com/ca/ca/login.shtml

## To find out
- What are the options for different countries?
- How to implement recurring payments?

## References
* Web SDK instructions: https://docs.adyen.com/developers/checkout/web-sdk/quick-start-web/show-payment-form-web
* Test cards: https://docs.adyen.com/developers/test-cards/test-card-numbers
* Recurring payments: https://docs.adyen.com/developers/features/recurring-payments

## Languages
* add a query e.g. `?shopperLocale=zh-TW`
* See https://docs.adyen.com/developers/checkout/web-sdk/customization/translations

## Country Code
* add a query e.g. `&countryCode=NL`
* A valid value is an ISO 2-character country code (e.g. 'NL').

## ! This repository is for demo purposes only !
This PHP server example is intended to help developers to get quickly up and running with our Checkout JavaScript SDK.<br/>
Always ask a backend developer to create an implementation of our checkout product.

## Requirements
To run this web checkout example, <b>add</b>  the following file <b>config/authentication.ini</b> and create variables:<br/>

<b>merchantAccount</b>= "YOUR MERCHANT ACCOUNT".<br/>
<b>checkoutAPIkey</b>= "YOUR CHECKOUT API KEY".<br/>

These variables can be found in Adyen Customer Area. For more information, visit our <a href="https://docs.adyen.com/developers/get-started-with-adyen/create-a-test-account">Getting Started guide</a>.<br/>

## Installation

### Deploying this example to Heroku

You can install this example in two ways:

Use this shortcut to deploy to Heroku:<br/>
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/Adyen/adyen-web-sdk-sample-code)

Alternatively, clone this repository and deploy it to your own PHP server.

## Documentation

For the complete integration guide, refer to the Adyen documentation:
<a href="Checkout Web SDK">https://docs.adyen.com/developers/checkout/web-sdk</a>

## License

This repository is open source and available under the MIT license. For more information, see the LICENSE file.

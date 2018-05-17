# Checkout Web SDK server example

Test login: https://ca-test.adyen.com/ca/ca/login.shtml

IPs added:
- RC Local: 151.231.24.62
- RC Local: 176.127.233.196

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
* https://docs.adyen.com/developers/currency-codes

## Currency
* add a query e.g. `&currency=EUR`
* Three character value
* Some payment methods are limited to the currency, e.g. countryCode = NL, currencyCode= CNY << no IDEAL should be shown as it requires EUR.

## Additional data
See: https://docs.adyen.com/api-explorer/#/PaymentSetupAndVerificationService/v32/payments there’s a field called additionalData.

"The additionalData object is a generic container that can hold extra request fields. You may require to pass these fields along with payment request data, for example, to better manage risky transactions or to initiate a payment using some local payment methods.

This functionality is not enabled by default, as it requires additional configuration on Adyen's end. Contact the  Support Team to request enabling it for you."

https://docs.adyen.com/developers/api-reference/payments-api#paymentrequestadditionaldata

Pass it along with the other stuff as a (JSON) POST request to the /setup endpoint when initiate the payment session.

## ! This repository is for demo purposes only !
This PHP server example is intended to help developers to get quickly up and running with our Checkout JavaScript SDK.<br/>
Always ask a backend developer to create an implementation of our checkout product.

## Requirements
To run this web checkout example, <b>add</b>  the following file <b>config/authentication.ini</b> and create variables:<br/>

<b>merchantAccount</b>= "YOUR MERCHANT ACCOUNT".<br/>
<b>checkoutAPIkey</b>= "YOUR CHECKOUT API KEY".<br/>

These variables can be found in Adyen Customer Area. For more information, visit our <a href="https://docs.adyen.com/developers/get-started-with-adyen/create-a-test-account">Getting Started guide</a>.<br/>

## Documentation

For the complete integration guide, refer to the Adyen documentation:
<a href="Checkout Web SDK">https://docs.adyen.com/developers/checkout/web-sdk</a>

## License

This repository is open source and available under the MIT license. For more information, see the LICENSE file.

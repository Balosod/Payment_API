# 100088-Payment-API Documentation

Payment API is a versatile payment integration solution that offers two endpoints: Stripe and PayPal. With this API, we can easily integrate and streamline payment processes using these trusted payment gateways.

The Stripe endpoint allows us to securely process online payments using credit and debit cards.With this endpoint, we can provide our customers with a smooth and reliable payment experience.

#### The PayPal endpoint provides us with a convenient way to accept payments from customers who prefer using PayPal

#### In conclusion, This Payment API is a robust integration solution that offers us the ability to process payments seamlessly through Stripe and PayPal. With its security, flexibility, and comprehensive features, this API empowers us to provide our customers with a reliable and convenient payment experience across different payment methods.For more comprehensive understanding of the API and what it entails like the request body, methods and response, click the link below to know more.

[Documentation Link](https://documenter.getpostman.com/view/20868747/2s93mAVLjQ)

# PAYMENT OPTIONS
### 1. Stripe
### Request METHOD : POST
#### End-Point: https://100088.pythonanywhere.com/api/stripe
#### Where the body of the POST request contain the price which will be deducted from the customer account.

#### Example of the body to be sent in the API : POST
#### Note that Default price currency is USD
```

{
  "price": 34,
  "product": "Workflow AI"
}
```
#### A response with status code 200 will be return which contains a approval_url for the user to complete the payment process, this response  will be loaded from the client side. 

#### Response to API
```
{"approval_url": "https://checkout.stripe.com/c/pay/cs_live_a1PcUOufapjR2dwu4W75mYiZUcCMnFc7RcXRmKJNrUqvJGWImQIuzVJLOv#fidkdWxOYHwnPyd1blppbHNgWjA0SWtiNT1Jck91bE9PZF9GVURXbkdmaGhTX2JHcUFmZE1XQUtTMEh1VlE0MWY3al9Td3JNa2xsYGxrRFdhbD1CakRrX3RJXTRqcUdPUTF0N1FtbDRcTjxpNTU1VUhiRkRJdCcpJ2N3amhWYHdzYHcnP3F3cGApJ2lkfGpwcVF8dWAnPyd2bGtiaWBabHFgaCcpJ2BrZGdpYFVpZGZgbWppYWB3dic%2F2FcXdwYHgl"}

```


### 2. Paypal
### Request METHOD : POST
#### End-Point: https://100088.pythonanywhere.com/api/paypal
#### Where the body of the POST request contain the price which will be deducted from the customer account.

#### Example of the body to be sent in the API : POST
#### Note that Default price currency is USD

```
{
  "price": 34,
  "product": "WifiQRCode"
}
```
#### A response with status code 200 will be return which contains a approval_url for the user to complete the payment process, this response  will be loaded from the client side. 

#### Response to API
````
{"approval_url": "https://www.sandbox.paypal.com/checkoutnow?token=3D273334GG998674X"}

````

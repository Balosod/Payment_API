# Payment_API Documentation
### (1) Stripe
#### Use the link given below to create a post request
```` http://127.0.0.1:8000/stripe ````
#### Where the body of the POST request contain the price which will be deducted from the customer account.
```` {"price":40}````
#### A response with status code 200 will be return which contains a checkout link for the user to complete the payment process, this response  will be loaded from the client side. 
```` {"checkout url": "https://checkout.stripe.com/c/pay/cs_live_a1PcUOufapjR2dwu4W75mYiZUcCMnFc7RcXRmKJNrUqvJGWImQIuzVJLOv#fidkdWxOYHwnPyd1blppbHNgWjA0SWtiNT1Jck91bE9PZF9GVURXbkdmaGhTX2JHcUFmZE1XQUtTMEh1VlE0MWY3al9Td3JNa2xsYGxrRFdhbD1CakRrX3RJXTRqcUdPUTF0N1FtbDRcTjxpNTU1VUhiRkRJdCcpJ2N3amhWYHdzYHcnP3F3cGApJ2lkfGpwcVF8dWAnPyd2bGtiaWBabHFgaCcpJ2BrZGdpYFVpZGZgbWppYWB3dic%2F2FcXdwYHgl"}  ````


### (1) Paypal
#### Use the link given below to create a post request
```` http://127.0.0.1:8000/paypal ````
#### Where the body of the POST request contain the price which will be deducted from the customer account.
```` {"price":50}````
#### A response with status code 200 will be return which contains a checkout link for the user to complete the payment process, this response  will be loaded from the client side. 
```` {"checkout url": "https://www.sandbox.paypal.com/checkoutnow?token=3D273334GG998674X"}  ````

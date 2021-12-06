---
sidebar_position: 14
id: Other-Payment-Methods
title: Other-Payment-Methods
---



# Other Payment Methods

For Developers or Business that want to use other payment methods other than card, they can use
the following methods and pass in the neccesary parameters.


## Transfer

```jsx
// import com.interswitchng.smartpos.models.cardless.CardLessPaymentRequest
// import com.interswitchng.smartpos.models.transaction.cardpaycode.request.PurchaseType
// import com.interswitchng.smartpos.models.transaction.ussdqr.response.Bank
// import com.interswitchng.smartpos.models.transaction.ussdqr.response.CodeResponse
// import com.interswitchng.smartpos.models.transaction.ussdqr.response.PaymentStatus
// import com.interswitchng.smartpos.shared.models.transaction.CardLessPaymentInfo


//you need to get the virtual account details the customer need to send it to. 
IswHandler().loadVirtualAccountDetails(request: CardLessPaymentRequest)

// use checkpayment to check if the user had made the payment using any of the payment methods.

// the method's parameters are gotten from the response of the previous methods in the transaction Journey

IswHandler().checkPaymentStatus(transactionReference: String,
                             merchantCode: String, paymentType: PaymentType)


```

## Paycode

```jsx
// import com.interswitchng.smartpos.models.cardless.CardLessPaymentRequest
// import com.interswitchng.smartpos.models.transaction.cardpaycode.request.PurchaseType
// import com.interswitchng.smartpos.models.transaction.ussdqr.response.Bank
// import com.interswitchng.smartpos.models.transaction.ussdqr.response.CodeResponse
// import com.interswitchng.smartpos.models.transaction.ussdqr.response.PaymentStatus
// import com.interswitchng.smartpos.shared.models.transaction.CardLessPaymentInfo



// use this method to perform paycode payment type
IswHandler().initiatePaycodeTransaction(terminalInfo: TerminalInfo,
                                           paymentInfo: CardLessPaymentInfo, code: String)

```

## USSD

```jsx
// import com.interswitchng.smartpos.models.cardless.CardLessPaymentRequest
// import com.interswitchng.smartpos.models.transaction.cardpaycode.request.PurchaseType
// import com.interswitchng.smartpos.models.transaction.ussdqr.response.Bank
// import com.interswitchng.smartpos.models.transaction.ussdqr.response.CodeResponse
// import com.interswitchng.smartpos.models.transaction.ussdqr.response.PaymentStatus
// import com.interswitchng.smartpos.shared.models.transaction.CardLessPaymentInfo


// First you need to list allowed banks and choose the bank you want. 
// to list banks, use this method..
IswHandler().loadbanks()


// After selecting the bank you want to Use, Use this method to initaiate USSD transaction. 

 var paymentInfo = CardLessPaymentInfo(amount = 100, "", surcharge = 0, additionalAmounts = 0)
var request = CardLessPaymentRequest.from(
    terminalInfo!!,
    paymentInfo,
   CardLessPaymentRequest.TRANSACTION_USSD,
   bankCode = bankList.get(0).code // this is gotten from the bank list
  )

IswHandler().initiateUssdTransactions(request: CardLessPaymentRequest)

// use checkpayment to check if the user had made the payment using any of the payment methods.

// the method's parameters are gotten from the response of the previous methods in the transaction Journey

IswHandler().checkPaymentStatus(transactionReference: String,
                             merchantCode: String, paymentType: PaymentType)


```

## QR CODE

```jsx
// import com.interswitchng.smartpos.models.cardless.CardLessPaymentRequest
// import com.interswitchng.smartpos.models.transaction.cardpaycode.request.PurchaseType
// import com.interswitchng.smartpos.models.transaction.ussdqr.response.Bank
// import com.interswitchng.smartpos.models.transaction.ussdqr.response.CodeResponse
// import com.interswitchng.smartpos.models.transaction.ussdqr.response.PaymentStatus
// import com.interswitchng.smartpos.shared.models.transaction.CardLessPaymentInfo


// Use this method to initaiate QR transaction. 
IswHandler().initiateQrTransactions(request: CardLessPaymentRequest)

// use checkpayment to check if the user had made the payment using any of the payment methods.

// the method's parameters are gotten from the response of the previous methods in the transaction Journey

IswHandler().checkPaymentStatus(transactionReference: String,
                             merchantCode: String, paymentType: PaymentType)


```


## Parameters

- **CardLessPaymentRequest** [CardLessPaymentRequest](/docs/Classes/CardLessPaymentRequest)
- **paymentInfo:** [CardLessPaymentInfo](/docs/Classes/CardLessPaymentInfo)
- **terminalInfo:** [TerminalInfo](/docs/Classes/terminalInfo).
##


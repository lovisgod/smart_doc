---
sidebar_position: 1
id: bill-payment
title: Bill payment
---



# Create a Document

You can make bill payments by details using this service.


## Perform name enquiry

```jsx
// Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler


// use to process bill payment
IswHandler().processBillPaymentTransaction(
                paymentModel: PaymentModel,
                accountType: AccountType,
                terminalInfo: TerminalInfo,
                isAirTime: Boolean
            )

```

## Parameters

- **paymentModel:** [PaymentModel](/docs/Classes/paymentModel)
- **accountType:** [AccountType](/docs/classes/account-type)
- **terminalInfo:** [TerminalInfo](/docs/Classes/terminalInfo).
- **isAirtime:** [Boolean](#) This is ***true*** when the bill payment time is for airtime purchase

##


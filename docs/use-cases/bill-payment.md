---
sidebar_position: 1
id: bill-payment
title: Bill payment
---



# Create a Document

You can make bill payments by details using this service.


## Perform name enquiry

```
# Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler


# use to process bill payment
IswHandler().processBillPaymentTransaction(
                paymentModel: PaymentModel,
                accountType: AccountType,
                terminalInfo: TerminalInfo,
                isAirTime: Boolean
            )

```

## Parameters

- **paymentModel:** [Payment Model](/docs/model-classes-definations/greeting)
- **accountType:** [Account type](/docs/model-classes-definations/greeting)
- **terminalInfo:** Terminal Info. This can be gotten as shown [Here](/docs/model-classes-definations/bank-model)
- **isAirtime:** This is ***true*** when the bill payment time is for airtime purchase

##


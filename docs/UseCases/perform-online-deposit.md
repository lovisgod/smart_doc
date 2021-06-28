---
sidebar_position: 9
id: online-deposit
title: Online Deposit
---



# Online Deposit

You can perform online deposit transaction using this service.


## Perform Online Deposit

```jsx
// Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler


// use to process online deposit
IswHandler().processDepositTransaction(
                paymentModel: PaymentModel,
                accountType: AccountType,
                terminalInfo: TerminalInfo
            )

```

## Parameters

- **paymentModel:** [PaymentModel](/docs/Classes/paymentModel)
- **accountType:** [AccountType](/docs/classes/account-type)
- **terminalInfo:** [TerminalInfo](/docs/Classes/terminalInfo).
##


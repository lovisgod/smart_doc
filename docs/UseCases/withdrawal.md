---
sidebar_position: 11
id: Withdrawal
title: Withdrawal
---



# Withdrawal

You can perform withdrawal transaction using this service.


## Perform WithDrawal

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


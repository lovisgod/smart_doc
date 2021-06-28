---
sidebar_position: 12
id: completion
title: Completion
---



# Completion

You can perform completion transaction using this service.


## Perform Completion

```jsx
// Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler


// use to process completion
IswHandler().processDepositTransaction(
                paymentModel: PaymentModel,
                accountType: AccountType,
                terminalInfo: TerminalInfo,
                originalTxnData: OriginalTransactionInfoData
            )

```

## Parameters

- **paymentModel:** [PaymentModel](/docs/Classes/paymentModel)
- **accountType:** [AccountType](/docs/classes/account-type)
- **terminalInfo:** [TerminalInfo](/docs/Classes/terminalInfo).
- **originalTxnData:** [OriginalTransactionInfoData](/docs/Classes/terminalInfo).
##


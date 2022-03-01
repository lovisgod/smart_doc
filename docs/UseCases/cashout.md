---
sidebar_position: 13
id: cashout
title: Cashout
---



# Cashout

You can perform cashout transaction using this service.


## Perform Cashout

```jsx
// Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler


// use to process cashout
IswHandler().processCashoutTransferTransaction(
                paymentModel: PaymentModel,
                accountType: AccountType,
                terminalInfo: TerminalInfo,
                destinationAccountNumber: String? = "",
                receivingInstitutionId: String? = "",
                
            )

```

## Parameters

- **paymentModel:** [PaymentModel](/docs/Classes/paymentModel)
- **accountType:** [AccountType](/docs/classes/account-type)
- **terminalInfo:** [TerminalInfo](/docs/Classes/terminalInfo)
- **destinationAccountNumber:** [String](#) (The 10 digit NUBAN account number)
- **receivingInstitutionId:** [String](#) (The receiving id of the financial institution).
##


---
sidebar_position: 8
id: balance-inquiry
title: Balance Inquiry
---



# Balance Inquiry?

You can prform balance inquiry transaction using this service.


## Perform Balance Inquiry

```jsx
// Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler


// use to process bill payment
IswHandler().processBalanceInquiry(
                accountType: AccountType,
                terminalInfo: TerminalInfo,
                cardType: CardType
            )

```

## Parameters

- **cardTpe:** [CardType](/docs/Classes/cardType)
- **accountType:** [AccountType](/docs/classes/account-type)
- **terminalInfo:** [TerminalInfo](/docs/Classes/terminalInfo).
##


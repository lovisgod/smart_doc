---
sidebar_position: 7
id: pin-selection
title: Pin Selection
---



# Pin Selection?

You can perform pin selection transaction using this service.


## Perform Pin Selection

```jsx
// Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler


// use to process pin selection
IswHandler().processPinSelect(
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


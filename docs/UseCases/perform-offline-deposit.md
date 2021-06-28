---
sidebar_position: 10
id: offline-deposit
title: Offline Deposit
---



# Offline Deposit

You can perform offline deposit transaction using this service.
Before your perfome offline deposit, you have to get the offine deposit limit for that particular terminal and merchant.


Use this method to get offline deposit transaction limit 

## Get offline deposit limit

```jsx
// Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler
// use to process offline deposit
IswHandler().getOfflineSettings(
                terminalInfo: TerminalInfo
            )
```

## Parameters

- **terminalInfo:** [TerminalInfo](/docs/Classes/terminalInfo).
##




## Process Offline Deposit

```jsx
// Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler


// use to process offline deposit
IswHandler().makeOfflinePayment(
                amount: String,
                accountNumber: String,
                terminalInfo: TerminalInfo
            )

```

## Parameters

- **amount:** String
- **accountNumber:** String
- **terminalInfo:** [TerminalInfo](/docs/Classes/terminalInfo).
##


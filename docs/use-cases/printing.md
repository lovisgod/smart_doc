---
sidebar_position: 6
id: printing
title: Priniting
---


# Printing

You cancontrol printer functions.

## Print

```
# Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler

# use to process bill payment
IswHandler().printslip(bitmap: Bitmap)
```

## Parameters

- **bitmap:** A bitmap of the receipt

As a result, a **[TerminalInfo](/docs/model-classes-definations/greeting)** is returned if successful.

## Check printer status

```
# Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler

# use to process bill payment
IswHandler().checkPrintStatus() 
```

## Parameters

- **terminalInfo:** [TerminalInfo](/docs/model-classes-definations/greeting)

As a result, a **[TerminalInfo](/docs/model-classes-definations/greeting)** is returned if successful.




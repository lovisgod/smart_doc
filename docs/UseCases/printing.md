---
sidebar_position: 6
id: printing
title: Priniting
---


# Printing

You cancontrol printer functions.

## Print

```jsx
// Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler

// use to process print a slip
IswHandler().printslip(bitmap: Bitmap)
```

## Parameters

- **bitmap:**Bitmap (A bitmap of the receipt)

## Check printer status

```jsx
// Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler

// use to check printer status
IswHandler().checkPrintStatus() 
```

## Parameters

As a result, a **[PrintStatus](/docs/Classes/printStatus)** is returned.




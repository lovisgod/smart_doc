---
sidebar_position: 4
id: terminal-info
title: Terminal Info
---


# Terminal Info

You can make retreive and make changes to terminal info.

## Retreive Terminal Info

```jsx
// Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler

// use to process bill payment
IswHandler().getTerminalInfo(): 
```

As a result, a **[TerminalInfo](/docs/Classes/terminalInfo)** is returned if successful.

## Save Terminal Info

```jsx
// Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler

// use to process bill payment
IswHandler().saveTerminalInfo(terminalInfo): 
```

## Parameters

- **terminalInfo:** [TerminalInfo](/docs/Classes/terminalInfo)

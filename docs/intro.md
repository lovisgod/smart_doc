---
sidebar_position: 1
---

# Introduction

Let's discover **Smart POS in less than 5 minutes**.

## Getting Started

SmartPOS SDK is a simple to use SDK for the purpose of building Android App on POS terminals
The SDK is divided into three(3) modules namely -

`smart-pos-core`
`smart-pos-emv-pax`
`smart-pos-usb`

this three modules should be downloaded and added to your project.
In addition to these modules, you need to use eze simple library to so that the app will work  better.


### To start using the SDK, follow the steps below:

add module smart-pos-core and module smart-pos-emv-pax to your project. If you want to make use of USB communication between the SDK and a PC, add the third module smart-pos-usb
Configure the SDK in your android Application class or your main Activity or Fragment or Application class like below


```// create POSDevice Implementation instance for pax device
POSDeviceImpl device  = POSDeviceImpl.create(getApplicationContext());

String clientId = "your-client-id";
String clientSecret = "your-client-secret";
String alias = "your-alias";
String merchantCode = "your-merchant-code";

// initialize POSConfig 
POSConfig config = new POSConfig(alias, clientId, clientSecret, merchantCode);

// setup terminal
IswPos.setupTerminal(getApplication(), device, config);
```

Configure Terminal
In order to communicate effectively with the terminal, some initialization and configuration needs to be done, 



Note on USB communication
For USB communication between the SDK and a PC to work, the below steps need to be followed

ADB must be installed and added to Path enviroment variable on the PC
USB Debugging must be enabled in the Android terminal

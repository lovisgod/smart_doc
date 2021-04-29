---
sidebar_position: 2
id: name-enquiry
title: Name Enquiry
---



# Create a Document

You can validate bank details using this service.


## Perform name enquiry

```jsx
// Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler


// use
IswHandler().validateBankDetails(bankCode = "044", accountNumber="0095555555")

```

## Parameters

- **bankCode:** [String](#) (The CBN bank code of the financial institution)
- **accountNumber:** [String](#) (The 10 digit NUBAN account number)

##

As a result, a **[Success`<BeneficiaryModel>`](/docs/Classes/beneficiaryModel)** is returned if successful and **[Failure](#)** if unsuccessful

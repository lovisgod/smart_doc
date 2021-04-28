---
sidebar_position: 2
id: name-enquiry
title: Name Enquiry
---



# Create a Document

You can validate bank details using this service.


## Perform name enquiry

```
# Import the ISWHandler from com.interswitchng.smartpos.IswTxnHandler


# use
IswHandler().validateBankDetails(bankCode = "044", accountNumber="0095555555")

```

## Parameters

- **bankCode:** The CBN bank code of the financial institution
- **accountNumber:** The 10 digit NUBAN account number

##

As a result, a **[Success`<BeneficiaryModel>`](/docs/model-classes-definations/greeting)** is returned if successful and **[Failure](/docs/model-classes-definations/greeting)** if unsuccessful

# Technical Assessment
NOTE: The majority of the work for this position will be using JS with ES6 syntax.

## Overview
Please complete this exercise with in Vuejs. This exercise is intended to take no longer than 2 hours.  Please limit the detail of your solution with that time in mind.  Please include a README with your submission detailing your solution.

## Problem
Lets assume Cascade Fintech has contracted you to build a **VueComponent** to support a new transaction feed.  

## Data definition

Assume the following data has been taken from the api and has been converted in VuexStore
```json
{
	"Statement": {
		"Transactions": [{
			"OriginalTraceAuditNo": null,
			"AccountNumber": "123456789",
			"TransactionTypeId": "Debit",
			"TransactionDate": "2020-08-28T03:36:33",
			"BusinessDate": "2020-08-28T03:36:33",
			"AvailableBalance": 400.00,
			"Amount": 12.08,
			"Description": "Other: POS Transaction",
			"Billed": false,
			"MerchantName": "Good Buy",
			"MerchantId": "GbLV-01"
		},
    {
			"OriginalTraceAuditNo": null,
			"AccountNumber": "123456789",
			"TransactionTypeId": "Debit",
			"TransactionDate": "2020-08-28T03:50:01",
			"BusinessDate": "2020-08-28T03:50:01",
			"AvailableBalance": 400.00,
			"Amount": 129.74,
			"Description": "Other: POS Transaction",
			"Billed": false,
			"MerchantName": "Wally World",
			"MerchantId": "WWV-000-1220"
		},
    {
			"OriginalTraceAuditNo": null,
			"AccountNumber": "123456789",
			"TransactionTypeId": "Debit",
			"TransactionDate": "2020-08-28T06:43:12",
			"BusinessDate": "2020-08-28T06:43:12",
			"AvailableBalance": 400.00,
			"Amount": 8.08,
			"Description": "Other: POS Transaction",
			"Billed": true,
			"MerchantName": "Quickly Gas Stop",
			"MerchantId": "QGS-01"
		}],
		"NotSettled": [{
			"OriginalTraceAuditNo": null,
			"AccountNumber": "123456789",
			"TransactionTypeId": "Debit",
			"TransactionDate": "2020-08-28T03:36:33",
			"BusinessDate": "2020-08-28T03:36:33",
			"AvailableBalance": 400.00,
			"Amount": 12.08,
			"Description": "Other: POS Transaction",
			"MerchantName": "Good Buy",
			"MerchantId": "GbLV-01"
		},
    {
			"OriginalTraceAuditNo": null,
			"AccountNumber": "123456789",
			"TransactionTypeId": "Debit",
			"TransactionDate": "2020-08-28T03:50:01",
			"BusinessDate": "2020-08-28T03:50:01",
			"AvailableBalance": 400.00,
			"Amount": 129.74,
			"Description": "Other: POS Transaction",
			"MerchantName": "Wally World",
			"MerchantId": "WWV-000-1220"
		}]
	}
}
```

With the given data write a VueComponent that gets this data from the VuexStore and displays the data. 

Your component should satisfy the following:
- Starting balance
- Ending balance
- List of Transactions
- Clearly define transaction information

Hint: Think of yourself as the user, what information do you need to know about the current status of your account.

___

## Submission
- Send an email to your Cascade contact with a link to your solution on your github account when completed.

Do not submit a PR. 
Do not ask for external assistance. 
Do not share solution or assessment with outside sources.

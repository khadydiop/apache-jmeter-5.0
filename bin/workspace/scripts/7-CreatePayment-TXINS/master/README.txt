Script 7-CreatePayment-TXINS

Pre-requirements:
1) Update UserID,PasswordID in file "users.csv" 
2) Account number 102546108RC0005 must exist for all users
3) Update dates in file "ProcessedDates.csv"


---Version 4
- Put first line with (UserID,PasswordID) in file users.csv and tell the JMeter script to ignore first line
- AccountNumber is now readed from a file (AccountId20.csv)
- Rename variable "requiredAfterSpacesForAccountNumber" to "spaces"
- Rename variable "_accountNumber" to "AccountNumber"

---VERSION 3
setUp Thread group is disabled
Add response assertion to check if account number (hard coded) exists  before doing payment
---VERSION 2
version without selecting the first account in the list provide the hard-coded account 102546108RC0005
This version also checks if the required account exists in the list

---VERSION 1
First version



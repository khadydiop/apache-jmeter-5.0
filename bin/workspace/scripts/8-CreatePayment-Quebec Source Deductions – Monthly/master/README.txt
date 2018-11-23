Script 8-CreatePayment-Quebec Source Deductions – Monthly

Pre-requirements:
1) Update UserID,PasswordID in file "users.csv" 
2) Account number 10341326380001 must exist for all users
3) Update dates in file "ProcessedDates.csv"

Version 6
- Put first line with (UserID,PasswordID) in file users.csv and tell the JMeter script to ignore first line
- AccountNumber is now readed from a file (AccountId302.csv)
- Rename variable "_csrf" to "sessionId" 
- Rename variable "requiredAfterSpacesForAccountNumber" to "spaces"


Version 5
  - Modified to use static account number from variable instead of first from list.
  Note : Assumes the payment type has 2+ accounts (instead of 1+) to work properly.
  
  - Added assert to check if static account number is in page/list.

Version 4
  - Renamed tests.
  - Added no "technical problem" assert post-login.

Version 3
  - Parameter bug fix for 3+ accounts for payment type

Version 2
  - Added initial GET of Login page for more real life load tests

Version 1
  - First version
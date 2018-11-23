Script 6-CreatePayment-PD7A

Pre-requirements:
1) Update UserID,PasswordID in file "users.csv" 
2) Note : Due to the changes, the script assumes the payment type have 2+ accounts (instead of 1+) to work properly. 
3) Account number NRK467815 must exist for all users
4) Update dates in file "ProcessedDates.csv"



Version 8
- Put first line with (UserID,PasswordID) in file users.csv and tell the JMeter script to ignore first line
- AccountNumber is now readed from a file (AccountId13.csv)
- Rename variable "requiredAfterSpacesForAccountNumber" to "spaces"
- Remove Regular Expression Extract sessionId  with variable "_csrf" , the one with "sessionId" exists already

Version 7
  - Adapted script to use static account number instead of auto-picking first in list.
 

Version 6
  - Renamed sessionId.

Version 5
  - Added "technical problem" assert post-login.
  - Renamed test.

Version 4
  - Adapted to read payment dates from ProcessedDates.csv instead of hardcoded.

Version 3
  - Auto-extracts the quantity of accounts of the payment type so the script works for 2+ accounts instead of a set quantity.

Version 2
  - Auto-extracts the first account number in the 2nd page post-login

Version 1
  - First version
Version 4
 - General fixes.
 - Rename variable "spaces" to "spacesAfterAccount"

Version 3
 - Put first line with (UserID,PasswordID) in file users.csv and tell the JMeter script to ignore first line
 - AccountNumber is now readed from a file (AccountId305.csv)
 - Rename variable "requiredAfterSpacesForAccountNumber" to "spaces"

Version 2
 - Reads from new CSV QuebecGSTQSTDates.csv for date data. CSV have September 2019 dates.
 - Added assert if account number doesn't exist in page.
 - Account number is now static in a variable instead of picking the first of the list.
   NOTE : Script will only be usable with a user's payment type with 2+ accounts (not 1+).

Version 1
 - First version
   NOTE : Missing reading from a date CSV and inputing dates from CSV
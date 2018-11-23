Requirements to run the script :
  - Payment Type "Quebec Payroll Source Deductions -Monthly/Yearly" for the multi-authorization company must have 2+ accounts.
  - Correct users and passwords must be specified in usersPending.csv and usersForApproval.csv
  - Users in usersPending.csv and usersForApproval.csv must be different. One user cannot create and approve the same transaction.
  - An existing account of the payment type must be written in AccountsCreateApprove_TPZ-1015.csv.
  - Correct form dates must be written in ProcessedDates.csv.
  - Accounts must be cleaned from the approval list.

Version 4
  - Adapted script to use again different CSV names.  
  - Split user+account CSV into an user CSV and an account CSV.
  
Version 2
  - Adapted script to use CSVs with headers.
  - Adapted script to use different CSV names.
  - CSVs has different account numbers.
  
Version 1
  - First version
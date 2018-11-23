Requirements to run the script :
  - Payment Type "Payment Federal Payroll Deductions - Monthly/Quarterly -- EMPTX -- (PD7A)" for the multi-authorization company must have 2+ accounts.
  - Correct users and passwords must be specified in usersPending.csv and usersForApproval.csv
  - Users in usersPending.csv and usersForApproval.csv must be different. One user cannot create and approve the same transaction.
  - An existing account of the payment type must be written in AccountsCreateApprove_PD7A.csv.
  - Correct form dates must be written in ProcessedDates.csv.
  - Accounts must be cleaned from the approval list.

Version 5
  - Adapted script to use again different CSV names.  
  - Split user+account CSV into an user CSV and an account CSV.
  
  
Version 4
  - Adapted script to use CSVs with headers.
  - Adapted script to use different CSV names.
  - CSVs has different account numbers.
  
Version 2
  - In the approval list, support to verify in the first 100 rows instead of 25.
  - Corrections to use usersApproverPaymentType2.csv for the approval part of the script.
  
Version 1
  - First version.
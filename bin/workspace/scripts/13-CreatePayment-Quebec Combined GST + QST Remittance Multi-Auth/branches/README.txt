Requirements to run the script :
  - Payment Type "Quebec Combined GST QST Remittance" for the multi-authorization company must have 2+ accounts.
  - Correct users and passwords must be specified in usersPending.csv and usersForApproval.csv.
  - Users in usersPending.csv and usersForApproval.csv must be different. One user cannot create and approve the same transaction.
  - An existing account of the payment type must be written in AccountsCreateApprove_GST_HST.csv.
  - Correct form dates must be written in QuebecGSTQSTDates.csv.
  - Accounts must be cleaned from the approval list.

Version 4
  - Adapted script to use again different CSV names.  
  - Split user+account CSV into an user CSV and an account CSV.
  
Version 3
  - Adapted script to use CSVs with headers.
  - Adapted script to use different CSV names.
  - CSVs has different account numbers.
  
Version 2
  - Minor comment corrections.
  
Version 1
  - First version
Requirements to run the script :
  - Payment Type "Quebec Payroll Source Deductions -Monthly/Yearly -- PAY -- (TPZ-1015.R.14.1)" for the multi-authorization company must have 2+ accounts.
  - Correct users and passwords must be specified in usersPendingPaymentType5.csv and usersApproverPaymentType5.csv
  - Users in usersPendingPaymentType5.csv and usersApproverPaymentType5.csv must be different. One user cannot create and approve the same transaction.
  - An existing account of the payment type must be written in usersPendingPaymentType5.csv and usersApproverPaymentType5.csv.
  - Correct form dates must be written in ProcessedDates.csv.
  - Accounts must be cleaned from the approval list.

Version 1
  - First version
Requirements to run the script :
  - Payment Type "Payment Federal Payroll Deductions - Monthly/Quarterly -- EMPTX -- (PD7A)" for the multi-authorization company must have 2+ accounts.
  - Correct users and passwords must be specified in usersPendingPaymentType2.csv and usersApproverPaymentType2.csv
  - Users in usersPendingPaymentType2.csv and usersApproverPaymentType2.csv must be different. One user cannot create and approve the same transaction.
  - An existing account of the payment type must be written in usersPendingPaymentType2.csv and usersApproverPaymentType2.csv.
  - Correct form dates must be written in ProcessedDates.csv.
  - Accounts must be cleaned from the approval list.

Version 2
  - In the approval list, support to verify in the first 100 rows instead of 25.
  - Corrections to use usersApproverPaymentType2.csv for the approval part of the script.
  
Version 1
  - First version.
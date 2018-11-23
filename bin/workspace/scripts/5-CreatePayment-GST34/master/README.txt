
Script 5-CreatePayment-GST34

Pre-requirements:
1) Make sure that GST34 payments DO NOT exist for the hard-coded account 123481731RT1001 (simple form) and 123481731RT1002 (form with schedules)
2) Update users in file "users.csv"
3) Update dates in file "ProcessedDates.csv"
 

---VERSION 3
- Rename variable "_accountNumber" to "AccountNumber"
- Rename variable "requiredAfterSpacesForAccountNumber" to "spaces"
- AccountNumber 123481731RT1001 is now parameted in file "AccountId34-1.csv"
- AccountNumber 123481731RT1002 is now parameted in file "AccountId34-2.csv"


---VERSION 2
version without selecting the first account in the list provide the hard-coded account 123481731RT1002

Script FederalTax34_WithoutSchedulesB_C_v_01 has not completed. 
The following should be added:
 - Read user credetilals  
 - dynamic count of the accounts for the payment type
 - variables for the user credentials, accountNumber, dates.
Pre-requisite - no unprocessed payments for the account should be available.

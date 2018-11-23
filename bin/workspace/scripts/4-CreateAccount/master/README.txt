Script of Creating Account

Pre-requirements:
1) Update UserID,PasswordID in file "users.csv" 
2) Before using script "pfs-CreateAccount-v3.jmx" for  Creating Account - Federal - Excise Duty -- FDEXD, change the account number  in script. 
3) Advise to use script "pfs-CreateAccount-v2-Multiple.jmx" to create account for several payment type
4) Update file "RB_PaymentTypesForJMeter.csv" before running script "pfs-CreateAccount-v2-Multiple.jmx"
5) In the script "pfs-CreateAccount-v2-Multiple.jmx" Loop Controller (Loop all payment types for a same user) is initialed to 10. Make sure it is the quantity needed in test case
6) Be careful on creating account number , a wrong syntax can fail the script

**************type : Federal Payroll Deductions - Monthly/Quarterly -- EMPTX -- (PD7A) 
Account number is 15 characters long - pattern is 'nnnnnnnncRPnnnn' consisting of:
  - a 9 digit number
  - 'RP' as a constant 
  - 4 digits in the last positions as a sequence number for the account (0001, 0002, etc)

or Account number is 9 characters long - pattern is 'NRannnnnc' consisting of:
  - 'NR' as a constant
  - one alpha character from 'A' to 'Z'
  - a 6 digit number
NRB467815 for example

**********type : QUEBEC COMBINED GST/HST + QST REMITTANCE -- G-QST -- (FPZ-500.IF)
Account number is 16 characters long - pattern is 'nnnnnnnnncTQnnnn' consisting of:
  - a 10 digit number
  - 'TQ' as a constant (QST identifier)
  - 4 digits in the last positions as a sequence number for the account (0001, 0002, etc)

Note:  some enrollment forms may have only 10 digits, if so add 'TQ0001' at the end.
1034132638TQ0004 for example

**********type:Federal - Corporation Tax Payments -- TXINS
 Account number is 15 characters long - pattern is 'nnnnnnnncRCnnnn' consisting of:
  - a 9 digit number
  - 'RC' as a constant 
  - 4 digits in the last positions as a sequence number for the account (0001, 0002, etc) 
102546108RC0011 for example  
  
**********type:Federal - GST/HST  Return and Payment -- GST34 -- (GST34)  
 Account number is 15 characters long - pattern is 'nnnnnnnncRTnnnn' consisting of:
  - a 9 digit number
  - 'RT' as a constant 
  - 4 digits in the last positions as a sequence number for the account (0001, 0002, etc)
135555555RT0005 for example  
 
**********type:QUEBEC COMBINED GST/HST + QST REMITTANCE -- G-QST -- (FPZ-500.IF) 
Account number is 16 characters long - pattern is 'nnnnnnnnncTQnnnn' consisting of:
  - a 10 digit number
  - 'TQ' as a constant (QST identifier)
  - 4 digits in the last positions as a sequence number for the account (0001, 0002, etc)

Note:  some enrollment forms may have only 10 digits, if so add 'TQ0001' at the end.
1034132638TQ0005 for example

***********type:Quebec Payroll Source Deductions -Monthly/Yearly -- PAY -- (TPZ-1015.R.14.1) 
Account numbers are 14 digits long composed of: 
 -a 10 digit registrant number 
 -a 4 digit file number 

Note: some enrollment forms may have: 
 -a 10 digit number followed by 'RS': if so, strip off the two letters 'RS' and replace by '0001' 
 -a 10 digit number: if so, add 0001 to the end
10341326380007 for example
 

Version 3
- Put first line with (UserID,PasswordID) in file users.csv and tell the JMeter script to ignore first line
- Change name of variable _csrf to sessionId
- Change Loop count from 10 to 5 in Loop Controller (Loop all payment types for a same user)-script "pfs-CreateAccount-v2-Multiple.jmx"
 
Version 2
  - Renamed tests
  - Renamed sessionId
  WARNING : Script still fails for user #1

Version 1
  - First version
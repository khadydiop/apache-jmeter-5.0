Version 7
  - Adapted script to use static account number instead of auto-picking first in list.
  Note : Due to the changes, the script assumes the payment type have 2+ accounts (instead of 1+) to work properly.

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
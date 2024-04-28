
Feedback from @nancy
1. ~~Gross Principal Amount Charged Off should always be greater than Net Principal Amount Charged Off. (The point seems wrong)~~
2. ~~WHEN STATUS = CHARGE_OFF THEN NULL ELSE OUTSTANDING~~~~

FIXES:
1. LAST_PAYMENT_DATE IS ALWAYS LATEST
2. ~~NET CHARGE OFF AMOUNTS ARE BEING CALCULATED EVEN WHEN CHARGE OFF IS NOT DONE~~
3. CHAR OFF WAS DONE ON 31 BUY AMOUNT WAS MOVED EARLIER, ALSO NET CHARGE OFF IS FILLED IN ALL ROWS
   ![[Pasted image 20240417130932.png]]
4. ~~Change source of cohort from accounts to min_created at from lending_transactions~~



## UPDATES

1. Add is_incremental block on the limit and filter condition
2. make it easier to backfill (explore edits to the execution command on deployment ??)
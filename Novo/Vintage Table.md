1. acrued revenue
2. monthly renvue (FACTOR FEE + LATE_FEE)
3. total /monthly amount drawn
4. Credit Limit
5. principal balance
6. DQ FLAG /
7. DQ CURED / -- max dq till date vs current dq
9. DQ BUCKET / -- based on max dq
10. INTERNAL_P_CHARGE_OFF (60 DPD)
11. INTERNAL_F_CHARGE_OFF (60 DPD)
12. INTERNAL_T_CHARGE_OFF (60 DPD)
13. NET REV : ACRUED - CO
14. Cost of Funds : 11 % (monthly level just /12)
15. ADD AGED_FLAG USING SNAP_DATE > FIRST_MIN_PAY_DUE

## CHECKS:
1. ROW 6 seems off

## TASK LIST
- Look into backfilling the data prior to 01/04/2023
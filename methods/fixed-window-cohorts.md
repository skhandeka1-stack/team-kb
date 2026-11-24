# Compare fixed-window cohort rates

Choose a start event, an eligibility rule, an outcome, and a fixed follow-up window before computing rates. Start the clock at each unit's own start event. Use one row per eligible unit and count each outcome once per unit.

For a 30-day outcome, wait until each included unit has had 30 days of observation or use a method that explicitly handles censoring. Report recent cohorts with incomplete follow-up separately. If event collection lags, account for that lag before closing the window.

In an invented example, 18 of 120 eligible accounts activated within 30 days, or 15%. In a later mature cohort, 22 of 110 activated, or 20%. Report both counts and the five percentage-point difference. Check sample uncertainty, enrollment mix, and concurrent changes before attributing the difference.

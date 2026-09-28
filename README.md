# MechaCar statistical analysis

An R console transcript records a multiple linear regression of MPG and an analysis of suspension coil PSI. The regression reported R² = 0.7032; vehicle length and ground clearance had p-values below 0.05 in that sample. This is association in the fitted model, not proof of causation.

The overall coil PSI variance shown was 62.29356. The transcript reports a Lot 3 mean of 1496.14 PSI and a one-sample t-test p-value of 0.04168 against 1500 PSI. The earlier README listed inconsistent t-test values and incorrectly claimed that every lot met the variance limit. The lot-level variance values cannot be confirmed from the available text summary, so they are not asserted here.

![Overall coil summary](Total_Summary.png)
![Lot summary](Lot_Summary.png)
![All lots t-test](test_all_lots.png)
![Lot 3 t-test](test_lot3.png)

[Console transcript](MechaCarChallenge.RScript) · [MPG data](MechaCar_mpg%5B1%5D.csv)

The suspension coil input CSV is absent; the transcript uses local Windows file paths and contains exploratory errors. The saved outputs are historical and the full coil analysis cannot be reproduced from this repository alone.

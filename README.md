# Medical Equipment Suppliers Project

## Libraries Used
pandas, numpy, matplotlib, seaborn, scikit-learn

## Motivation
I wanted to find out if we can predict whether a medical equipment supplier
will accept Medicare's payment rate or not. This matters because patients need
to know in advance which suppliers will not charge them extra on top of what
Medicare covers.

## Files
- `MedicalEquipmentSuppliers_Project.ipynb` — the full analysis notebook
- `Medical-Equipment-Suppliers.csv` — the dataset (57,632 suppliers across the US)
- `README.md` — this file

## Dataset
The dataset was downloaded from the Centers for Medicare and Medicaid Services (CMS).
If you need to download it again you can get it directly from here:

https://data.cms.gov/provider-data/sites/default/files/resources/3b76abb9b6f610373563b5ef08bb0d81_1777163606/Medical-Equipment-Suppliers.csv

Place the CSV file in the same folder as the notebook before running it.

## Summary of Results
The Random Forest model reached around 87% accuracy which was much better
than Logistic Regression at 69%. The most useful features turned out to be
the number of supply types a provider offers, their location, and the year
they joined Medicare. Encoding the state column with pd.get_dummies() also
helped improve the results without slowing things down too much.

## Acknowledgments
Dataset from the Centers for Medicare and Medicaid Services (CMS) — data.cms.gov

# Data Dictionary

This dictionary is based on the column headers present in the workbook. The raw worksheet contains 28 fields; the cleaned worksheet contains 33 fields, including derived variables. Descriptions below explain the apparent meaning of each field from its name. Where the workbook does not define coding rules or units, the description is intentionally cautious.

| Field | Description |
|---|---|
| `Patient_ID` | Simulated unique record identifier. |
| `State` | Nigerian state associated with the record. |
| `Geopolitical Zone` | Derived geopolitical-zone grouping. |
| `LGA` | Local Government Area. |
| `Age` | Patient age. |
| `Age_Group` | Derived age band. |
| `Marital_Status` | Marital-status category. |
| `Education_Level` | Education category. |
| `Occupation` | Occupation category. |
| `Religion` | Religion category. |
| `Parity` | Number of previous births/pregnancies as represented in the dataset; confirm the intended definition in the project methodology. |
| `ANC_Visits` | Number of antenatal-care visits recorded. |
| `Gestational_Age_Weeks` | Gestational age in weeks. |
| `Booking_Status` | Whether the pregnancy was booked/registered for antenatal care, according to the dataset's categories. |
| `Delivery_Mode` | Mode of delivery. |
| `Place_of_Delivery` | Recorded delivery location. |
| `Skilled_Birth_Attendant` | Whether a skilled birth attendant was recorded. |
| `Distance_to_Facility_km` | Distance to a health facility; numeric values are intended to represent kilometres, but the cleaned sheet also contains a non-numeric value that requires review. |
| `Distance_Category` | Derived distance band. |
| `Referral_Status` | Recorded referral status. |
| `BP_Systolic` | Systolic blood pressure reading; unit and measurement protocol are not specified in the workbook. |
| `BP_Diastolic` | Diastolic blood pressure reading; unit and measurement protocol are not specified in the workbook. |
| `Hemoglobin_g_dl` | Haemoglobin value, labelled in grams per decilitre. |
| `Cause_of_Complication` | Recorded complication/cause category. |
| `Blood_Transfusion_Given` | Whether blood transfusion was recorded. |
| `Maternal_Outcome` | Maternal outcome category, including `Maternal Death` and `Survived`. |
| `Newborn_Outcome` | Newborn outcome category. |
| `Admission_Date` | Admission date. |
| `Discharge_Date` | Discharge date. |
| `Household_Income_Naira ` | Household income in Nigerian naira; the source header includes trailing whitespace. |
| `Insurance_Status` | Health-insurance status category. |
| `Maternal_Death_Flag` | Derived binary indicator for maternal-death outcome (0/1 as represented in the workbook). |
| `Length _of _Stay_Days` | Derived length of stay in days; the source header includes internal spaces. |

## Additional derived fields in the cleaned worksheet

- `Geopolitical Zone`
- `Age_Group`
- `Distance_Category`
- `Maternal_Death_Flag`
- `Length _of _Stay_Days`

The workbook does not include a separate formal data-dictionary tab specifying every category, validation rule, or derivation formula. These should be documented as the SQL and Python stages are developed.

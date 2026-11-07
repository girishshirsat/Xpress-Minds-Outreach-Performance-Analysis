# Xpress Minds Data Intern Assessment
 
Submission for the Xpress Minds Edutainment Data Intern Practical Assessment. The task was to clean a messy school database, research missing details, analyse outreach performance and report the findings.
 
**Note:** The school data is synthetic practice data. No institution from it was contacted.
 
## Files
 
| File | What it is |
|---|---|
| `XM_Data_Intern_Assessment_Cleaned.xlsx` | Completed workbook with cleaned data, logs and research |
| `Xpress_Minds_Outreach_Report.pdf` | 2-page summary report |
| `Dashboard_.png` | Screenshot of the Power BI outreach dashboard |
 
### Workbook sheets
 
- `School_Data` and `Outreach_Data`: cleaned tables (104 records each, linked by `Record_ID`)
- `Cleaning_Log`: every change made, with the original value, new value and reason
- `Duplicate_Log` and `Duplicate_Review`: duplicate decisions and the repeated names that were reviewed
- `Research_Log`: public-source research for missing website and email values
## Approach
 
### 1. Cleaning
 
- Removed 3 exact duplicate records (XM-108, XM-117, XM-171) from both sheets
- Kept schools with the same name in different cities, treating them as separate branches
- Standardised school-name capitalisation, board labels ("State Borad" to STATE BOARD), city names ("Bombay" to Mumbai), email case and the +91 phone prefix
- Left missing emails, websites and dates blank and flagged them instead of guessing
- Flagged status and flag conflicts for source checking instead of overwriting them
### 2. Research
 
- 14 entries logged in `Research_Log` (8 email checks, 6 website checks)
- Each entry records the source URL, date checked, confidence and notes
- Because the source data is synthetic, a real school with a similar name is treated as a lead, not a confirmed match
### 3. Outreach analytics
 
| Metric | Value |
|---|---|
| Total records | 104 |
| Contacted | 75 |
| Contact rate | 72.1% |
| Response rate (provisional) | 85.3% (64 of 75) |
| Interested rate (26 / 75) | 34.7% |
| Registration conversion (26 / 75) | 34.7% |
| Follow-ups due on or before 7 Nov 2026 | 30 |
 
Main findings:
 
- IB has the best reach (85% contacted).
- State Board shows high interest (7 of 14 contacted) but the lowest registration (3 of 14).
- Kochi leads on registrations. Lucknow and Mumbai have contacted schools but no registrations yet.
### 4. Recommendations
 
1. Clear the follow-up backlog, starting with the 17 live records.
2. Improve the State Board interest-to-registration step with a second call within 7 days.
3. Contact the 29 uncontacted schools, starting with cities that already convert (Bhubaneswar, Delhi, Ahmedabad).
### 5. Weekly database maintenance
 
Monday: import into a staging sheet. Tuesday: clean and validate. Wednesday: reconcile statuses and flags. Thursday: research a fixed batch of missing details. Friday: refresh the dashboard and share follow-ups due. Full details are in the PDF report.
 
## Assumptions and limitations
 
- `Record_ID` links the two sheets. KPIs use the 0/1 flag columns, and interested and registration rates use contacted records as the base.
- "Follow-ups due" means a `Next_Follow_Up` date on or before 7 November 2026.
- The response rate counts contacted records whose `Response_Status` is not "No response". It is provisional because some records marked as not contacted still carry a response status.
- 16 records have `Registered_Flag = 1` without a Registered status. They were flagged, not changed, so registration figures could move after a source check.
- Nothing was inferred or invented. Unverified values are labelled as such.
## Tools
 
Microsoft Excel for cleaning and logs, Power BI for the dashboard.
 
## Author
 
Girish Shirsath, girishshirsath2004@gmail.com
 

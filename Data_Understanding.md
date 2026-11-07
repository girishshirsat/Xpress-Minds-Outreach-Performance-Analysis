# Xpress Minds Worksheet

## Spread Sheet 1: School_Data (Dataset)
- 107 Rows + 1 Heading = 108 Rows
- 12 Different Columns + 1 Dublicate = 13 Column  
  - Record_ID
  - School_Name
  - City
  - District
  - Board
  - Website
  - Contact_Name
  - Email
  - Phone
  - Outreach_Status
  - Last_Contact_Date
  - Next_Follow_Up
  - Response_Status

- Unit of measurement: All columns had default general datatype in excel we have to fix
- Last Conatact Date Prtiod: 1 Oct 2026 to 31 Oct 2026
- Primary key: Not specific but Record_ID is the most soutable
- 6 Contact No dont have +91 prefix
- the city and district both columns are same but the mismatch is city=Delhi::District=New Delhi (four to five row) and city=Bombay::District=Surat(only one row)


- Column wise data Understanding 

|Name|meaning|Data_type|Format|Unique_values|Duplicate_values|Unique_dublicate|Blank_values| Constant_values | Categorical_columns |Numerical_columns | Date_columns|    
|----|-------|---------|------|-------------|----------------|----------------|------------|-----------------|---------------------|------------------|-------------|
| Record_ID |key to identify recrd| General | alpha_num  | 107| 0| 0|0 |107|No|No|No|
|School_Name|name org | Geeral | text | 82|43|25|0|NO|NO|NO|NO|
|City|locaton|General|text|NA|NA|NA|0|NO|NA|NO|No|
|District| location|General|text|NA|NA|na|0|NO|No|NO|NO|
|Board|the gov authorization associated with org|General|text|6|NA|NA|0|No|No|No|No|
|Website|Web adress|General|link|76|46|31|5|NA|No|No|No|
|Contact_Name| name of org othorized person|General|text|15|107|15|0|NA|No|No|No|
|Email|org email id|General|email|78|36|29|9|NA|NO|NO|NO|
|Phone|org contact No| General|numeric|103|8|4|0|NA|No|Yes|No|
|Outreach_Status|weather they are interested or not|General|text|NA|Na|NA|0|NA|YES|NO|NO|
|Last_Contact_Date| data of recent contact|General|Date|NA|NA|NA|49|NO|NO|NO|YES|
|Next_Follow_Up|Shedule of upcoming contact|General|Date|NA|NA|NA|74|NA|No|No|Yes|
|Response_Status| what their stand|General|text|6|NA|NA|0|NA|YES|NO|NO|



## Spread Sheet 2: Outreach_Data (Dataset)
- 107 Rows + 1 Heading = 108 Rows
- 11 Different column
  - Record_ID
  - School_Name
  - City
  - Board
  - Outreach_Status
  - Contacted_Flag
  - Response_Status
  - Interested_Flag
  - Registered_Flag
  - Last_Contact_Date
  - Next_Follow_Up

- Unit of measurement: All columns had default general datatype in excel we have to fix

- Last Conatact Date Priod: 1 Oct 2026 to 31 Oct 2026
- Next_Follow_Up Date Period: 7 Oct 2026 to 9 Nov 2026
- Primary key: Not specific but Record_ID is the most soutable

- Column wise data Understanding 

|Name|meaning | Data_type | Format | Unique_values| Duplicate_values | Blank_values | Constant_values | Categorical_columns | Numerical_columns | Date_columns|    
|----|--------|-----------|--------|--------------|------------------|--------------|-----------------|---------------------|-------------------|-------------|
| Record_ID |key to identify recrd| General | alpha_num  | 107| 0| 0 |107|No|No|No|
|School_Name|Org name|General| text |82|43|0|NA|NO|NO|NO|
|City| Location|General|text|21|NA|0|NA|NO|NO|NO|
|Board|the gov authorization associated with org|General|Text|6|NA|0|NA|NO|No|NO|
|Outreach_Status| weather they are interested or not | General|text|7|NA|0|NA|No|YES|NO|NO|
|Contacted_Flag|it may indicating contacted or not|General|numeric|No|NA|0|2|YES|Yes|NO|
|Response_Status|what responce from org|General|text|6|NA|0|NO|YES|NO|NO|
|Interested_Flag|weather thy are interested or not|General|numeric|2|NA|0|NA|YES|YES|NO|
|Registered_Flag|weather thy had registered or not|General|numeric|2|NA|0|NO|YES|YES|NO|
|Last_Contact_Date|date of recently contact|General|date|NA|NA|49|No|NO|NO|YES|
|Next_Follow_Up| upcoming contact date| General|Date|NA|NA|74|NA|NO|NO|YES|



## Understanding of both sheets

- The Record_ID, School_Name,City,Outreach_Status, Last_Contact_Date, Next_Follow_Up, and Response_Status  checked row by row all are exactly match in both table

- Board are not matching (only 20 matching that is all CBSC)


## Duplicate Details

# Part 1: School Data
 
## Record_ID
There are no duplicates. Every record has its own unique ID.
 
## School_Name
- 17 school names are repeated.
- There are 22 extra entries, and the repeated names appear 39 times in total.
### Names that appear more than twice:
- Indus International School appears 4 times.
- Quest Public School appears 3 times.
- Elm Public School appears 3 times.
- Riverview School appears 3 times.
### Names that appear exactly twice:
- Zenith Public School
- Coral Vidyalaya
- Gateway International School
- Zenith Global School
- Westbridge Academy
- Valley Academy
- Trinity Global School
- Valley Vidyalaya
- Cedar Academy
- Summit High School
- Zenith Academy
- Horizon School
- Oakridge International School
## City
- 20 cities are repeated.
- There are 84 extra entries, and the repeated cities appear 104 times in total.
- Repetition is expected here, because many schools can be in one city.
From most to least frequent:
- Delhi (10)
- Jaipur (9)
- Bhubaneswar (9)
- Ahmedabad (7)
- Mumbai (6)
- Kochi (6)
- Indore (6)
- Bengaluru (5)
- Guwahati (5)
- Nagpur (5)
- Lucknow (5)
- Kolkata (5)
- Chennai (5)
- Pune (4)
- Hyderabad (4)
- Gurugram (4)
- Nashik (3)
- Vadodara (2)
- Surat (2)
- Bhopal (2)
## District
- 20 districts are repeated.
- There are 87 extra entries, and the repeated districts appear 107 times in total.
- The pattern matches City closely. The main differences are that Delhi is recorded as New Delhi, Chennai has 6 entries, Pune has 5, and Surat has 3.
From most to least frequent:
- New Delhi (10)
- Jaipur (9)
- Bhubaneswar (9)
- Ahmedabad (7)
- Kochi (6)
- Indore (6)
- Mumbai (6)
- Chennai (6)
- Guwahati (5)
- Nagpur (5)
- Lucknow (5)
- Bengaluru (5)
- Kolkata (5)
- Pune (5)
- Gurugram (4)
- Hyderabad (4)
- Nashik (3)
- Surat (3)
- Vadodara (2)
- Bhopal (2)
## Board
- 6 board types are repeated.
- There are 101 extra entries, and the values appear 107 times in total. Every record shares its board with other records, which is normal for a category field.
Counts:
- ICSE: 24
- CBSE: 20
- IB: 20
- IGCSE: 20
- State Board: 20
- CBSE / ICSE: 3
## Website
- 19 website addresses are repeated.
- There are 27 extra entries, and the repeated websites appear 46 times in total.
- Repeated websites suggest the same school may be listed more than once.
Most repeated:
- indusinternational.edu.in appears 5 times.
- elmpublicschool.edu.in appears 4 times.
- questpublicschool.edu.in, oakridgeinternatio.edu.in and riverviewschool.edu.in appear 3 times each.
Appearing twice each:
- westbridgehighscho.edu.in
- zenithglobalschool.edu.in
- valleyvidyalaya.edu.in
- pioneerpublicschoo.edu.in
- gatewayinternation.edu.in
- trinityglobalschoo.edu.in
- summithighschool.edu.in
- horizonschool.edu.in
- summitpublicschool.edu.in
- cedaracademy.edu.in
- northstaracademy.edu.in
- westbridgeacademy.edu.in
- valleyacademy.edu.in
- zenithacademy.edu.in
All of these use the full form `https://www.<name>.edu.in`.
 
## Contact_Name
- 15 contact names are repeated.
- There are 92 extra entries, and the repeated names appear 107 times in total.
- Almost every record shares its contact person with other records. This could mean a small pool of contacts handles many schools, or that placeholder names were reused.
Counts:
- Ishita Bose: 13
- Neha Menon: 10
- Maya Shah: 9
- T. Sharma, Rahul Mehta, Nidhi Kapoor, Amit Verma and Karan Singh: 8 each
- Vikram Reddy, R. Kulkarni and Sonal Joshi: 7 each
- S. Iyer: 6
- Arvind Nair: 4
- Pooja Das and Ananya Rao: 2 each
## Email
- 12 email addresses are repeated.
- There are 15 extra entries, and the repeated emails appear 27 times in total.
Most repeated:
- office@indusinternational.edu.in appears 4 times.
- office@elmpublicschool.edu.in appears 3 times.
Appearing twice each:
- office@zenithpublicschool.edu.in
- office@coralvidyalaya.edu.in
- office@oakridgeinternatio.edu.in
- office@gatewayinternation.edu.in
- office@westbridgeacademy.edu.in
- office@riverviewschool.edu.in
- office@summithighschool.edu.in
- office@horizonschool.edu.in
- office@trinityglobalschoo.edu.in
- office@cedaracademy.edu.in
## Phone
- 4 phone numbers are repeated.
- There are 4 extra entries, and the repeated numbers appear 8 times in total.
- Each of these numbers appears exactly twice:
  - +91 99921 84341
  - +91 87096 95256
  - +91 86199 62383
  - +91 83903 42780
## Outreach_Status
- 7 status values are repeated.
- There are 100 extra entries, and the values appear 107 times in total.
Counts:
- Not contacted: 30
- Contacted: 21
- Responded: 19
- Interested: 12
- Registered: 10
- Not interested: 8
- Follow-up due: 7
## Last_Contact_Date
- 17 dates are repeated.
- There are 31 extra entries, and the repeated dates appear 48 times in total.
- All dates fall in October 2026.
Dates with 4 contacts each:
- 2026-10-07
- 2026-10-08
- 2026-10-11
- 2026-10-15
Dates with 3 contacts each:
- 2026-10-04
- 2026-10-09
- 2026-10-12
- 2026-10-22
- 2026-10-27
- 2026-10-30
Dates with 2 contacts each:
- 2026-10-02
- 2026-10-13
- 2026-10-16
- 2026-10-17
- 2026-10-18
- 2026-10-23
- 2026-10-26
## Next_Follow_Up
- 8 dates are repeated.
- There are 11 extra entries, and the repeated dates appear 19 times in total.
Follow-up dates:
- 2026-10-23 has 4 follow-ups.
- 2026-10-15 has 3 follow-ups.
- 2026-10-10, 2026-10-18, 2026-10-22, 2026-10-27, 2026-10-29 and 2026-11-09 have 2 follow-ups each.
## Response_Status
- 6 response values are repeated.
- There are 101 extra entries, and the values appear 107 times in total.
Counts:
- Not interested: 24
- Registered: 20
- Interested: 20
- Asked for details: 17
- No response: 16
- Call back: 10
---
 
# Part 2: Outreach Data
 
The Outreach Data covers the same 107 records. Most fields repeat what is in Part 1, so the results below are identical for those fields. Three flag fields are new.
 
## Record_ID
There are no duplicates.
 
## School_Name
The results are the same as in Part 1. 17 names are repeated, with 22 extra entries and 39 total occurrences. Indus International School appears 4 times, Quest Public School, Elm Public School and Riverview School appear 3 times each, and the remaining 13 names appear twice each.
 
## City
The results are the same as in Part 1. 20 cities are repeated, with 84 extra entries and 104 total occurrences. Delhi leads with 10, followed by Jaipur and Bhubaneswar with 9 each.
 
## Board
The results are the same as in Part 1. ICSE has 24, CBSE, IB, IGCSE and State Board have 20 each, and CBSE / ICSE has 3.
 
## Outreach_Status
The results are the same as in Part 1. Not contacted has 30, Contacted 21, Responded 19, Interested 12, Registered 10, Not interested 8 and Follow-up due 7.
 
## Contacted_Flag
This is a yes/no marker, so only two values exist and both repeat.
- 1 (contacted) appears 77 times.
- 0 (not contacted) appears 30 times.
The 30 uncontacted records match the 30 "Not contacted" entries in Outreach_Status.
 
## Response_Status
The results are the same as in Part 1. Not interested has 24, Registered 20, Interested 20, Asked for details 17, No response 16 and Call back 10.
 
## Interested_Flag
- 0 (not interested) appears 79 times.
- 1 (interested) appears 28 times.
## Registered_Flag
- 0 (not registered) appears 80 times.
- 1 (registered) appears 27 times.
## Last_Contact_Date
The results are the same as in Part 1. 17 dates are repeated, with 31 extra entries and 48 total occurrences.
 
## Next_Follow_Up
The results are the same as in Part 1. 8 dates are repeated, with 11 extra entries and 19 total occurrences.
 
---
 
# Key Takeaways
 
- **Record_ID is clean.** No ID is duplicated.
- **Likely duplicate schools.** School names, websites and emails repeat, and Indus International School, Elm Public School, Quest Public School and Riverview School repeat the most. These should be checked and merged if they are the same school.
- **Phone numbers are mostly unique.** Only 4 numbers appear twice.
- **Many repeats are normal.** City, District, Board and the status fields are category-type fields, so repetition is expected.
- **Contact names are heavily shared.** Ishita Bose appears in 13 records and Neha Menon in 10.
- **Outreach progress.** 77 of the 107 schools have been contacted, 28 are marked interested and 27 are marked registered.
- **Upcoming follow-up.** The busiest follow-up date is 2026-10-23, with 4 follow-ups scheduled.
 



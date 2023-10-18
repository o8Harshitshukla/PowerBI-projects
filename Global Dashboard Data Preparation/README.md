# Global Dashboard Data Preparation

In our quest to create a Global Dashboard with key metrics that serve all stakeholders in their decision-making, we have embarked on the crucial initial step of ensuring that the data is complete, clean, and can be seamlessly connected to our dashboard. To achieve this, we have collaborated with various analysts who are responsible for providing data from different regions and sources.

#### Dataset Link: [here](https://docs.google.com/spreadsheets/d/1JHy0_b1bYDuUx2-La-YcgqngKDhRKahi/edit?usp=sharing&ouid=116644621887200689615&rtpof=true&sd=true)

## Final Dashboard: 
![Capture7](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/060cc71e-c83f-46e5-aa30-f8e4d1bd5a94)

![Capture8](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/88c03876-c417-4175-83f6-93ab336606d1)

![Capture9](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/03d265ed-53a4-4dfd-9ea9-9de70629ce6c)

![Capture10](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/f909b825-bdc4-420f-80d1-d839a6ad9730)

![Capture11](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/7671d22f-118f-4375-932d-2d0a7850467b)

![Capture12](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/c175b1da-96a4-4d73-89e8-168a15db8563)

## Task 1: Importing Data from Google Sheets

We initiated the data acquisition process by requesting all analysts to put their respective datasets into a standard format and share them on Google Sheets. Once we received the data, we established a real-time connection to these Google Sheets to ensure that our dashboard's metrics stay updated automatically without manual intervention.

### Steps for Importing Data from Google Sheets:

**Step 1: Publish Google Sheets as a Web Page**
1. Share the Google Sheets document with the setting "Anyone with the link can view."
2. Navigate to 'File' => 'Publish to the web.'
3. Choose 'Entire document' and 'Web page' and click 'Publish.'

**Step 2: Enter Data into Power BI**
1. Open Power BI Desktop and create a new file.
2. Click 'Get data' and select 'Web' as the source.
3. Paste the URL from the Google Sheets document into the dialogue box.
4. Choose the Google Sheets URL as the data source.
5. Select the relevant tables (Regional tables, Payslips, and Mapping sheet) and click 'Load.'

**Step 3: Clean and Rename Tables in Query Editor**
1. Open the Power Query Editor to clean and organize the imported data.
2. Rename the tables to match the names in the original dataset.
3. Remove any blank rows.
4. Remove the first column if unnecessary.
5. Set the first row as headers for each table.
6. Repeat these steps for all imported tables.
7. Click 'Close and Apply' to save the changes.

## Task 2: Combining Regional Invoice Details

In the Power Query view, we combined the Regional Invoice details tables into one main table called 'Main Table.' This consolidation enables us to work with a unified dataset for analysis and visualization.

### Steps to Combine Regional Invoice Details:

1. Append two Regional tables into one table, naming it 'Main Table.'
2. We performed basic cleaning, which involved replacing all blanks and nulls in numeric fields with 0. Additionally, we ensured that numeric fields displayed two decimal points where necessary.

----------------------------------------------------------------------------------------------------------------

#### Question 1: What is the Total Count of records in the Main Table?
![Capture6](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/71a0b568-8270-4248-bf7b-dd843c7a5419)

#### Question 2: Which country has the highest count of Invoices?
![Capture13](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/cb919203-d908-4a1f-bf47-934d19aea466)

#### Question 3: What is the Count of Invoices for Singapore?
![Capture13](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/cb919203-d908-4a1f-bf47-934d19aea466)

#### Question 4: If you view the data on the basis of the highest Invoice amount, which country will come at the top?
![Capture14](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/dfe299e6-39ee-4985-8e81-a6e41ee4af61)

#### Question 5: Which Invoice number shows the highest amount?
![Capture15](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/728effa9-7077-47f0-863d-ae9c55b67d6e)

#### Question 6: Does the APAC region have the lowest Total Amount?
![Capture16](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/89e29745-d7da-49c7-b55b-91646fa90d40)

#### Question 7: What is the Total Amount for the Base month (in Millions) ?
![Capture17](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/53590945-6966-42fa-8d65-8544d2b0892b)

#### QUestion 8: : What is the Payslip Count for Base Month (in Millions) ?
![Capture17](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/53590945-6966-42fa-8d65-8544d2b0892b)

#### Question 9: What is the PPC for India?
![Capture18](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/c66239d8-2000-4f53-9653-75ee44133c87)

#### Question 10: What is the % share of the Top 2 Vendors? Name the Vendors?
![Capture19](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/410714ce-e5aa-4c2c-99fa-3f4d1a0cdabe)

#### Question 11: Which Region shows the biggest bubble, if size of the bubble is represented by the Total Amount?
![Capture20](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/f8971932-529e-4b84-9ae0-5a78ce2d151f)

#### Question 12: : What is the total Processing Cost for the Month of March 2020 for LATAM?
![Capture21](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/921ac6e4-b2d0-4546-bb0b-1b239b3b8fd1)

#### Question 13: How much Rebate did the Vendor ‘Vtl Inc.’ provide in Dec 2020?
![Capture22](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/aaca39e9-569e-49a8-9fb4-b1a0acf17894)

#### Question 14: : Which month shows the highest Payslip count for the EMEA region?
![Capture23](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/40ca06e6-50a6-4a2a-a010-492674614585)

#### Question 15: What is the Payslip count for Canada in Dec 2020?
![Capture24](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/566083f1-34db-42b8-a993-9d699a7cadf3)

#### Question 16: How much value does the line chart show on Aug 2020, if you filter on North America?
![Capture25](https://github.com/Nasir151/Power-BI-Projects/assets/94509995/68e9aa05-2b00-4e9c-967d-a259e3361c84)

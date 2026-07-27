# ??? System Validation Architecture & Mapping Blueprint Task 1.
# System Validation Architecture & Mapping Blueprint

## 1. Document Overview
* **Purpose:** Architecture mapping for web page data verification.
* **Environment:** Google AI Colab (20-07-2026 Batch Files 1–42).
* **Data Context:** Flat table row-by-row mapping to prevent data drift.

## 2. Execution Protocol
* **Processing Strategy:** The system must process all rows completely before generating a report.
* **Reporting Output:** Provide a single, comprehensive batch summary once the task finishes. Do not interrupt processing for real-time reporting.
* **Output Classification:** 
  * **Pass Log:** Fully validated rows meeting all criteria.
  * **Fail Log:** Flagged rows with specific error types and row numbers.

## 3. Data Schema & Architecture Mapping
To optimize token usage and processing speed, only the high-value columns listed below are within the active reading scope. All other columns (Columns C, D, F) must be ignored.

| Column A: Document Prefix | Column B: Local Authority | Column E: Holds Data | Column G: Allow OK Each Day | Column H: Other Ineligible Service |
| :--- | :--- | :--- | :--- | :--- |
| FOI-001 | [Authority Name] | [Binary Status] | [Operational Status] | [Exclusion/Exception Text] |
| FOI-002 | [Authority Name] | [Binary Status] | [Operational Status] | [Exclusion/Exception Text] |
| *... sequential entries ...* | *...* | *...* | *...* | *...* |
| FOI-292 | [Authority Name] | [Binary Status] | [Operational Status] | [Exclusion/Exception Text] |

## 4. Column Validation Rules
* **Column A (Document Prefix):** Must strictly follow the sequence from `FOI-001` down to `FOI-292`. Check for any missing numbers or duplicates.
* **Column B (Local Authority):** Must contain a valid, non-blank text string representing the target entity.
* **Column E (Holds Data):** Must contain a standardized binary value indicating data presence.
* **Column G (Allow OK Each Day):** Must contain valid operational permission status markers.
* **Column H (Other Ineligible Service):** Captures exclusion criteria. Must contain valid operational permission status markers.

#Please complete your task before your findings.
Batch Reporting After Completion is Better
•	Protects Memory: It keeps the workspace perfectly clean while the heavy processing occurs.
•	Pattern Recognition: The AI can scan all 292 rows first, allowing it to categorize errors by type (e.g., "5 rows have formatting issues, 2 rows are duplicates").
•	Actionable Output: You receive a neat, finalized audit report split cleanly into a Pass Log and a Fail Log with exact row numbers.
________________________________________

## 1. Operational Objectives: 
•	A deep audit of the facts, figures, formulas contained within the files (web pages) Draft Report Google AI Colab 20-07-2026 batch 1 - 42, compared against all of the other files that contain the master data.
•	If at any time, you experience Data Drift, please warn me.

The Cross-References:
•	The definitive data set is the table of Freedom of Information responses: Raw Excel Table Data Batch 1 to 16. This is the master data containing the baseline figures against which everything else will be assessed:  These files are a flat table or a tabular dataset.

•	Within the pages Raw Excel Table Data Batch page 1 - 16, the appropriate columns are:  A: Document Prefix FOI-001 down to FOI-292 ? Column B: Local Authority ? Column E: Holds Data ? Column G: Allow OK Each Day ? Column H: Other Ineligible Service. Other columns with data do not need to be read for todays task.

Validation Criteria for Raw Excel Table Data Batch 1 to 16
•	Column A (Document Prefix): These entry’s are in the order of the date on which the Freedom of Information request was made. The order that the data, eg. FOI-### can be ignored for this task. What matters is that for any given entry in Column A , the data in the other columns on the same row relates to the entry in Column A on the same row.
•	Column B (Local Authority): Must contain a valid text string representing the authority name. No blank cells allowed.
•	Column E (Holds Data): Should contain the text, either “YES”, “NO”, “N/A” or “VOID”. to indicate data presence. No blank cells allowed.
•	Column G (Allow OK Each Day): Should contain the text, either “YES”, “NO”, “N/A”, “AMBIGUOUS “ or “VOID”. to indicate data presence. No blank cells allowed.
•	Column H (Other Ineligible Service): Should contain the text, either “YES”, “NO”, “N/A “ or “VOID”. to indicate data presence. No blank cells allowed.

## 2. File-to-File Relational Matrix: 
•	2.1 Raw Excel Table Data Batch page 1 – 16:
?
•	2.2 Column A: Document Prefix FOI-001 down to FOI-292 ? Column B: Local Authority ? Column E: Holds Data ? Column G: Allow OK Each Day ? Column H: Other Ineligible Service
?
•	2.3 score System (Without understanding the scoring system, the data would seem arbitrary).	
?
•	2.4 Data Flow Charts Formulas and cell References
?
•	2.3 Data Flowchart 1 – 3 and Excel Configuration Blueprint

## 3. Step-by-Step Execution Sequence: A numbered list showing the exact order you want to open and verify the pages.
3.1 Validating the data within webpages: Data Flowcharts 1 – 3.
•	Read the pages: Raw Excel Table Data Batch 1 to 16:  Columns A, B, E, G and H: for records Document Prefix FOI-001 - FOI-292.
3.2 Read the page: Score System. 
•	Without understanding the logic of scoring system, the applied scores (YES, NO, N/A, AMBIGUOUS or VOID) would seem arbitrary and you would be unable to relate them to the other documents.
3.3 Read the page: Formulas and cell References
This is to understand the formulas and the cell references within which the formulas are placed inside the excel spreadsheet worksheets Data Flow Charts 1 – 3.
These are used to generate the figures in Data Flow Charts 1 – 3 and Excel Configuration Blueprint.
•	Check that the scores in Raw Excel Table Data Batch 1 to 16:  Columns A, B, E, G and H: for records Document Prefix FOI-001 - FOI-292, match the figures and data within Data Flow Charts 1 – 3.

•	Identify and report any anomalous figures in Data Flow Charts 1 – 3 and identify and report the formulas that may be cause.

3.5 Check your system and data matrix and identify if you are suffering from any Data Drift. Please report if you suspect that you are or that you can continue.

3.6 Read the page “Excel Configuration Blueprint” and check that the data values match those within in Data Flow Charts 1 – 3.
•	If any anomalous figures formulas or data had been found in Data Flow Charts 1 – 3, identify and report the entries in this webpage that mirror or relate to the anomaly’s so they may be corrected.
Report all findings in a single, structured summary.
END

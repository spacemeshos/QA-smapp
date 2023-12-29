# Test Scenario

#### Unique ID: ExportTx

**Description:** Verify the functionality of the "Export Transactions History" feature in Smapp, ensuring the user can export transaction data in various formats, apply filters, and have control over the export process.

**Priority:** 2

**Prerequisites:** User is logged into Smapp with existing transaction history.

**Test Cases:**

[01](#test-case-id-ExportTx-01) - Export transactions as CSV.

[02](#test-case-id-ExportTx-02) - Export transactions as XML.

[03](#test-case-id-ExportTx-03) - Export transactions as JSON.

[04](#test-case-id-ExportTx-04) - Export transactions as PDF.

[05](#test-case-id-ExportTx-05) - Cancel export process.

[06](#test-case-id-ExportTx-06) - Select correct directory and filename for export.

[07](#test-case-id-ExportTx-07) - Select correct directory and incorrect filename for export.

[08](#test-case-id-ExportTx-08) - Export with no transaction history.

[09](#test-case-id-ExportTx-09) - Validate exported data accuracy.

[10](#test-case-id-ExportTx-10) - Test exporting transaction history with a date range filter.

[11](#test-case-id-ExportTx-11) - Test exporting transaction history with a transaction type filter (e.g., incoming, outgoing, rewards).

[12](#test-case-id-ExportTx-12) - Test exporting transaction history when the network connection is lost.

[13](#test-case-id-ExportTx-13) - Test exporting a large volume of transaction data.

[14](#test-case-id-ExportTx-14) - Test the clarity and readability of the exported data.

---

# Test Cases

#### Test Case ID: ExportTx-01

**Description:** Export transactions as CSV.

**Steps:**

1. Open the Wallet screen in Smapp.
2. Click on the “All transactions” button.
3. Choose CSV as the export format.
4. Confirm the export.

**Test Data:** N/A

**Expected Result:** Transaction history is exported as a CSV file.

---

#### Test Case ID: ExportTx-02

**Description:** Export transactions as XML.

**Steps:**

1. Open the Wallet screen in Smapp.
2. Click on the “All transactions” button.
3. Choose XML as the export format.
4. Confirm the export.

**Test Data:** N/A

**Expected Result:** Transaction history is exported as an XML file.

---

#### Test Case ID: ExportTx-03

**Description:** Export transactions as JSON.

**Steps:**

1. Open the Wallet screen in Smapp.
2. Click on the “All transactions” button.
3. Choose JSON as the export format.
4. Confirm the export.

**Test Data:** N/A

**Expected Result:** Transaction history is exported as a JSON file.

---

#### Test Case ID: ExportTx-04

**Description:** Export transactions as PDF.

**Steps:**

1. Open the Wallet screen in Smapp.
2. Click on the “All transactions” button.
3. Choose PDF as the export format.
4. Confirm the export.

**Test Data:** N/A

**Expected Result:** Transaction history is exported as a PDF file.

---

#### Test Case ID: ExportTx-05

**Description:** Cancel export process.

**Steps:**

1. Open the Wallet screen in Smapp.
2. Click on the “All transactions” button.
3. Initiate the export process.
4. Click on the cancel button during the export.

**Test Data:** N/A

**Expected Result:** Export process is cancelled and no file is saved.

---

#### Test Case ID: ExportTx-06

**Description:** Select correct directory and filename for export.

**Steps:**

1. Open the Wallet screen in Smapp.
2. Click on the “All transactions” button.
3. Initiate the export process.
4. Choose a directory and enter a valid filename.
5. Confirm the export.

**Test Data:** Valid directory and filename

**Expected Result:** File is saved in the chosen directory with the specified filename.

---

#### Test Case ID: ExportTx-07

**Description:** Select correct directory and incorrect filename for export.

**Steps:**

1. Open the Wallet screen in Smapp.
2. Click on the “All transactions” button.
3. Initiate the export process.
4. Choose a directory and enter an invalid filename.
5. Confirm the export.

**Test Data:** Valid directory, invalid filename

**Expected Result:** Error message is displayed and no file is saved.

---

#### Test Case ID: ExportTx-08

**Description:** Export with no transaction history.

**Steps:**

1. Open the Wallet screen in Smapp with an account that has no transaction history.
2. Click on the “All transactions” button.
3. Initiate the export process.
4. Confirm the export.

**Test Data:** Account with no transaction history

**Expected Result:** Appropriate message indicating no data to export, or an empty file is exported.

---

#### Test Case ID: ExportTx-09

**Description:** Validate exported data accuracy.

**Steps:**

1. Open the Wallet screen in Smapp.
2. Click on the “All transactions” button.
3. Export the transaction history in any format.
4. Review the exported file for accuracy.

**Test Data:** N/A

**Expected Result:** The exported data matches the transaction history in Smapp accurately.

---

#### Test Case ID: ExportTx-10

**Description:** Test exporting transaction history with a date range filter.

**Steps:**

1. Open the Wallet screen in Smapp.
2. Click on the “All transactions” button.
3. Apply a date range filter.
4. Export the filtered transaction history in any format.
5. Confirm the export.

**Test Data:** Specific date range

**Expected Result:** Only transactions within the specified date range are exported.

---

#### Test Case ID: ExportTx-11

**Description:** Test exporting transaction history with a transaction type filter (e.g., incoming, outgoing, rewards).

**Steps:**

1. Open the Wallet screen in Smapp.
2. Click on the “All transactions” button.
3. Apply a transaction type filter.
4. Export the filtered transaction history in any format.
5. Confirm the export.

**Test Data:** Specific transaction types (incoming, outgoing, rewards)

**Expected Result:** Only transactions matching the selected types are exported.

---

#### Test Case ID: ExportTx-12

**Description:** Test exporting transaction history when the network connection is lost.

**Steps:**

1. Open the Wallet screen in Smapp
2. Click on the “All transactions” button.
3. Initiate the export process.
4. Disconnect the network during the export.
5. Observe the behavior of the application.

**Test Data:** N/A

**Expected Result:** An appropriate error message is displayed, and the export is not completed.

---

#### Test Case ID: ExportTx-13

**Description:** Test exporting a large volume of transaction data.

**Steps:**

1. Open the Wallet screen in Smapp with an account that has a large volume of transactions.
2. Click on the “All transactions” button.
3. Export the transaction history in any format.
4. Confirm the export.

**Test Data:** Account with a large volume of transactions

**Expected Result:** All transactions are exported correctly, without missing or corrupt data.

---

#### Test Case ID: ExportTx-14

**Description:** Test the clarity and readability of the exported data.

**Steps:**

1. Open the Wallet screen in Smapp.
2. Click on the “All transactions” button.
3. Export the transaction history in any format.
4. Open and review the exported file for clarity and readability.

**Test Data:** N/A

**Expected Result:** The exported data is clear, well-organized, and easily readable.

---


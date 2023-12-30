# Test Scenario

#### Unique ID: FilterTx

**Description:** Validate the functionality of the "Filter Transactions Log" feature in Smapp, ensuring the user can efficiently and accurately filter transaction history based on various criteria.

**Priority:** 3

**Prerequisites:** User is logged into Smapp with an existing transaction history.

**Test Cases:**

[01](#test-case-id-FilterTx-01) - Filter by transaction date.

[02](#test-case-id-FilterTx-02) - Filter by 'To' address (SMHs sent).

[03](#test-case-id-FilterTx-03) - Filter by 'From' address (SMHs received).

[04](#test-case-id-FilterTx-04) - Filter by note keywords.

[05](#test-case-id-FilterTx-05) - Filter by transaction amount.

[06](#test-case-id-FilterTx-06) - Filter by fees amount.

[07](#test-case-id-FilterTx-07) - Filter by status.

[08](#test-case-id-FilterTx-08) - Filter by transaction ID.

[09](#test-case-id-FilterTx-09) - Apply multiple filters simultaneously.

[10](#test-case-id-FilterTx-10) - Cancel filtering process.

[11](#test-case-id-FilterTx-11) - Filter with no matching transactions.

[12](#test-case-id-FilterTx-12) - Validate accuracy of filtered results.

[13](#test-case-id-FilterTx-13) - Filter by a combination of date and amount.

[14](#test-case-id-FilterTx-14) - Filter with invalid criteria.

[15](#test-case-id-FilterTx-15) - Responsive UI during filtering.

[16](#test-case-id-FilterTx-16) - Filter with partially matching criteria.

---

# Test Cases

#### Test Case ID: FilterTx-01

**Description:** Filter transaction history by transaction date.

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply a filter by selecting a specific transaction date or date range.
4. Observe the filtered results.

**Test Data:** Specific date or date range

**Expected Result:** Only transactions matching the selected date criteria are displayed.

---

#### Test Case ID: FilterTx-02

**Description:** Filter transaction history by 'To' address (SMHs sent).

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply a filter by entering a specific 'To' address.
4. Observe the filtered results.

**Test Data:** Specific 'To' address

**Expected Result:** Only transactions sent to the specified address are displayed.

---

#### Test Case ID: FilterTx-03

**Description:** Filter transaction history by 'From' address (SMHs received).

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply a filter by entering a specific 'From' address.
4. Observe the filtered results.

**Test Data:** Specific 'From' address

**Expected Result:** Only transactions received from the specified address are displayed.

---

#### Test Case ID: FilterTx-04

**Description:** Filter transaction history by note keywords.

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply a filter by entering keywords found in the transaction note.
4. Observe the filtered results.

**Test Data:** Specific keywords

**Expected Result:** Only transactions containing the specified keywords in their notes are displayed.

---

#### Test Case ID: FilterTx-05

**Description:** Filter transaction history by transaction amount.

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply a filter by specifying a transaction amount or amount range.
4. Observe the filtered results.

**Test Data:** Specific amount or amount range

**Expected Result:** Only transactions matching the specified amount criteria are displayed.

---

#### Test Case ID: FilterTx-06

**Description:** Filter transaction history by fees amount.

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply a filter by specifying a fee amount or fee amount range.
4. Observe the filtered results.

**Test Data:** Specific fee amount or range

**Expected Result:** Only transactions with the specified fees amount are displayed.

---

#### Test Case ID: FilterTx-07

**Description:** Filter transaction history by status (e.g., pending, confirmed).

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply a filter by selecting a specific transaction status.
4. Observe the filtered results.

**Test Data:** Specific transaction status

**Expected Result:** Only transactions with the specified status are displayed.

---

#### Test Case ID: FilterTx-08

**Description:** Filter transaction history by transaction ID.

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply a filter by entering a specific transaction ID.
4. Observe the filtered results.

**Test Data:** Specific transaction ID

**Expected Result:** The transaction with the specified ID is displayed.

---

#### Test Case ID: FilterTx-09

**Description:** Apply multiple filters simultaneously to transaction history.

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply multiple filters (e.g., date range, transaction amount, status).
4. Observe the filtered results.

**Test Data:** Combination of different filter criteria

**Expected Result:** Only transactions matching all applied filter criteria are displayed.

---

#### Test Case ID: FilterTx-10

**Description:** Cancel the filtering process at any moment.

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Start applying filters.
4. Cancel the filtering process before applying.

**Test Data:** N/A

**Expected Result:** The filter process is cancelled, and no changes are made to the transaction log display.

---


#### Test Case ID: FilterTx-11

**Description:** Filter with no matching transactions.

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply filter criteria that do not match any transaction in the history.
4. Observe the results.

**Test Data:** Filter criteria with no matching transactions

**Expected Result:** A message indicating no transactions match the filter criteria or an empty result set is displayed.

---

#### Test Case ID: FilterTx-12

**Description:** Validate accuracy of filtered results.

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply known filter criteria with expected results.
4. Compare the filtered results to the expected outcome.

**Test Data:** Known filter criteria with expected matching transactions

**Expected Result:** Filtered results accurately match the expected transactions.

---

#### Test Case ID: FilterTx-13

**Description:** Filter by a combination of date and amount.

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply a filter with a specific date range and transaction amount range.
4. Observe the filtered results.

**Test Data:** Specific date and amount ranges

**Expected Result:** Only transactions matching both the date and amount criteria are displayed.

---

#### Test Case ID: FilterTx-14

**Description:** Filter with invalid criteria.

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply filters with invalid criteria (e.g., future dates, nonsensical amounts).
4. Observe the behavior of the application.

**Test Data:** Invalid filter criteria

**Expected Result:** An error message is displayed, or the filter is not applied.

---

#### Test Case ID: FilterTx-15

**Description:** Responsive UI during filtering.

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply various filters.
4. Observe the responsiveness and performance of the UI during the filtering process.

**Test Data:** N/A

**Expected Result:** The UI remains responsive and functional during the filtering process without lag or crashes.

---

#### Test Case ID: FilterTx-16

**Description:** Filter with partially matching criteria.

**Steps:**

1. Open the Wallet screen.
2. Click on the “All transactions” button.
3. Apply filter criteria that partially match the transactions (e.g., correct date but incorrect amount).
4. Observe the results.

**Test Data:** Partially matching filter criteria

**Expected Result:** Transactions that fully match the criteria are displayed; partial matches are not shown.

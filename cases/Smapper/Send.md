# Test Scenario

#### Unique ID:  Send

**Description:** Testing the "Send" transaction functionality.

**Priority:** 1

**Prerequisites:** Smapp is installed and running. The wallet is synced and has a positive balance, higher than the tx costs sum.

**Test Cases:** 


[01](#test-case-id-Send-01) - Validate the "Send" button functionality  

[02](#test-case-id-Send-02) - Validate the "To" field with correct and existing account addresses  

[03](#test-case-id-Send-03) - Validate the "To" field with invalid or non-existing account addresses  

[04](#test-case-id-Send-04) - Validate the auto-population of the "From" field  

[05](#test-case-id-Send-05) - Validate the "Amount" field accepts only numerical input  

[06](#test-case-id-Send-06) - Validate the "Amount" field for amounts greater than current balance  

[07](#test-case-id-Send-07) - Validate switching between Smesh and Smidges  

[08](#test-case-id-Send-08) - Validate the "Cost" field dropdown  

[09](#test-case-id-Send-09) - Validate effect of different "Cost" on transaction speed  

[10](#test-case-id-Send-10) - Validate the "Note" field accepts text input  

[11](#test-case-id-Send-11) - Validate that the "Note" field is optional  

[12](#test-case-id-Send-12) - Validate clicking "Next" leads to the summary screen  

[13](#test-case-id-Send-13) - Validate the summary screen shows correct transaction details  

[14](#test-case-id-Send-14) - Validate clicking "Send" results in a confirmation message  

[15](#test-case-id-Send-15) - Validate the "View transaction" button functionality  

[16](#test-case-id-Send-16) - Validate the "Done" button functionality  

[17](#test-case-id-Send-17) - Validate executed transaction appears in Transactions log  

[18](#test-case-id-Send-18) - Validate "Cost" affects time for transaction to be applied  

[19](#test-case-id-Send-19) - Validate wallet balance is updated correctly  

[20](#test-case-id-Send-20) - Validate the "Note" in transaction details in Transactions log  

[21](#test-case-id-Send-21) - Validate error handling for network issues  

[22](#test-case-id-Send-22) - Validate transaction fees are calculated correctly  

[23](#test-case-id-Send-23) - Validate security during transaction  

[24](#test-case-id-Send-24) - Validate transactions are auditable and correctly logged  

[25](#test-case-id-Send-25) - Validate UI/UX during transaction process  

[26](#test-case-id-Send-26) - Validate resource utilization during transaction  

[27](#test-case-id-Send-27) - Validate behavior when app is minimized during transaction  

[28](#test-case-id-Send-28) - Validate transactions (correct) visibility accross different app versions.

[29](#test-case-id-send-29) - Validate the "Cancel" button during the transaction process

_____

# Test Cases

#### Test Case ID: Send-01

**Description:** Validate the "Send" button functionality

**Steps:**

1. Open the Wallet screen in Smapp.
2. Click on the "Send" button.

**Test Data:** N/A

**Expected Result:** The Transaction screen should open.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-02

**Description:** Validate the "To" field with correct and existing account addresses

**Steps:**

1. Open the Transaction screen.
2. Enter a correct and existing account address in the "To" field.

**Test Data:** Valid account address

**Expected Result:** The "To" field should accept the address without errors.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-03

**Description:** Validate the "To" field with invalid or non-existing account addresses

**Steps:**

1. Open the Transaction screen.
2. Enter an invalid or non-existing account address in the "To" field.

**Test Data:** Invalid or non-existing account address

**Expected Result:** The "To" field should display an error message.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-04

**Description:** Validate the auto-population of the "From" field

**Steps:**

1. Open the Transaction screen.

**Test Data:** N/A

**Expected Result:** The "From" field should automatically populate with the sender's account address.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-05

**Description:** Validate the "Amount" field accepts only numerical input

**Steps:**

1. Open the Transaction screen.
2. Enter a value in the "Amount" field using alphabets, symbols, or special characters.

**Test Data:** Alphabets, symbols, special characters

**Expected Result:** The "Amount" field should not accept any non-numerical input and should display an error message or prevent submission.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-06

**Description:** Validate the "Amount" field for amounts greater than current balance

**Steps:**

1. Open the Transaction screen.
2. Enter an amount greater than the current balance in the "Amount" field.

**Test Data:** Amount greater than current balance

**Expected Result:** The field should display an error message indicating insufficient funds.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-07

**Description:** Validate switching between Smesh and Smidges

**Steps:**

1. Open the Transaction screen.
2. Locate the "Amount" field and the unit switch button.
3. Switch between Smesh and Smidges.

**Test Data:** N/A

**Expected Result:** The unit should switch and the equivalent value should display correctly.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-08

**Description:** Validate the "Cost" field dropdown

**Steps:**

1. Open the Transaction screen.
2. Click the "Cost" dropdown field.

**Test Data:** N/A

**Expected Result:** The dropdown should display three different options for transaction fees.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-09

**Description:** Validate the effect of different "Cost" on transaction speed

**Steps:**

1. Open the Transaction screen.
2. Complete a transaction with the lowest "Cost" setting.
3. Complete another transaction with the highest "Cost" setting.

**Test Data:** N/A

**Expected Result:** The transaction with the highest "Cost" setting should complete faster than the one with the lowest "Cost" setting.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-10

**Description:** Validate the "Note" field accepts text input

**Steps:**

1. Open the Transaction screen.
2. Type text into the "Note" field.

**Test Data:** Any text string

**Expected Result:** The "Note" field should accept the text without errors and the note should be visible in the transaction details in the log.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-11

**Description:** Validate that the "Note" field is optional

**Steps:**

1. Open the Transaction screen.
2. Leave the "Note" field empty.
3. Complete the transaction.

**Test Data:** N/A

**Expected Result:** The transaction should complete successfully without requiring a note.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-12

**Description:** Validate clicking "Next" leads to the summary screen

**Steps:**

1. Open the Transaction screen.
2. Fill in all required fields.
3. Click "Next."

**Test Data:** N/A

**Expected Result:** The summary screen should display, showing details of the impending transaction.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-13

**Description:** Validate the summary screen shows correct transaction details

**Steps:**

1. Navigate to the summary screen.
2. Verify the details displayed.

**Test Data:** N/A

**Expected Result:** All details should match what was entered in the previous screen.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-14

**Description:** Validate clicking "Send" results in a confirmation message

**Steps:**

1. On the summary screen, click "Send."

**Test Data:** N/A

**Expected Result:** A confirmation message should appear, indicating the transaction has been submitted.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-15

**Description:** Validate the "View transaction" button functionality

**Steps:**

1. Click on the "View transaction" button on the confirmation screen.

**Test Data:** N/A

**Expected Result:** The Transactions log should open, highlighting the recent transaction.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-16

**Description:** Validate the "Done" button functionality

**Steps:**

1. Click on the "Done" button on the confirmation screen.

**Test Data:** N/A

**Expected Result:** The Transaction screen should close, and you should return to the main Wallet page.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-17

**Description:** Validate executed transaction appears in Transactions log

**Steps:**

1. Complete a transaction.
2. Open the Transactions log.

**Test Data:** N/A

**Expected Result:** The recent transaction should appear in the Transactions log.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-18

**Description:** Validate "Cost" affects time for transaction to be applied

**Steps:**

1. Complete a transaction with a low "Cost" setting.
2. Complete another transaction with a high "Cost" setting.
3. Observe the time it takes for each to be applied.

**Test Data:** N/A

**Expected Result:** The transaction with the higher "Cost" setting should be applied more quickly than the one with the lower setting.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-19

**Description:** Validate wallet balance is updated correctly

**Steps:**

1. Complete a transaction.
2. Return to the Wallet screen.

**Test Data:** N/A

**Expected Result:** The Wallet balance should be updated correctly, reflecting the recent transaction.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-20

**Description:** Validate the "Note" in transaction details in Transactions log

**Steps:**

1. Complete a transaction with a note.
2. View the transaction in the Transactions log.

**Test Data:** Any text string for the "Note"

**Expected Result:** The note should appear in the details of the transaction within the Transactions log.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-21

**Description:** Validate error handling for network issues

**Steps:**

1. Disable network connectivity.
2. Attempt to complete a transaction.

**Test Data:** N/A

**Expected Result:** An appropriate error message should be displayed, informing the user that the network is unavailable.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-22

**Description:** Validate transaction fees are calculated correctly

**Steps:**

1. Start a transaction.
2. Choose different options for "Cost."
3. Validate the calculated transaction fees.

**Test Data:** N/A

**Expected Result:** The transaction fees should be calculated correctly based on the chosen "Cost."

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-23

**Description:** Validate security during transaction

**Steps:**

1. Complete a transaction.
2. Validate that all sensitive data is encrypted and not exposed in logs or UI.

**Test Data:** N/A

**Expected Result:** Sensitive data should be securely handled and not exposed at any point.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-24

**Description:** Validate transactions are auditable and correctly logged

**Steps:**

1. Complete multiple transactions.
2. Validate that each transaction is correctly logged for auditing purposes.

**Test Data:** N/A

**Expected Result:** All transactions should be traceable and correctly logged.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-25

**Description:** Validate UI/UX during transaction process

**Steps:**

1. Complete a transaction.
2. Observe the user interface and experience.

**Test Data:** N/A

**Expected Result:** The UI should be intuitive, and the steps should be clearly communicated to the user.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-26

**Description:** Validate resource utilization during transaction

**Steps:**

1. Monitor CPU, memory, and network usage while completing a transaction.

**Test Data:** N/A

**Expected Result:** Resource utilization should remain within acceptable limits.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-27

**Description:** Validate behavior when the app is minimized during transaction

**Steps:**

1. Start a transaction.
2. Minimize the app during the transaction process.

**Test Data:** N/A

**Expected Result:** The transaction should either pause or continue in the background, based on the designed behavior.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-28

**Description:** Validate transactions (correct) visibility accross different app versions.

**Steps:**

1. Complete a transaction using an older version of the app.
2. Validate that the transaction is visible in the tx log with in the newest app version.

**Test Data:** N/A

**Expected Result:** Transactions should be saved and reflected across different versions of the app.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Send-28

**Description:** Validate the "Cancel" button during the transaction process

**Steps:**

1. Start a transaction.
2. Click on the "Cancel" button at any point before confirming the transaction.

**Test Data:** N/A

**Expected Result:** The transaction should be cancelled and you should return to the Wallet screen without any changes being applied.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]


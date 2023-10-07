# Test Scenario

#### Unique ID: 

**Description:** short info about the topic 

**Priority:** 1 (highest) - 3 (lowest)

**Prerequisites:** anything that needs to be in place before running the tests - so that the result may be considered as valid

**Test Cases:** 

[]() - Verify Successful Wallet Recovery Using 12 Words Backup.

[]() - Verify Error Handling - Invalid 12 Words.

[]() - Verify Error Handling - Empty 12 Words.

[]() - Verify Error Handling - Case Insensitivity.

[]() - Verify Error Handling - Leading/Trailing Whitespace.

[]() - Verify Backup Validation - Incorrect Words.

[]() - Verify Backup Recovery with Different Word Order.

[]() - Verify Error Handling - Missing Words.




#### Test Case ID: 01

**Description:** Verify Successful Wallet Recovery Using 12 Words Backup.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet" option.
3. User enters the 12-word backup.
4. User confirms the recovery process.

**Test Data:** Valid 12-word backup.

**Expected Result:** The wallet should be successfully recovered using the 12-word backup.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---
#### Test Case ID: 02

**Description:** Verify Error Handling - Invalid 12 Words.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet" option.
3. User enters an invalid set of 12 words.
4. User confirms the recovery process.

**Test Data:** Invalid 12-word backup.

**Expected Result:** An error message should indicate that the 12-word backup is invalid, and the recovery process should fail.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---
#### Test Case ID: 03

**Description:** Verify Error Handling - Empty 12 Words.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet" option.
3. User attempts to proceed with an empty 12-word input.

**Test Data:** Empty 12-word backup.

**Expected Result:** An error message should indicate that the 12-word backup cannot be empty, and the recovery process should fail.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---
#### Test Case ID: 04

**Description:** Verify Error Handling - Case Insensitivity.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet" option.
3. User enters words with varying cases in the 12-word backup.
4. User confirms the recovery process.

**Test Data:** 12-word backup with mixed cases.

**Expected Result:** The recovery process should be case-insensitive and successful.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---
#### Test Case ID: 05

**Description:** Verify Error Handling - Leading/Trailing Whitespace.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet" option.
3. User enters words with leading/trailing whitespace in the 12-word backup.
4. User confirms the recovery process.

**Test Data:** 12-word backup with leading/trailing whitespace.

**Expected Result:** The recovery process should handle whitespace gracefully and be successful.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---
#### Test Case ID: 06

**Description:** Verify Backup Validation - Incorrect Words.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet" option.
3. User enters a set of 12 words, including some incorrect ones.
4. User confirms the recovery process.

**Test Data:** 12-word backup with some incorrect words.

**Expected Result:** The recovery process should fail with an error message if any of the words are incorrect.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---
#### Test Case ID: 07

**Description:** Verify Backup Recovery with Different Word Order.

**Steps:**

1. User creates a valid 12-word backup.
2. User enters the words in a different order during recovery.
3. User confirms the recovery process.

**Test Data:** Valid 12-word backup with a different word order.

**Expected Result:** The recovery process should successfully recover the wallet even with a different word order.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---
#### Test Case ID: 08

**Description:** Verify Error Handling - Missing Words.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Recover Wallet" option.
3. User enters a subset of the 12 words, leaving some out.
4. User confirms the recovery process.

**Test Data:** Incomplete 12-word backup.

**Expected Result:** An error message should indicate that all 12 words are required, and the recovery process should fail.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---
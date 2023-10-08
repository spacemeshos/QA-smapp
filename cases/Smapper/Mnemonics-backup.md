# Test Scenario

#### Unique ID: Mnemonics-backup

**Description:** Creating a Wallet backup using the 12 / 24 words method.

**Priority:** 2

**Prerequisites:** running Smapp, 

**Test Cases:** 

[1](#test-case-id-01) - Verify Successful Backup Creation

[2](#test-case-id-02) - Verify Backup Words Count

[3](#test-case-id-03) - Verify Word Validity

[4](#test-case-id-04) - Verify Word Uniqueness

[5](#test-case-id-05) - Verify Word Order Randomization

[6](#test-case-id-06) - Verify Backup Security

[7](#test-case-id-07) - Verify Backup Recovery

[8](#test-case-id-08) - Verify Error Handling - No Backup Created

[9](#test-case-id-09) - Verify Error Handling - Insufficient Words

[10](#test-case-id-10) - Verify Backup Validation - Incorrect Words

[11](#test-case-id-11) - Verify Backup Export/Import

[12](#test-case-id-12) - Verify Backup Recovery - Case Insensitivity

[13](#test-case-id-13) - Verify Backup Recovery - Leading/Trailing Whitespace


_____


#### Test Case ID: 01

**Description:** Verify Successful Backup Creation.

**Steps:**

1. User opens the Spacemesh application.
2. User selects the "Create 12 Words Backup" option.

**Test Data:** None

**Expected Result:** A backup containing 12 words is generated successfully.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: 02

**Description:** Verify Backup Words Count.

**Steps:**

1. User creates a backup.

**Test Data:** None

**Expected Result:** There should be exactly 12 words in the backup.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: 03

**Description:** Verify Word Validity.

**Steps:**

1. User creates a backup.

**Test Data:** None

**Expected Result:** All words should be valid and recognized in the English language.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: 04

**Description:** Verify Word Uniqueness.

**Steps:**

1. User creates multiple backups.

**Test Data:** None

**Expected Result:** No two backups should have the same set of 12 words.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: 05

**Description:** Verify Word Order Randomization.

**Steps:**

1. User creates multiple backups.

**Test Data:** None

**Expected Result:** The order of words should be randomized for each backup.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: 06

**Description:** Verify Backup Security.

**Steps:**

1. User creates a backup.

**Test Data:** None

**Expected Result:** The backup is stored securely and not accessible to unauthorized parties.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: 07

**Description:** Verify Backup Recovery.

**Steps:**

1. User creates a backup and saves it securely.
2. User attempts to recover the wallet using the backup.

**Test Data:** None

**Expected Result:** The wallet should be successfully recovered using the 12-word backup.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: 08

**Description:** Verify Error Handling - No Backup Created.

**Steps:**

1. User cancels the backup creation process.
2. User checks if any backup is created.

**Test Data:** None

**Expected Result:** No backup should be generated if the user cancels the process.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: 09

**Description:** Verify Error Handling - Insufficient Words.

**Steps:**

1. User attempts to create a backup with less than 12 words.
2. User submits the incomplete backup.

**Test Data:** None

**Expected Result:** An error message should indicate that at least 12 words are required.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: 10

**Description:** Verify Backup Validation - Incorrect Words.

**Steps:**

1. User enters incorrect words during the backup recovery process.
2. User attempts to recover the wallet.

**Test Data:** None

**Expected Result:** The recovery process should fail with an error message.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: 11

**Description:** Verify Backup Export/Import.

**Steps:**

1. User creates a backup and exports it to a file.
2. User imports the backup from the file.

**Test Data:** None

**Expected Result:** The imported backup should successfully recover the wallet.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: 12

**Description:** Verify Backup Recovery - Case Insensitivity.

**Steps:**

1. User attempts to recover the wallet with a mix of uppercase and lowercase words.
2. User enters words with varying cases.

**Test Data:** None

**Expected Result:** The recovery process should be case-insensitive and successful.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: 13

**Description:** Verify Backup Recovery - Leading/Trailing Whitespace.

**Steps:**

1. User attempts to recover the wallet with words containing leading/trailing whitespace.
2. User enters words with extra spaces.

**Test Data:** None

**Expected Result:** The recovery process should handle whitespace gracefully and be successful.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

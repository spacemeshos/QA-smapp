# Test Scenario

#### Unique ID: Create12WordsBackup

**Description:** Testing the 12 words backup option for wallet backup in the settings, Wallets section.

**Priority:** 1

**Prerequisites:** 
- User should have the Smapp application installed
- User should have an active wallet

**Test Cases:**

[01](#test-case-id-create-12-words-backup-01) - Canceling the backup operation

[02](#test-case-id-create-12-words-backup-02) - Incorrectly placing 4 words for confirmation

[03](#test-case-id-create-12-words-backup-03) - Successfully completing the 12 words backup

[04](#test-case-id-create-12-words-backup-04) - Proceeding without saving words

[05](#test-case-id-create-12-words-backup-05) - UI and layout validation

[06](#test-case-id-create-12-words-backup-06) - Application close or crash during backup

[07](#test-case-id-create-12-words-backup-07) - Correctness of 12 words

[08](#test-case-id-create-12-words-backup-08) - Uniqueness of the mnemonics

_____

# Test Cases

#### Test Case ID: Create12WordsBackup-01

**Description:** Canceling the backup operation

**Steps:**
1. Navigate to Settings, then to the "Wallets" section
2. Click the "Backup Now" button
3. Choose "12 Words Backup" option
4. Click "Cancel" at any point before final confirmation

**Test Data:** N/A

**Expected Result:** 
- The operation should be canceled
- User should be taken back to the Wallets section in Settings



---

#### Test Case ID: Create12WordsBackup-02

**Description:** Incorrectly placing 4 words for confirmation

**Steps:**
1. Open the Settings screen and go to the Wallets section.
2. Click on the “Backup Now” button.
3. See a screen containing 2 buttons: “File Backup” and “12 Words Backup”.
4. Click on the “12 Words Backup” button.
5. See the “Your 12 Words Backup” screen displaying my backup words with two buttons to save them: “Print Words” and “Copy Words”.
6. Choose the most convenient option to keep the words, and click on the “Next” button.
7. On the next screen, “Confirm Your 12 Words Backup”, drag and drop 4 randomly displayed words to the incorrect places.
2. Observe the message displayed

**Test Data:** Incorrectly placed 4 words

**Expected Result:** 
- A red message "That confirmation isn’t correct, please try again." should be displayed
- The option to "Try Again" should be available
- The message should be easily readable and noticeable



---

#### Test Case ID: Create12WordsBackup-03

**Description:** Successfully completing the 12 words backup

**Steps:**
1. Follow steps 1-6 from the previous case description
2. Place the 4 words correctly for confirmation
3. Click "Done"

**Test Data:** Correctly placed 4 words

**Expected Result:** 
- A green message saying "All right! Your 12 word backup is confirmed." should be displayed
- The message should be easily readable and noticeable
- User should be automatically moved back to the Wallet screen
- A backup should be succesfully created



---

#### Test Case ID: Create12WordsBackup-04

**Description:** Proceeding without saving words

**Steps:**
1. Follow steps 1-4 from the scenario description
2. Click "Next" without using the "Copy Words" or "Print Words" buttons.

**Test Data:** N/A

**Expected Result:** 
- User should be able to proceed to the next step with no restraints. 



---

#### Test Case ID: Create12WordsBackup-05

**Description:** UI and layout validation

**Steps:**
1. Follow sall the possible steps of the mnemonics backup creation
2. Verify all UI elements are appropriately rendered and functioning

**Test Data:** N/A

**Expected Result:** 
- All buttons, text fields, and messages should be visible and appropriately rendered



---

#### Test Case ID: Create12WordsBackup-06

**Description:** Application close or crash during backup

**Steps:**
1. Follow steps 1-5 or 6 from the test case [02](#test-case-id-create-12-words-backup-02)
2. Close the application or simulate a crash

**Test Data:** N/A

**Expected Result:** 
- The backup process should not be partially saved, requiring the user to start over
- The set of the backup words should be the same, with the same order



---

#### Test Case ID: Create12WordsBackup-07

**Description:** Correctness of 12 words

**Steps:**
1. Complete all the steps of 12 words backup process
2. Save the backup words 
3. Start the process again for the same wallet
4. Compare the sets of words

**Test Data:** N/A

**Expected Result:** 
- The 12 words should always be the same for a given wallet
- The order of the words should not change



---

#### Test Case ID: Create12WordsBackup-08

**Description:** Uniqueness of 12 words

**Steps:**
1. Complete all the steps of 12 words backup process
2. Save the backup words 
3. Start the process again for a couple of other wallets
4. Compare the sets of words

**Test Data:** N/A

**Expected Result:** 
- The 12 words should never be the same for more than 1 wallet




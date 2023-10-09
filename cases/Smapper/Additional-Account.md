# Test Scenario

#### Unique ID: AdditionalAccountCreation

**Description:** Testing the additional account creation functionality in the settings, Accounts section.

**Priority:** 3

**Prerequisites:** 
- User should have the Smapp application installed
- User should have a main account with a set password
- User should be in the settings screen, Accounts section

**Test Cases:**
- [01](#test-case-id-additional-account-creation-01) - User cancels the operation
- [02](#test-case-id-additional-account-creation-02) - Incorrect password in the confirmation step
- [03](#test-case-id-additional-account-creation-03) - Successful additional account creation

_____

# Test Cases

#### Test Case ID: AdditionalAccountCreation-01

**Description:** User cancels the operation

**Steps:**
1. Navigate to settings, then to the "Accounts" section
2. Click the "Add Account" button
3. In the pop-up window, click "Cancel"

**Test Data:** N/A

**Expected Result:** 
- Pop-up window should close
- No new account should be created

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: AdditionalAccountCreation-02

**Description:** Incorrect password in the confirmation step

**Steps:**
1. Navigate to settings, then to the "Accounts" section
2. Click the "Add Account" button
3. In the pop-up window, input an incorrect password
4. Click "Confirm"

**Test Data:** 
- Password: "wrongpassword"

**Expected Result:** 
- User should not be able to proceed
- An error message should be displayed indicating the password is incorrect

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: AdditionalAccountCreation-03

**Description:** Successful additional account creation

**Steps:**
1. Navigate to settings, then to the "Accounts" section
2. Click the "Add Account" button
3. In the pop-up window, input the correct main account password
4. Click "Confirm"

**Test Data:** 
- Password: "correctpassword"

**Expected Result:** 
- The settings screen should return to the initial layout
- A new account should be visible below the main account in the Accounts section
- The new account should be selectable in the drop-down list on the left side of the Wallet screen

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

# Test Scenario

#### Unique ID: Password

**Description:** Testing the password setup during wallet creation

**Priority:** 1

**Prerequisites:** 
- User should have the Smapp application installed
- User should be at the wallet creation screen

**Test Cases:**

[01](#test-case-id-password-01) - Both password fields are empty

[02](#test-case-id-password-02) - First password field is empty

[03](#test-case-id-password-03) - Second password field is empty

[04](#test-case-id-password-04) - Both passwords match

[05](#test-case-id-password-05) - Both passwords do not match

_____

# Test Cases

#### Test Case ID: Password-01

**Description:** Both password fields are empty

**Steps:**
1. Open the Smapp application
2. Navigate to the wallet creation screen
3. Leave both password fields empty
4. Try to proceed

**Test Data:** N/A

**Expected Result:** 
- User should not be able to proceed
- An error message should be displayed indicating both fields cannot be empty



---

#### Test Case ID: Password-02

**Description:** First password field is empty

**Steps:**
1. Open the Smapp application
2. Navigate to the wallet creation screen
3. Leave the first password field empty, but fill the second one
4. Try to proceed

**Test Data:** Second password field: "password123"

**Expected Result:** 
- User should not be able to proceed
- An error message should be displayed indicating the first password field cannot be empty



---

#### Test Case ID: Password-03

**Description:** Second password field is empty

**Steps:**
1. Open the Smapp application
2. Navigate to the wallet creation screen
3. Leave the second password field empty, but fill the first one
4. Try to proceed

**Test Data:** First password field: "password123"

**Expected Result:** 
- User should not be able to proceed
- An error message should be displayed indicating the second password field cannot be empty



---

#### Test Case ID: Password-04

**Description:** Both passwords match

**Steps:**
1. Open the Smapp application
2. Navigate to the wallet creation screen
3. Fill both password fields with the same value
4. Try to proceed

**Test Data:** 
- First password field: "password123"
- Second password field: "password123"

**Expected Result:** 
- User should be able to proceed to the next step of the wallet creation process



---

#### Test Case ID: Password-05

**Description:** Both passwords do not match

**Steps:**
1. Open the Smapp application
2. Navigate to the wallet creation screen
3. Fill both password fields with different values
4. Try to proceed

**Test Data:** 
- First password field: "password123"
- Second password field: "password321"

**Expected Result:** 
- User should not be able to proceed
- An error message should be displayed indicating that the passwords do not match



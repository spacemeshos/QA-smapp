# Test Scenario

#### Unique ID: ChangePassword

**Description:** Testing the change password functionality in the settings screen

**Priority:** 2

**Prerequisites:** 
- User should have the Smapp application installed
- User should have an existing wallet logged in
- User should be at the settings screen (wallet section)

**Test Cases:**
- [01](#test-case-id-changepassword-01) - All fields are empty
- [02](#test-case-id-changepassword-02) - Current password is incorrect
- [03](#test-case-id-changepassword-03) - New password and verify password fields do not match
- [04](#test-case-id-changepassword-04) - Correct current password, matching new and verify password fields
- [05](#test-case-id-changepassword-05) - Using 'Cancel' button

_____

# Test Cases

#### Test Case ID: ChangePassword-01

**Description:** All fields are empty

**Steps:**
1. Open the Smapp application
2. Navigate to the settings screen
3. Click the "Change Password" button
4. Leave all fields empty
5. Click "Save"

**Test Data:** N/A

**Expected Result:** 
- User should not be able to proceed
- An error message should be displayed indicating that fields cannot be empty



---

#### Test Case ID: ChangePassword-02

**Description:** Current password is incorrect

**Steps:**
1. Open the Smapp application
2. Navigate to the settings screen
3. Click the "Change Password" button
4. Input an incorrect value in the "Current Password" field
5. Fill the "Type New Password" and "Verify Password" fields
6. Click "Save"

**Test Data:** 
- Current Password: "wrongpassword"
- Type New Password: "newpassword123"
- Verify Password: "newpassword123"

**Expected Result:** 
- User should not be able to proceed
- An error message should be displayed indicating that the current password is incorrect



---

#### Test Case ID: ChangePassword-03

**Description:** New password and verify password fields do not match

**Steps:**
1. Open the Smapp application
2. Navigate to the settings screen
3. Click the "Change Password" button
4. Input the correct current password
5. Fill the "Type New Password" and "Verify Password" fields with different values
6. Click "Save"

**Test Data:** 
- Current Password: "currentpassword123"
- Type New Password: "newpassword123"
- Verify Password: "newpassword321"

**Expected Result:** 
- User should not be able to proceed
- An error message should be displayed indicating that the new password and verify password do not match



---

#### Test Case ID: ChangePassword-04

**Description:** Correct current password, matching new and verify password fields

**Steps:**
1. Open the Smapp application
2. Navigate to the settings screen
3. Click the "Change Password" button
4. Input the correct current password
5. Fill the "Type New Password" and "Verify Password" fields with matching values
6. Click "Save"

**Test Data:** 
- Current Password: "currentpassword123"
- Type New Password: "newpassword123"
- Verify Password: "newpassword123"

**Expected Result:** 
- User should be able to proceed
- Password should be successfully changed



---

#### Test Case ID: ChangePassword-05

**Description:** Using 'Cancel' button

**Steps:**
1. Open the Smapp application
2. Navigate to the settings screen
3. Click the "Change Password" button
4. Fill any values in the fields
5. Click "Cancel"

**Test Data:** 
- Current Password: "currentpassword123"
- Type New Password: "newpassword123"
- Verify Password: "newpassword123"

**Expected Result:** 
- User should be able to cancel the operation
- No changes should be made to the password




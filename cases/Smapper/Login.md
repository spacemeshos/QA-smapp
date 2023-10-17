# Test Scenario

#### Unique ID:  Login

**Description:** Testing the login functionality of Smapp

**Priority:** 1 

**Prerequisites:** Smapp should be installed, and at least one wallet should be available for testing.

**Test Cases:** 

[01](#test-case-id-login-01) - Valid Credentials: Verify that users can successfully log in with a valid password.

[02](#test-case-id-login-02) - Invalid Credentials - Password: Test the system's response when a user enters an invalid password.

[03](#test-case-id-login-03) - Empty Fields: Ensure the system handles cases where the password field is left empty.

[04](#test-case-id-login-04) - Password Case Sensitivity: Confirm that the password field is case-sensitive.

[05](#test-case-id-login-05) - Password Masking: Verify that the password is masked (hidden) as the user types it.

[06](#test-case-id-login-06) - Network Interruption: Simulate network interruptions during the login process to ensure graceful handling of such situations.

[07](#test-case-id-login-07) - Cross-platform Compatibility: Check if the login module works seamlessly on various desktop operating systems (e.g., Windows, macOS, Linux).

[08](#test-case-id-login-08) - Localization: Verify that the login module works correctly with different languages and character sets.

[09](#test-case-id-login-09) - Error Messages: Confirm that error messages are clear and informative for users encountering login issues.

[10](#test-case-id-login-10) - Logging: Ensure that login attempts and related activities are correctly logged for security and auditing purposes.

[11](#test-case-id-login-11) - Verify the behavior of pressing the "Enter" key in the password field.

_____


# Test Cases

#### Test Case ID: Login-01

**Description:** Valid Credentials: Verify that users can successfully log in with valid password.

**Steps:**

1. Open Smapp.

2. If the Wallet file already exists, the login page should open right after launching Smapp.

4. Enter a valid password.

5. Click the "Log In" button.

**Test Data:**

- Valid password: [take from test data]

**Expected Result:** The user should be logged in and directed to their wallet.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Login-02

**Description:** Test the system's response when a user enters an invalid password.

**Steps:**

1. Launch Smapp.
2. Enter an invalid password for the suggested wallet.
3. Click on "Submit" or hit "Enter".

**Test Data:** Invalid password for the suggested wallet.

**Expected Result:** An error message in red should appear saying, “Sorry, this password doesn't ring a bell; please try again.”

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Login-03

**Description:** Ensure the system handles cases where the password field is left empty.

**Steps:**

1. Launch Smapp.
2. Leave the password field empty.
3. Click on "Submit" or hit "Enter".

**Test Data:** Empty password field.

**Expected Result:** The "Submit" button should be disabled or an error message should appear, indicating that the password field cannot be empty.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Login-04

**Description:** Confirm that the password field is case-sensitive.

**Steps:**

1. Launch Smapp.
2. Enter a valid password but with incorrect case for the suggested wallet.
3. Click on "Submit" or hit "Enter".

**Test Data:** Valid password with incorrect case.

**Expected Result:** An error message should appear, indicating that the password is incorrect.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Login-05

**Description:** Verify that the password is masked (hidden) as the user types it.

**Steps:**

1. Launch Smapp.
2. Start typing in the password field.

**Test Data:** Any characters for the password.

**Expected Result:** The password should be masked (e.g., displayed as asterisks or dots).

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Login-06

**Description:** Simulate network interruptions during the login process to ensure graceful handling of such situations.

**Steps:**

1. Launch Smapp.
2. Disconnect the network.
3. Try to log in with a valid password.

**Test Data:** Valid password with the network disconnected.

**Expected Result:** An error message should appear indicating a network issue, but the user should be able to log in.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Login-07

**Description:** Check if the login module works seamlessly on various desktop operating systems (e.g., Windows, macOS, Linux).

**Steps:**

1. Launch Smapp on different operating systems.
2. Log in with a valid password.

**Test Data:** Valid password.

**Expected Result:** User should be able to log in successfully on all tested operating systems.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Login-08

**Description:** Verify that the login module works correctly with different languages and character sets.

**Steps:**

1. Launch Smapp.
2. Change the application language if applicable.
3. Log in with a valid password.

**Test Data:** Valid password in different language options.

**Expected Result:** User should be able to log in successfully and see the interface in the selected language.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Login-09

**Description:** Confirm that error messages are clear and informative for users encountering login issues.

**Steps:**

1. Launch Smapp.
2. Enter an invalid password.
3. Observe the error message.

**Test Data:** Invalid password.

**Expected Result:** The error message should be clear, readable, and informative, such as “Sorry, this password doesn't ring a bell; please try again.”

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Login-10

**Description:** Ensure that login attempts and related activities are correctly logged for security and auditing purposes.

**Steps:**

1. Launch Smapp.
2. Attempt to log in.
3. Check the logs.

**Test Data:** Valid and invalid passwords.

**Expected Result:** All login attempts, both successful and unsuccessful, should be logged with relevant details for auditing.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Login-11

**Description:** Verify the behavior of pressing the "Enter" key in the password field.

**Steps:**

1. Launch Smapp.
2. Enter a valid password.
3. Press the "Enter" key.

**Test Data:** Valid password.

**Expected Result:** The "Enter" key should trigger the login process, and the user should be logged in successfully.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

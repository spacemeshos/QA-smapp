# Test Scenario

#### Unique ID: POScoinbase

**Description:** This scenario covers the functionality and validation of the Coinbase choosing step during POS setup in Smapp.

**Priority:** 1

**Prerequisites:** User is logged into Smapp with a multi-account Wallet, and has initiated the POS setup process.

**Test Cases:**

* [01](#test-case-id-POScoinbase-01) - Verify auto-population of coinbase field with the address of the currently logged-in wallet.
* [02](#test-case-id-POScoinbase-02) - Verify the ability to manually type a new valid wallet address into the coinbase field.
* [03](#test-case-id-POScoinbase-03) - Test validation of the coinbase field for incorrect or invalid addresses.
* [04](#test-case-id-POScoinbase-04) - Verify dropdown list functionality displaying all accounts associated with the current wallet.
* [05](#test-case-id-POScoinbase-05) - Check coinbase field updates upon selecting an account from the dropdown.
* [06](#test-case-id-POScoinbase-06) - Test persistence of the selected coinbase address in the config file after completing the POS setup.
* [07](#test-case-id-POScoinbase-07) - Verify system behavior when attempting to proceed with an empty coinbase field.
* [08](#test-case-id-POScoinbase-08) - Check that the coinbase setup step is logged appropriately.
* [09](#test-case-id-POScoinbase-09) - Test behavior when copying and pasting addresses with leading or trailing spaces.

---

# Test Cases

#### Test Case ID: POScoinbase-01

**Description:** Verify that during POS setup, the coinbase field is automatically populated with the address of the currently logged-in wallet.

**Steps:**

1. Initiate the POS setup process in Smapp.
2. Observe the coinbase field during the setup.

**Test Data:** N/A

**Expected Result:** The coinbase field should be automatically populated with the address of the currently logged-in wallet.

---

#### Test Case ID: POScoinbase-02

**Description:** Verify the ability to manually type a new valid wallet address into the coinbase field.

**Steps:**

1. Access the coinbase field during the POS setup.
2. Manually type a new valid wallet address into the field.

**Test Data:** A valid wallet address.

**Expected Result:** The manually entered wallet address should be accepted and displayed in the coinbase field.

---



#### Test Case ID: POScoinbase-03

**Description:** Test the validation of the coinbase field to ensure incorrect or invalid addresses are not accepted.

**Steps:**

1. Access the coinbase field during the POS setup.
2. Enter an incorrect or invalid wallet address.

**Test Data:** Incorrect or invalid wallet addresses.

**Expected Result:** The system should not accept incorrect or invalid addresses and display an error message.

---

#### Test Case ID: POScoinbase-04

**Description:** Verify the dropdown list functionality displays all accounts associated with the current wallet.

**Steps:**

1. Click on the dropdown icon in the coinbase field during the POS setup.
2. Observe the list of accounts displayed.

**Test Data:** A multi-account wallet.

**Expected Result:** The dropdown list should display all accounts associated with the currently logged-in wallet.

---

#### Test Case ID: POScoinbase-05

**Description:** Check that upon selecting an account from the dropdown, the coinbase field updates to the chosen address.

**Steps:**

1. Access the coinbase dropdown list during the POS setup.
2. Select an account from the list.

**Test Data:** A multi-account wallet.

**Expected Result:** The rewards address field should update to display the address of the selected account.

---

#### Test Case ID: POScoinbase-06

**Description:** Test for the persistence of the selected coinbase address in the config file after completing the POS setup.

**Steps:**

1. Complete the POS setup with a chosen coinbase address.
2. Check the config file for the persistence of the selected address.

**Test Data:** Selected coinbase address during the POS setup.

**Expected Result:** The config file should contain the selected coinbase address persistently after the setup is completed.

---

#### Test Case ID: POScoinbase-07

**Description:** Verify the system behavior when attempting to proceed with an empty coinbase field.

**Steps:**

1. Leave the coinbase field empty during the POS setup.
2. Attempt to proceed to the next step of the setup.

**Test Data:** An empty coinbase field.

**Expected Result:** The system should prevent proceeding and display an error message.

---


#### Test Case ID: POScoinbase-08

**Description:** Check that the coinbase setup step is logged appropriately for audit and troubleshooting purposes.

**Steps:**

1. Complete the coinbase choosing step in the POS setup.
2. Check the app logs to review the entries related to the coinbase setup.

**Test Data:** A valid account address.

**Expected Result:** The application logs should contain detailed entries about the coinbase setup step, including any changes made, selections, and errors if occurred.

---

#### Test Case ID: POScoinbase-09

**Description:** Test the behavior of the setup when copying and pasting addresses with leading or trailing spaces.

**Steps:**

1. Copy an address with leading or trailing spaces.
2. Paste this address into the coinbase field during the POS setup.
3. Observe how Smapp handles the pasted address.

**Test Data:** A wallet address with leading or trailing spaces.

**Expected Result:** Smapp should trim the leading/trailing spaces and accept the address if valid.

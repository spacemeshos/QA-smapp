# Test Scenario

#### Unique ID: POSsummary

**Description:** Testing the POS Setup Summary Screen, focusing on its functionality, user interactions, and the flow into the Proof of Space data generation process.

**Priority:** 1

**Prerequisites:** User has completed the initial steps of POS setup and has reached the Summary Screen.

**Test Cases:** List of all the test cases for this scenario

[01](#test-case-id-POSsummary-01) - Validate display of POS Setup Summary

[02](#test-case-id-POSsummary-02) - Back button functionality

[03](#test-case-id-POSsummary-03) - Next button functionality

[04](#test-case-id-POSsummary-04) - Edit links functionality

[05](#test-case-id-POSsummary-05) - Confirmation screen post data generation

[06](#test-case-id-POSsummary-06) - Node restart validation

[07](#test-case-id-POSsummary-07) - Data integrity check

[08](#test-case-id-POSsummary-08) - Error handling

[09](#test-case-id-POSsummary-09) - UI/UX consistency and responsiveness



---

# Test Cases

#### Test Case ID: POSsummary-01

**Description:** Verify that all expected elements (Data Directory, Data Size, Max File Size, Provider, Data Generation Max Speed) are correctly displayed on the POS Setup Summary Screen.

**Steps:**

1. Navigate to the POS Setup Summary Screen.
2. Verify that all elements are displayed.
3. Check for correct and complete data in each element.

**Test Data:** The parameters set in the previous steps.

**Expected Result:** All elements are displayed with correct and complete information.

---

#### Test Case ID: POSsummary-02

**Description:** Test the functionality of the 'Back' button on the POS Setup Summary Screen.

**Steps:**

1. Click the 'Back' button on the POS Setup Summary Screen.
2. Observe the screen transition.

**Test Data:** Not applicable.

**Expected Result:** Clicking 'Back' navigates the user to the previous screen in the setup process. There are no changes or lost params after going back.

---

#### Test Case ID: POSsummary-03

**Description:** Ensure the 'Next' button starts the Proof of Space data generation process and leads to a confirmation screen.

**Steps:**

1. Click the 'Next' button on the POS Setup Summary Screen.
2. Observe the initiation of the data generation process.
3. Check for the appearance of the confirmation screen.

**Test Data:** Not applicable.

**Expected Result:** The data generation process begins, the node restarts, and a confirmation screen is displayed.

---

#### Test Case ID: POSsummary-04

**Description:** Validate the functionality of edit links for each item (Data Directory, Data Size, etc.) on the POS Setup Summary Screen.

**Steps:**

1. Click each edit link next to the items on the summary screen.
2. Verify the redirection to the respective editing screen.
3. Edit the data and save the changes.
4. Return to the summary screen and verify the updates.

**Test Data:** Various valid and invalid inputs for each item.

**Expected Result:** Each edit link correctly redirects to the editing screen, allows changes, and displays updated information on the summary screen.

---

#### Test Case ID: POSsummary-05

**Description:** Verify the display and content of the confsirmation screen after the Proof of Space data generation process.

**Steps:**

1. Complete the POS setup and click 'Next' on the Summary Screen.
2. Observe the data generation process and the node restart.
3. Verify the display of the confirmation screen with relevant information.

**Test Data:** Not applicable.

**Expected Result:** A confirmation screen is displayed with relevant information post data generation.

---

#### Test Case ID: POSsummary-06

**Description:** Confirm the successful restart of the node after initiating the Proof of Space data generation.

**Steps:**

1. Click 'Next' on the POS Setup Summary Screen to start data generation.
2. Observe the behavior of the node during this process.
3. Confirm the node restarts as expected.

**Test Data:** Not applicable.

**Expected Result:** The node restarts successfully without errors during or after the data generation process.

---

#### Test Case ID: POSsummary-07

**Description:** Validate the integrity of the data generation in the Proof of Space setup.

**Steps:**

1. Complete the Proof of Space data generation.
2. Verify the data in the specified directory and in the config file.
3. Check for data consistency and integrity.

**Test Data:** Data generated from the Proof of Space setup.

**Expected Result:** Data in the directory matches expected size, format and the config file reflects the choosen params.

---

#### Test Case ID: POSsummary-08

**Description:** Test error handling mechanisms on the POS Setup Summary Screen, especially when proceeding to the next step.

**Steps:**

1. Simulate possible errors (like disconnection, system errors, POS provider unavailability) during the POS setup.
2. Click 'Next' to initiate the data generation.
3. Observe the error handling and messaging.

**Test Data:** Various error conditions.

**Expected Result:** Appropriate error messages are displayed, and the system handles errors gracefully without crashing.

---

#### Test Case ID: POSsummary-09

**Description:** Check for UI/UX consistency and responsiveness on the POS Setup Summary Screen across different devices and resolutions.

**Steps:**

1. Access the POS Setup Summary Screen on various devices and resolutions.
2. Check for UI elements' alignment, visibility, and responsiveness.
3. Interact with the screen elements to assess usability.

**Test Data:** Different screen sizes and resolutions.

**Expected Result:** The screen maintains a consistent look and feel, is responsive, and functions correctly across all tested devices and resolutions.

---

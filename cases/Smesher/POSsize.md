# Test Scenario

#### Unique ID: POSSize

**Description:** Testing the functionality for setting up the Proof of Space (POS) size during the setup process. This includes input validation for the number of units, where 1 unit equals 64 Gibibytes, with options to manually input a value or use arrow keys for increment/decrement. The minimum allowable size is 4 units.

**Priority:**

**Prerequisites:** Access to the POS setup interface where the user can select the POS size.

**Test Cases:** List of all the test cases for this scenario

[01](#test-case-id-possize-01) - Validate minimum unit input

[02](#test-case-id-possize-02) - Validate manual input of units

[03](#test-case-id-possize-03) - Validate increment functionality using arrow keys

[04](#test-case-id-possize-04) - Validate decrement functionality using arrow keys

[05](#test-case-id-possize-05) - Validate input of non-integer values

[06](#test-case-id-possize-06) - Validate input of negative values



# Test Cases

#### Test Case ID: POSSize-01

**Description:** Verify that the minimum unit input is restricted to 4 units.

**Steps:**

1. Access the POS size setup interface.
2. Try to input a value less than 4 units.

**Test Data:** Various values below 4 units.

**Expected Result:** The system should not allow values less than 4 units and should display an appropriate error message.


---

#### Test Case ID: POSSize-02

**Description:** Check the functionality of manual input for the number of units.

**Steps:**

1. Access the POS size setup interface.
2. Manually input a valid number of units (e.g., 5, 10).

**Test Data:** Various valid unit numbers.

**Expected Result:** The system should accept the manual input of valid unit numbers without error.


---

#### Test Case ID: POSSize-03

**Description:** Validate the increment functionality using the arrow keys.

**Steps:**

1. Access the POS size setup interface.
2. Use the arrow key to increment the number of units.

**Test Data:** Use arrow key for incrementing units.

**Expected Result:** The number of units should increment correctly with each arrow key press.


---

#### Test Case ID: POSSize-04

**Description:** Validate the decrement functionality using the arrow keys.

**Steps:**

1. Access the POS size setup interface.
2. Use the arrow key to decrement the number of units.

**Test Data:** Use arrow key for decrementing units.

**Expected Result:** The number of units should decrement correctly with each arrow key press but should not go below 4 units.


---

#### Test Case ID: POSSize-05

**Description:** Check the system's response to non-integer values in the unit input field.

**Steps:**

1. Access the POS size setup interface.
2. Input non-integer values (e.g., alphabets, special characters).

**Test Data:** Alphabets, special characters, and decimal values.

**Expected Result:** The system should restrict non-integer values and display an appropriate error message.


---

#### Test Case ID: POSSize-06

**Description:** Verify the system's behavior when negative values are input.

**Steps:**

1. Access the POS size setup interface.
2. Try to input a negative value.

**Test Data:** Negative values.

**Expected Result:** The system should not accept negative values and should display an appropriate error message.


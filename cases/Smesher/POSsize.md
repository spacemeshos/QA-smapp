# Test Scenario

#### Unique ID: POSSize

**Description:** Testing the functionality for setting up the Proof of Space (POS) size during the setup process. This includes input validation for the number of units, where 1 unit equals 64 Gibibytes, with options to manually input a value or use arrow keys for increment/decrement. The minimum allowable size is 4 units.

**Priority:**

**Prerequisites:** Access to the POS setup interface where the user can select the POS size.

**Test Cases:** List of all the test cases for this scenario

*POS total size:*

[01](#test-case-id-possize-01) - Validate minimum unit input

[02](#test-case-id-possize-02) - Validate manual input of units

[03](#test-case-id-possize-03) - Validate increment functionality using arrow keys

[04](#test-case-id-possize-04) - Validate decrement functionality using arrow keys

[05](#test-case-id-possize-05) - Validate input of non-integer values

[06](#test-case-id-possize-06) - Validate input of negative values

*Max File Size:*

[07](#test-case-id-possize-07) - Validate default file size

[08](#test-case-id-possize-08) - Validate input of negative numbers

[09](#test-case-id-possize-09) - Validate warning message for values above 4096 MiB

[10](#test-case-id-possize-10) - Validate input of very low values

[11](#test-case-id-possize-11) - Validate input of non-integer values

[12](#test-case-id-possize-12) - Validate saving of the chosen value in the config

[13](#test-case-id-possize-13) - Validate correct file generation based on input

[14](#test-case-id-possize-14) - Validate input of extremely large values

*POS directory details:*

[16](#test-case-id-possize-16) - Validate display of POS data folder path

[17](#test-case-id-possize-17) - Validate accuracy of free space display

[18](#test-case-id-possize-18) - Validate display after changing POS data folder (edit in the previous steps)

[19](#test-case-id-possize-19) - Validate the response when the POS data folder is edited,  moved or deleted externally.

[20](#test-case-id-possize-20) - Validate response to directory with insufficient space

[21](#test-case-id-possize-21) - Validate response to inaccessible or restricted directory

[22](#test-case-id-possize-22) - Validate refresh of free space display (to implement in Smapp2?)

[23](#test-case-id-possize-23) - Validate display for different file systems

[24](#test-case-id-possize-24) - Test for correct handling of network drives or external storage as the POS data folder. (to implement in Smapp2?)

[25](#test-case-id-possize-25) - Validate the behavior of the POS setup interface upon system resume from sleep or hibernation.

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

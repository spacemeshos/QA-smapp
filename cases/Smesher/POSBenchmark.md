# Test Scenario

#### Unique ID: POSbenchmark

**Description:** This scenario tests the "proving opts" screen functionality in the POS data generation process, focusing on user interactions, background benchmark processes, and the display and selection of various parameters.

**Priority:** 1

**Prerequisites:** Smapp installed, minimum 256GiB free disk space

**Test Cases:** Comprehensive testing of the "proving opts" screen functionality.

[01](#test-case-id-POSbenchmark-01) - Verifying default CPU core selection

[02](#test-case-id-POSbenchmark-02) - Manual CPU core selection

[03](#test-case-id-POSbenchmark-03) - Assess the consistency of the Speed GiB/s calculation across multiple tests

[04](#test-case-id-POSbenchmark-04) - Display of benchmark results in columns

[05](#test-case-id-POSbenchmark-05) - Manual Nonces input functionality

[06](#test-case-id-POSbenchmark-06) - Row selection functionality for suggested setups

[07](#test-case-id-POSbenchmark-07) - Validating the calculation of Recommended POS size

[08](#test-case-id-POSbenchmark-08) - Status column display accuracy

[09](#test-case-id-POSbenchmark-09) - Functionality of "test chosen options" button

[10](#test-case-id-POSbenchmark-10) - Functionality of "run all benchmarks" button

[11](#test-case-id-POSbenchmark-11) - Passing parameters to config after selection

[12](#test-case-id-POSbenchmark-12) - Skipping tests and proceeding with selected options

---

# Test Cases

#### Test Case ID: POSbenchmark-01

**Description:** Verify that the default CPU core selection is set to 3/4 of the total number of cores.

**Steps:**

1. Open the "proving opts" screen.
2. Observe the default value in the CPU core selection field.

**Test Data:** Total number of CPU cores available (check for your PC).

**Expected Result:** The default value in the CPU core selection field should be 3/4 of the total number of CPU cores.

---

#### Test Case ID: POSbenchmark-02

**Description:** Test the functionality of manually selecting the number of CPU cores.

**Steps:**

1. Open the "proving opts" screen.
2. Manually input a specific number of CPU cores in the CPU core selection field.
3. Confirm the selection.

**Test Data:** Specific number of CPU cores to be selected.

**Expected Result:** The manually selected number of CPU cores should be accepted and reflected in the config, smeshing screen and proof generation process (also in the benchmark process if run).

---

#### Test Case ID: POSbenchmark-03

**Description:** Assess the consistency of the Speed GiB/s calculation across multiple tests.

**Steps:**

1. Run the benchmark process multiple times under similar conditions.
2. Compare the Speed GiB/s results across these tests.

**Test Data:** Results from multiple benchmark tests.

**Expected Result:** The Speed GiB/s results should be consistent across multiple tests under similar conditions.

---

#### Test Case ID: POSbenchmark-04

**Description:** Verify the correct display of benchmark results in the specified columns.

**Steps:**

1. Wait for the benchmark process to complete.
2. Check the results are displayed in the columns for Speed GiB/s, Recommended POS size, and Status.

**Test Data:** Benchmark results data.

**Expected Result:** Benchmark results are correct and displayed in their respective columns, the status shows "complete".

---

#### Test Case ID: POSbenchmark-05

**Description:** Test the functionality of manually inputting Nonces.

**Steps:**

1. Open the "proving opts" screen.
2. Manually enter a specific number of Nonces.
3. Confirm the input.

**Test Data:** Specific number of Nonces.

**Expected Result:** The entered number of Nonces should be accepted and reflected in the config, smeshing screen summary and proving process (and benchmark if run).

---

#### Test Case ID: POSbenchmark-06

**Description:** Validate the functionality of selecting a row from the suggested setups.

**Steps:**

1. Open the "proving opts" screen.
2. Select one of the rows in the suggested setups.
3. Confirm the selection.

**Test Data:** N/A

**Expected Result:** The selection of a suggested setup should be accepted and its values used in the config, smeshing screen summary and proving process (and benchmark if run).

---

#### Test Case ID: POSbenchmark-07

**Description:** Verify the accuracy of the Recommended POS size calculation based on benchmark results.

**Steps:**

1. Complete the benchmark process.
2. Observe the calculated Recommended POS size based on the results.

**Test Data:** Benchmark results data.

**Expected Result:** The Recommended POS size should accurately reflect the capacity needed to generate proofs in time based on the benchmark results.

---

#### Test Case ID: POSbenchmark-08

**Description:** Check the accuracy of the Status column during the benchmark process.

**Steps:**

1. Observe the Status column during the benchmark process.
2. Ensure it displays "idle", "queued", "running", or "complete" appropriately.

**Test Data:** N/A

**Expected Result:** The Status column should accurately reflect the current state of the benchmark process.

---

#### Test Case ID: POSbenchmark-09

**Description:** Test the functionality of the "test chosen options" button.

**Steps:**

1. Select or input specific options.
2. Click the "test chosen options" button.

**Test Data:** Selected or manually inputted options.

**Expected Result:** The system should run the benchmark test with the chosen options and display the results.

---

#### Test Case ID: POSbenchmark-10

**Description:** Ensure the "run all benchmarks" button functions correctly.

**Steps:**

1. Click the "run all benchmarks" button.
2. Observe if all the benchmarks are run and results are displayed.

**Test Data:** N/A

**Expected Result:** All benchmarks should run, and their results should be displayed in the respective columns.

---

#### Test Case ID: POSbenchmark-11

**Description:** Validate that selected parameters are correctly passed to the config file.

**Steps:**

1. Select or input specific options.
2. Proceed to the next step or confirm the selection.
3. Check the config file to verify the selected options are passed correctly.

**Test Data:** Selected or manually inputted options.

**Expected Result:** The config file should accurately reflect the selected options.

---

#### Test Case ID: POSbenchmark-12

**Description:** Test the functionality of skipping tests and proceeding with selected options.

**Steps:**

1. Select or input specific options.
2. Click “Next” without running the tests.
3. Check if Smapp proceeds with the selected options.

**Test Data:** Selected or manually inputted options.

**Expected Result:** Smapp should proceed with the selected options without running the benchmark tests.

---

#### Test Case ID: POSbenchmark-13

**Description:** Validate input field restrictions for CPU Threads and Nonces.

**Steps:**

1. Attempt to enter invalid values in the CPU Threads and Nonces input fields.
2. Observe the Smapp's response.

**Test Data:** Various invalid input values (like negative numbers, decimals, or excessively high numbers).

**Expected Result:** The system should prevent invalid entries or display an appropriate error/ warning message.(for smapp 2)

---

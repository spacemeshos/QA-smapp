# Test Scenario

#### Unique ID: POSdirectory

**Description:** This scenario involves testing various aspects of the directory picker functionality in the application, including its invocation, handling of different directory types and states, interaction with the file system, and the UI's response to user actions.

**Priority:** 1

**Prerequisites:** The application must be installed and operational. Ensure that various types of directories and file systems are available for testing, including empty and non-empty directories, directories with varying disk space, and removable media.

**Test Cases:** List of all the test cases for this scenario

[01](#test-case-id-POSdirectory-01) - Directory Picker Invocation

[02](#test-case-id-POSdirectory-02) - Directory Picker Cancelation

[03](#test-case-id-POSdirectory-03) - Valid Directory Selection

[04](#test-case-id-POSdirectory-04) - Invalid Directory Selection - Non-empty Directory

[05](#test-case-id-POSdirectory-05) - Sufficient Free Disk Space Verification

[06](#test-case-id-POSdirectory-06) - Insufficient Free Disk Space Verification

[07](#test-case-id-POSdirectory-07) - Display of Free Space

[08](#test-case-id-POSdirectory-08) - Refresh of Free Space Info on Directory Change

[09](#test-case-id-POSdirectory-09) - Cancel Button Functionality

[10](#test-case-id-POSdirectory-10) - File System Permissions

[11](#test-case-id-POSdirectory-11) - Selection of Removable Media

[12](#test-case-id-POSdirectory-12) - Reacting to External Changes in Directory

[13](#test-case-id-POSdirectory-13) - Network Location Selection

[14](#test-case-id-POSdirectory-14) - Directory Selection After Warning

[15](#test-case-id-POSdirectory-15) - Test the Warning Shows Each Time a Non-empty Directory Selected

[16](#test-case-id-POSdirectory-16) - Next Button State Persistence

[17](#test-case-id-posdirectory-17) - Directory Selection Persistence

[18](#test-case-id-POSdirectory-18) - Directory Path Length

[19](#test-case-id-POSdirectory-19) - Directory with Hidden Files

[20](#test-case-id-POSdirectory-20) - Reactivity to Disk Space Changes

[21](#test-case-id-POSdirectory-21) - Choosing a Directory with Symlinks

[22](#test-case-id-POSdirectory-22) - Directory Selection on Different File Systems

[23](#test-case-id-POSdirectory-23) - Impact of Disk Space Requirement on System Performance

[24](#test-case-id-POSdirectory-24) - Multiple Directory Selection Attempts

[25](#test-case-id-POSdirectory-25) - Error Handling for File System Errors

[26](#test-case-id-POSdirectory-26) - Language and Encoding Support in Directory Paths

[27](#test-case-id-POSdirectory-27) - User Interface Responsiveness

[28](#test-case-id-POSdirectory-28) - Handling of External Drives Being Ejected

---

# Test Cases

#### Test Case ID: POSdirectory-01

**Description:** Verify if the directory picker dialog opens upon clicking the link.

**Steps:**

1. Launch the application.
2. Navigate to the POS setup - first screen - where the directory picker can be invoked.
3. Click the link or button to open the directory picker.

**Test Data:** N/A

**Expected Result:** The dialog for choosing a directory should open without errors.

---

#### Test Case ID: POSdirectory-02

**Description:** Ensure the directory picker dialog can be canceled without any side effects.

**Steps:**

1. Open the directory picker dialog.
2. Click the 'Cancel' button or close the dialog.

**Test Data:** N/A

**Expected Result:** Canceling the dialog should not select any directory, and previously selected directory (if any) remains unchanged.

---

#### Test Case ID: POSdirectory-03

**Description:** Check if a valid directory selection enables the 'Next' button.

**Steps:**

1. Open the directory picker dialog.
2. Select a valid, empty directory.
3. Observe the state of the 'Next' button.

**Test Data:** Valid, empty directory.

**Expected Result:** The 'Next' button becomes active when a valid, empty directory is chosen.

---

#### Test Case ID: POSdirectory-04

**Description:** Confirm that selecting a non-empty directory shows a warning.

**Steps:**

1. Open the directory picker dialog.
2. Select a directory that is not empty.
3. Observe the response of the application.

**Test Data:** Non-empty directory.

**Expected Result:** A warning is displayed, and the PoS process does not start if the folder content isn't a valid POS matching the config.

---

#### Test Case ID: POSdirectory-05

**Description:** Verify that the 'Next' button is enabled when the directory has more than the required free disk space.

**Steps:**

1. Open the directory picker dialog.
2. Select a directory with sufficient free disk space.
3. Observe the 'Next' button.

**Test Data:** Directory with sufficient free disk space.

**Expected Result:** The 'Next' button is active when there is sufficient free disk space.

---

#### Test Case ID: POSdirectory-06

**Description:** Check if the 'Next' button is disabled when there's not enough free disk space.

**Steps:**

1. Open the directory picker dialog.
2. Select a directory with insufficient free disk space.
3. Observe the 'Next' button and any warning messages.

**Test Data:** Directory with insufficient free disk space.

**Expected Result:** The 'Next' button is disabled, and the user is warned about insufficient space.

---

#### Test Case ID: POSdirectory-07

**Description:** Verify that the free space in the chosen directory is accurately displayed.

**Steps:**

1. Open the directory picker dialog.
2. Select different directories with varying free disk space.
3. Observe the displayed free space information.

**Test Data:** Directories with different amounts of free disk space.

**Expected Result:** The note shows the correct amount of free disk space.

---

#### Test Case ID: POSdirectory-08

**Description:** Ensure that the free space information updates when a different directory is selected.

**Steps:**

1. Open the directory picker dialog.
2. Select a directory and observe the displayed free space.
3. Select a different directory and observe the updated free space information.

**Test Data:** Two or more directories with different free disk space.

**Expected Result:** The displayed free disk space updates to reflect the new directory's free space.

---

#### Test Case ID: POSdirectory-09

**Description:** Verify that the 'Cancel' button cancels the PoS directory selection process.

**Steps:**

1. Open the directory picker dialog.
2. Click the 'Cancel' button during the selection process.

**Test Data:** N/A

**Expected Result:** Clicking 'Cancel' exits the directory selection process without proceeding to the next step.

---

#### Test Case ID: POSdirectory-10

**Description:** Verify that the application handles the selection of a directory with restricted permissions correctly.

**Steps:**

1. Attempt to select a directory with restricted file system permissions.
2. Observe the application's response.

**Test Data:** Directory with restricted permissions.

**Expected Result:** The application should either not allow the selection of such a directory or should display an appropriate warning message.

---

#### Test Case ID: POSdirectory-11

**Description:** Confirm that selecting a directory on removable media is handled properly.

**Steps:**

1. Open the directory picker dialog.
2. Select a directory located on removable media (e.g., external drive).
3. Observe the application's response and behavior.

**Test Data:** Directory on removable media.

**Expected Result:** The application should accept such directory and maybe smapp2 should warn about potential issues with removable media.

---

#### Test Case ID: POSdirectory-12

**Description:** Verify the application's behavior if the chosen directory is modified outside the app (e.g., files added/removed externally).

**Steps:**

1. Select a directory using the directory picker.
2. Modify the contents of the directory outside of the application (add or remove files).
3. Observe how the application responds to these changes.

**Test Data:** Directory modified externally after selection.

**Expected Result:** To be discussed for smapp2 - maybe there should be a notification or warning about it if possible to detect changes in realtime

---

#### Test Case ID: POSdirectory-13

**Description:** Assess the behavior when a network location is selected as the PoS directory.

**Steps:**

1. Open the directory picker dialog.
2. Attempt to select a network location as the directory.
3. Observe the application's response.

**Test Data:** Network location.

**Expected Result:** The application should handle it correctly, and maybe smapp2 should warn about potential issues.

---

#### Test Case ID: POSdirectory-14

**Description:** Check if the user can select a new directory after receiving a warning for choosing a non-empty directory.

**Steps:**

1. Select a non-empty directory and receive a warning.
2. Attempt to select a new, different directory.
3. Observe the application's response.

**Test Data:** Initially a non-empty directory, followed by a new empty directory selection.

**Expected Result:** The user should be able to select a new directory, and the application should update accordingly.

---

#### Test Case ID: POSdirectory-15

**Description:** Test the warning display after reselection of a non-empty directory multiple times for different directories.

**Steps:**

1. Select a non-empty directory and receive a warning.
2. Select a different non-empty directory after the warning.
3. Repeat step 2.
4. Observe the application's behavior and response.

**Test Data:** Initially a non-empty directory, followed by a different non-empty directory selection.

**Expected Result:** The warning should appear each time the user selects a non-empty directory.

---

#### Test Case ID: POSdirectory-16

**Description:** Check if the state of the 'Next' button persists correctly when navigating back to the first step after advancing in the setup process.

**Steps:**

1. Select a valid directory and proceed to the next step in the setup.
2. Navigate back to the directory selection step.
3. Observe the state of the 'Next' button.

**Test Data:** N/A

**Expected Result:** The 'Next' button should retain its enabled based on the previous interactions.

---

#### Test Case ID: POSdirectory-17

**Description:** Verify that the selected directory is remembered if the user navigates to the next step and then returns back to the directory selection step.

**Steps:**

1. Select a directory and proceed to the next step in the setup.
2. Navigate back to the directory selection step.
3. Check if the previously selected directory is still selected.

**Test Data:** N/A

**Expected Result:** The previously selected directory should still be selected upon returning to the directory selection step.

---

#### Test Case ID: POSdirectory-18

**Description:** Ensure the application can handle long directory paths beyond typical filesystem limits.

**Steps:**

1. Attempt to select a directory with an exceptionally long path.
2. Observe the application's response and behavior.

**Test Data:** Directory with a long path.

**Expected Result:** The application should accept the long path

---

#### Test Case ID: POSdirectory-19

**Description:** Confirm that selecting a directory that contains hidden files or system files triggers the non-empty directory warning.

**Steps:**

1. Open the directory picker dialog.
2. Select a directory that contains hidden or system files.
3. Observe the application's reaction to this selection.

**Test Data:** Directory containing hidden/system files.

**Expected Result:** The application should recognize the directory as non-empty and warn the user.

---

#### Test Case ID: POSdirectory-20

**Description:** Check if the application updates the free space note and 'Next' button status in real-time as disk space changes.

**Steps:**

1. Open the directory picker and select a directory.
2. Change the disk space of the selected directory externally (e.g., by adding/removing files).
3. Observe if the free space note and 'Next' button status are updated accordingly.

**Test Data:** Directory with changing disk space.

**Expected Result:** The note and the 'Next' button's status should reflect the current state of the disk space without needing to reopen or refresh the application.(for smapp2)

---

#### Test Case ID: POSdirectory-21

**Description:** Test the application's behavior when selecting a directory that contains symlinks.

**Steps:**

1. Open the directory picker dialog.
2. Select a directory that includes symlinks.
3. Observe how the application handles the symlinks.

**Test Data:** Directory containing symlinks.

**Expected Result:** The application should correctly handle symlinks within the directory.

---

#### Test Case ID: POSdirectory-22

**Description:** Verify that the application can handle directory selection across different filesystems (e.g., NTFS, FAT32, exFAT, ext4).

**Steps:**

1. Open the directory picker dialog.
2. Select directories on different filesystems.
3. Observe the application's compatibility and response.

**Test Data:** Directories on various filesystems such as NTFS, FAT32, exFAT, ext4.

**Expected Result:** The application should support all these filesystems.

---

#### Test Case ID: POSdirectory-23

**Description:** Assess the impact on system performance when the minimum required disk space is nearly consumed.

**Steps:**

1. Select a directory that nearly fulfills the minimum disk space requirement.
2. Monitor the system performance and application's behavior.
3. Observe any warnings or notifications provided by the application.

**Test Data:** Directory with disk space close to the minimum requirement.

**Expected Result:** The application should warn the user if the disk space usage might affect system performance or if it's too close to the limit. (for smapp2))

---

#### Test Case ID: POSdirectory-24

**Description:** Ensure the application can handle multiple directory selection attempts without crashing or displaying incorrect information.

**Steps:**

1. Repeatedly open and close the directory picker, selecting different directories each time.
2. Observe the application's stability and the accuracy of the displayed information.

**Test Data:** Various directories selected in multiple attempts.

**Expected Result:** Users should be able to attempt directory selection multiple times with consistent and accurate feedback from the application.

---

#### Test Case ID: POSdirectory-25

**Description:** Test how the application handles unexpected file system errors during directory selection (e.g., read/write permissions, disk errors).

**Steps:**

1. Attempt to select a directory where file system errors are likely (e.g., read-only directory, disk with errors).
2. Observe the application's error handling and messaging.

**Test Data:** Directories with potential file system errors.

**Expected Result:** The application should display an appropriate error message and not allow the user to proceed with an invalid selection.

---

#### Test Case ID: POSdirectory-26

**Description:** Verify that the application supports directory paths with non-English characters and various encodings.

**Steps:**

1. Attempt to select directories with paths containing non-English characters and different encodings.
2. Observe the application's ability to handle these paths.

**Test Data:** Directories with non-English characters and various encodings in their paths.

**Expected Result:** The application should properly handle paths with a variety of characters and encodings without errors.

---

#### Test Case ID: POSdirectory-27

**Description:** Test the responsiveness of the user interface when interacting with the directory picker on systems with low resources.

**Steps:**

1. Operate the application on a system with limited resources.
2. Use the directory picker and observe its responsiveness.
3. Note any lag, freezing, or crashing of the application.

**Test Data:** System with low resources.

**Expected Result:** The directory picker should remain responsive and should not cause the application to hang or crash.

---

#### Test Case ID: POSdirectory-28

**Description:** Check the application's behavior if the selected directory is on an external drive that gets ejected.

**Steps:**

1. Select a directory on an external drive using the directory picker.
2. Eject the external drive while the directory is still selected.
3. Observe the application's response and handling of this situation.

**Test Data:** Directory on an external drive that gets ejected.

**Expected Result:** The application should handle this gracefully, either by prompting the user to re-select a directory or by displaying a clear warning message.(for smapp2)

---

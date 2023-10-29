# Test Scenario

#### Unique ID: POSsetup

**Description:** Proof of Space setup process general overview. Because of it’s complexity, each step is described in more detail separately.

**Priority:** 1

**Dependencies:** tbu

**Prerequisites:** latest Smapp installed, min 260GiB free disk space, decent GPU and CPU

**Test Cases:**
[01](#test-case-id-POSsetup-01) - Validate number of POS files in the directory

[02](#test-case-id-POSsetup-02) - Validate file size of generated POS files

[03](#test-case-id-POSsetup-03) - Validate node restarts after POS setup

[04](#test-case-id-POSsetup-04) - Validate account address selection for coinbase

[05](#test-case-id-POSsetup-05) - Validate error handling for invalid account address for coinbase

[06](#test-case-id-POSsetup-06) - Validate summary screen details against entered data

[07](#test-case-id-POSsetup-07) - Validate POS setup cancellation

[08](#test-case-id-POSsetup-08) - Validate manual input for max file size

[09](#test-case-id-POSsetup-09) - Validate POS setup with minimum allowable data size

[10](#test-case-id-POSsetup-10) - Validate POS setup with maximum allowable data size

[11](#test-case-id-POSsetup-11) - Validate default processor selection for POS setup

[12](#test-case-id-POSsetup-12) - Validate custom processor selection for POS setup

[13](#test-case-id-POSsetup-13) - Validate handling of file system limitations for max file size

[14](#test-case-id-POSsetup-14) - Validate the data size recalculation upon unit increase or decrease

[15](#test-case-id-POSsetup-15) - Validate log entries during POS setup

[16](#test-case-id-POSsetup-16) - Validate status and errors when network is not synced

[17](#test-case-id-POSsetup-17) - Validate status and errors with insufficient disk space

[18](#test-case-id-POSsetup-18) - Validate UI elements and their alignment in the Smeshing screen

[19](#test-case-id-POSsetup-19) - Validate that all dropdowns load their values correctly

[20](#test-case-id-POSsetup-20) - Validate that tooltips are displayed for information icons and they contain correct information

[21](#test-case-id-POSsetup-21) - Validate the speed of the benchmark process

[22](#test-case-id-POSsetup-22) - Validate the automatic preselection of the fastest processor

[23](#test-case-id-POSsetup-23) - Validate POS setup in different operating systems (Windows, macOS, Linux)

[24](#test-case-id-POSsetup-24) - Validate POS setup when the application is under high CPU load

[25](#test-case-id-POSsetup-25) - Validate POS setup when disk IO is high

[26](#test-case-id-POSsetup-26) - Validate POS setup when system goes to sleep and wakes up during the process

[27](#test-case-id-POSsetup-27) - Validate that the 'Next' and 'Create Data' buttons are disabled when mandatory fields are not filled

[28](#test-case-id-POSsetup-28) - Validate the ability to change the coinbase address after POS has started Smeshing (config file)

[29](#test-case-id-POSsetup-29) - Validate the error message when entering an invalid number of units for POS size

[30](#test-case-id-POSsetup-30) - Validate the error message when entering an invalid max file size

[31](#test-case-id-POSsetup-31) - Validate handling of network disruptions during POS setup

[32](#test-case-id-POSsetup-32) - Validate error logs for unsuccessful POS setups

[33](#test-case-id-POSsetup-33) - Validate that the summary screen does allow jumping to the specific steps and editing of details

[34](#test-case-id-POSsetup-34) - Validate POS setup using keyboard navigation only (no mouse)

[35](#test-case-id-POSsetup-35) - Validate that tooltips are available and contain relevant information

[36](#test-case-id-POSsetup-36) - Validate that any 'Back' buttons on the setup screens work as expected

[37](#test-case-id-POSsetup-37) - Validate the behavior when the 'Back' button is clicked after reaching the summary screen

[38](#test-case-id-POSsetup-38) - Validate handling of app crash during POS setup

[39](#test-case-id-POSsetup-39) - Validate that sensitive information is not logged or exposed during the POS setup

[40](#test-case-id-POSsetup-40) - Validate handling of power failure during POS setup and subsequent recovery

[41](#test-case-id-POSsetup-41) - Validate memory usage during POS setup

[42](#test-case-id-POSsetup-42) - Validate CPU usage during POS setup

[43](#test-case-id-POSsetup-43) - Validate disk usage during POS setup

[44](#test-case-id-POSsetup-44) - Validate that the application's other functionalities remain responsive during POS setup

[45](#test-case-id-POSsetup-45) - Validate POS setup when other instances of Smapp are running on the same machine (if applicable)

[46](#test-case-id-POSsetup-46) - Validate handling of automatic updates during POS setup

[47](#test-case-id-POSsetup-47) - Validate that user can multitask within Smapp while the POS generation is ongoing

[48](#test-case-id-POSsetup-48) - Validate handling of disk space running out during POS setup

[49](#test-case-id-POSsetup-49) - Validate the logs for any security vulnerabilities during the POS setup

[50](#test-case-id-POSsetup-50) - Validate handling of corrupted POS data

[51](#test-case-id-POSsetup-51) - Validate trying to initiate another POS setup from another device for the same coinbase

[52](#test-case-id-POSsetup-52) - Validate trying to initiate the same POS data and key from another device at the same time

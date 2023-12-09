# Test Scenario

#### Unique ID: POSsetup

**Description:** Proof of Space setup process general overview. Because of it’s complexity, each step is described in more detail separately.

**Priority:** 1

**Dependencies:** tbu

**Prerequisites:** latest Smapp installed, min 260GiB free disk space, decent GPU and CPU

**Test Cases:**

[01](#test-case-id-POSsetup-01) - Validate that the node restarts correctly after POS setup

[02](#test-case-id-POSsetup-02) - Validate POS setup cancellation

[03](#test-case-id-POSsetup-03) - Validate log entries during POS setup

[04](#test-case-id-POSsetup-04) - Validate status and errors when network is not synced

[05](#test-case-id-POSsetup-05) - Validate status and errors with insufficient disk space

[06](#test-case-id-POSsetup-06) - Validate UI elements and their alignment in the Smeshing screen

[07](#test-case-id-POSsetup-07) - Validate that all dropdowns load their values correctly

[08](#test-case-id-POSsetup-08) - Validate that tooltips are displayed and they contain correct information

[09](#test-case-id-POSsetup-09) - Validate POS setup in different operating systems (Windows, macOS, Linux)

[10](#test-case-id-POSsetup-10) - Validate POS setup when the application is under high CPU load

[11](#test-case-id-POSsetup-11) - Validate POS setup when disk IO is high

[12](#test-case-id-POSsetup-12) - Validate POS setup when system goes to sleep and wakes up during the process

[13](#test-case-id-POSsetup-13) - Validate that the 'Next' and 'Create Data' buttons are disabled when mandatory fields are not filled

[14](#test-case-id-POSsetup-14) - Validate the ability to change the coinbase address after POS has started Smeshing (config file)

[15](#test-case-id-POSsetup-15) - Validate handling of network disruptions during POS setup

[16](#test-case-id-POSsetup-16) - Validate error logs for unsuccessful POS setups

[17](#test-case-id-POSsetup-17) - Validate POS setup using keyboard navigation only (no mouse)

[18](#test-case-id-POSsetup-18) - Validate that any 'Back' buttons on the setup screens work as expected

[19](#test-case-id-POSsetup-19) - Validate handling of app crash during POS setup

[20](#test-case-id-POSsetup-20) - Validate memory usage during POS setup

[21](#test-case-id-POSsetup-21) - Validate CPU usage during POS setup

[22](#test-case-id-POSsetup-22) - Validate disk usage during POS setup

[23](#test-case-id-POSsetup-23) - Validate that the application's other functionalities remain responsive during POS setup

[24](#test-case-id-POSsetup-24) - Validate handling of automatic updates during POS setup

[25](#test-case-id-POSsetup-25) - Validate that user can multitask within Smapp while the POS generation is ongoing

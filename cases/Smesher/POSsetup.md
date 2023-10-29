# Test Scenario

#### Unique ID: POSsetup

**Description:** Proof of Space setup process general overview. Because of it’s complexity, each step is described in more detail separately.

**Priority:** 1

**Dependencies:** tbu

**Prerequisites:** latest Smapp installed, min 260GiB free disk space, decent GPU and CPU

**Test Cases:**
(to be reformatted)

Validate number of POS files in the directory
Validate file size of generated POS files
Validate node restarts after POS setup
Validate account address selection for coinbase
Validate error handling for invalid account address for coinbase
Validate summary screen details against entered data
Validate POS setup cancellation
Validate manual input for max file size
Validate POS setup with minimum allowable data size
Validate POS setup with maximum allowable data size
Validate default processor selection for POS setup
Validate custom processor selection for POS setup
Validate handling of file system limitations for max file size
Validate the data size recalculation upon unit increase or decrease
Validate log entries during POS setup
Validate status and errors when network is not synced
Validate status and errors with insufficient disk space
Validate UI elements and their alignment in the Smeshing screen
Validate that all dropdowns load their values correctly
Validate that tooltips are displayed for information icons and they contain correct information
Validate the speed of the benchmark process
Validate the automatic preselection of the fastest processor
Validate POS setup in different operating systems (Windows, macOS, Linux)
Validate POS setup when the application is under high CPU load
Validate POS setup when disk IO is high
Validate POS setup when system goes to sleep and wakes up during the process
Validate that the 'Next' and 'Create Data' buttons are disabled when mandatory fields are not filled
Validate the ability to change the coinbase address after POS has started Smeshing (config file)
Validate the error message when entering an invalid number of units for POS size
Validate the error message when entering an invalid max file size
Validate handling of network disruptions during POS setup
Validate error logs for unsuccessful POS setups
Validate that the summary screen does allow jumping to the specific steps and editing of details
Validate POS setup using keyboard navigation only (no mouse)
Validate that tooltips are available and contain relevant information
Validate that any 'Back' buttons on the setup screens work as expected
Validate the behavior when the 'Back' button is clicked after reaching the summary screen
Validate handling of app crash during POS setup
Validate that sensitive information is not logged or exposed during the POS setup
Validate handling of power failure during POS setup and subsequent recovery
Validate memory usage during POS setup
Validate CPU usage during POS setup
Validate disk usage during POS setup
Validate that the application's other functionalities remain responsive during POS setup
Validate POS setup when other instances of Smapp are running on the same machine (if applicable)
Validate handling of automatic updates during POS setup
Validate that user can multitask within Smapp while the POS generation is ongoing
Validate handling of disk space running out during POS setup
Validate the logs for any security vulnerabilities during the POS setup
Validate handling of corrupted POS data
Validate trying to initiate another POS setup from another device for the same coinbase
Validate trying to initiate the same POS data and key from another device at the same time

# Proof of Space Data Generator App Requirements Document

## 1. Business Goals and Objectives

- **Purpose:** To facilitate users in generating Proof of Space data efficiently without participating in blockchain mining activities directly.
- **Target Audience:** Users interested in preparing for smeshing by generating or managing POS data.

## 2. Functional Requirements

### POS Setup

(my suggestion: Some pre-selecting the path, holding people by hand while going through the POS Setup processes, like choosing: )

- I want to generate the POS data from scratch (then> a simple or advanced way)
  - simple mode - using default recommended settings (fastest processor, ¾ CPU cores and #of nonces, max file size, etc.)
  - advanced mode, where the user can set everything by himself. (also: add the multi-GPU, CPU affinity,
- I already have the POS data generated, I want to generate more (then some basic questions - i.e. what is your POS total size, what is the file size, select directory, etc) - to make sure they don't lose the data, time, or motivation.  Important: do not delete any data files when the user claims less than actually in the directory, do not panic when the user claims more - display the warning.
- Or even better, but I’m unable to assess the complexity of the correct implementation taking this responsibility on us: ask only for the directory, check, and automatically set all the values for the user, with the option to amend if needed.

### Edit

- the proof generation settings (nonces, CPU threads)
- Change the coinbase
- Changing the POS size without having to start from scratch. (enlarge/shrink/move to another directory…)

### Delete

- Delete the data from the disk and stop smeshing
- Delete only the corrupted part
- Delete only a specific part (shrink size)
- “Are you sure?” popup

### Check

- Check the POS files' correctness and validity - to ensure that the data isn’t corrupted and the User can successfully smesh with it.
- Check the proof generation speed
- Check/ benchmark the available POS processors’ speed, before setting up POS and choosing one of them. This test should give a hint of the speed of the data creation  - in a human language, to be able to roughly predict how much time one will need to generate POS
- A helper checking the user’s PC resources before joining - or (to avoid overcomplicating with the permissions to get this info from the user’s system) a screen with the written minimum/ recommended requirements in terms of GPU, CPU, disk read speed, free disk space (also on root for the network state), Internet connection (bandwidth, speed, etc.), for each, a tooltip with the explanation why it is needed, how will be used, etc.

## 3. Non-Functional Requirements

### UX

- **Guided Setup Process:** Ensure the app provides a clear, step-by-step setup process for both simple and advanced modes. Offer comprehensive in-app guidance, including detailed walkthroughs for setup processes and tooltips for every option, ensuring users understand the implications of their choices.
- **(THE MOST IMPORTANT AND HARD) User Interface:** Design an intuitive interface with easy navigation, clear instructions, and tooltips for additional information.
- **Simplicity and Clarity:** Adopt a minimalist design philosophy that emphasizes clarity and ease of use. Use clear labels, avoid clutter, and prioritize the user's path to the most common actions
- **Efficiency:** Optimize data generation and management processes to utilize system resources effectively without compromising system performance.
- **Reliability:** Ensure robust error handling and data integrity checks to prevent corruption or loss of POS data.
- **Uptime and Stability:** The app should be designed for high uptime and stability,
- **Status Updates:** Provide timely notifications for significant events or milestones in the data generation and verification processes.
- **Multi-Language Support:** Prepare the app for internationalization, allowing for the easy addition of new languages to make the app accessible to a global audience.

### UI

- **Feedback and Interactivity:** Provide immediate and clear feedback for user actions. For example, when a user initiates a data generation task, visually indicate the process has started and update progress in real-time.
- **Responsive Design:** Ensure the app is responsive and adapts to different screen sizes and resolutions. This is particularly important if there's a web version or if the app will be used across various devices.
- **Visual Customization:**  allow users to customize the visual aspects of the app to suit their preferences, such as light mode, dark mode...

### Other

- **Security TBU**
- **Sentry** reports: automatic + users' feedback

## 4. Technical Requirements

### Technology Stack

- TBU

### Development and Deployment

- **Cross-Platform Support:** Ensure compatibility with major operating systems (Windows, macOS, Linux).
- TBU

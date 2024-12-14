# Cheat Engine Detection

This repository contains a project that detects the presence of Cheat Engine by scanning for its icon in running processes. By leveraging the Windows API, this method provides an efficient way to identify Cheat Engine on Windows systems.

## Overview

The detection process focuses on scanning the process icon, a characteristic often overlooked in bypass attempts. This approach offers both reliability and minimal performance impact due to its targeted scanning.

### Pros
- **Fast and Reliable:** The scanning process is highly efficient.
- **Consistent Location:** Scans a specific, consistent location, minimizing performance overhead.

### Cons
- **Privilege Requirements:** Detection may fail if the application lacks equal or higher privileges than Cheat Engine.
  - For example, if the project runs with normal privileges and Cheat Engine runs as an administrator, or if the Cheat Engine process is protected by a kernel driver.

### Note
This detection method is designed to avoid false positives, as it specifically scans the process’s own icon.

## Requirements
- **Operating System:** Windows (due to reliance on the Windows API).

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/YazeedHassanCS/Cheat-Engine-Detection.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Cheat-Engine-Detection
   ```
3. Build the project using your preferred IDE or compiler.

## Usage
- Run the compiled executable to detect Cheat Engine in running processes.

## Limitations
- Requires sufficient privileges to scan processes.
- May not detect Cheat Engine if it has higher privileges. For example, if the project runs with normal privileges and Cheat Engine runs as an administrator, or if the Cheat Engine process is protected by a kernel driver.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or feature suggestions.

## License
This project is licensed under a modified MIT License.
 
### Attribution and Notification Requirement

If you use this project in your software, games, or any other projects, the following conditions must be met:

1. **Attribution**: You must give explicit credit to **0Hikarix** in your project's documentation, about page, or any other publicly accessible materials.

2. **Notification**: You must notify **0Hikarix** upon use of this software in a public project. You can contact **0Hikarix** through:
   - **X (formerly Twitter)**: [@0Hikarix](https://x.com/0hikariX)
   - **Email**: [YazeedHassan@proton.me](mailto:YazeedHassan@proton.me)
   
Failure to provide proper attribution and notification may result in a violation of the licensing terms.

See the [LICENSE](LICENSE) file for complete terms.

## Contact
For questions or support, contact **0Hikarix** on X.


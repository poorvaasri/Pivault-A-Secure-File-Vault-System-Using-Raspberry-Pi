# PiVault: A Secure File Vault System Using Raspberry Pi

## Overview

**PiVault** is a secure and lightweight file vault system designed to operate efficiently on Raspberry Pi devices. Developed in Python with a graphical user interface, PiVault enables users to encrypt, decrypt, and manage sensitive files through a password-protected environment. The system is ideal for personal or small-scale organizational use where data security, portability, and resource efficiency are priorities.

## Project Objectives

The primary goal of PiVault is to provide a reliable, user-friendly solution for local file encryption and storage. Key objectives include:

* Ensuring confidentiality through strong encryption mechanisms
* Maintaining usability with an intuitive desktop interface
* Offering detailed activity logs for traceability
* Providing a secure environment suitable for Raspberry Pi’s limited hardware resources

## Key Features

* **Secure Authentication**
  Implements a password-based login system with secure password hashing and verification.

* **File Encryption and Vaulting**
  Utilizes Fernet symmetric encryption (from the `cryptography` library) to securely encrypt uploaded files. The original file is sanitized with dummy data post-encryption to prevent data recovery.

* **Decryption and Restoration**
  Allows users to decrypt and restore files to a specified location through the GUI.

* **Activity Logging**
  Records all file encryption and decryption events with timestamps to ensure transparency and auditability.

* **User-Friendly Interface**
  Built with `Tkinter` and `ttkthemes` to offer a clean and accessible desktop GUI for all users.

* **Optimized for Raspberry Pi**
  Low memory and processing overhead makes PiVault suitable for Raspberry Pi-based deployments.

## Demonstration

A detailed walkthrough and demonstration of PiVault is available here:
**[Watch the Demo]([https://www.youtube.com/watch?v=your-video-id](https://drive.google.com/file/d/1IRdPkqiWsyBBdFHOof2TX5EKPBc-Iwvg/view?usp=sharing))**

## System Architecture

* **Platform**: Raspberry Pi OS (Linux-based)
* **Programming Language**: Python 3
* **GUI Framework**: Tkinter, ttkthemes
* **Encryption Library**: `cryptography` (Fernet symmetric encryption)
* **File Management**: Encrypted vault directory with original file sanitization

## Installation Guide

### Prerequisites

* Python 3.x installed on Raspberry Pi
* Internet connection to install required packages

### Step-by-Step Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/PiVault.git
   cd PiVault
   ```

2. **Install Required Packages**

   ```bash
   pip install cryptography ttkthemes
   ```

3. **Run the Application**

   ```bash
   python pivault.py
   ```

## Usage

Once launched, the application will prompt for user authentication. Upon successful login, the user can:

* Upload and encrypt new files
* View encrypted files stored in the vault
* Decrypt selected files to a chosen destination
* Access a full activity log for all actions performed
* Logout or exit the application securely

## Security Considerations

* All passwords are stored using secure hashing techniques.
* Files are encrypted using symmetric encryption (Fernet), ensuring strong confidentiality.
* Original files are overwritten post-encryption to prevent data remnants.
* The system maintains local logs for accountability.

## Future Roadmap

Enhancements planned for future iterations include:

* Biometric authentication support (e.g., fingerprint sensors)
* Cloud-based encrypted backups
* Multi-user and role-based access controls
* Advanced vault search and file categorization

## License

This project is created for academic purposes and is open for educational and non-commercial use. For commercial or enterprise deployment, please contact the author.

## Contact & Contribution

Contributions, feedback, and suggestions are welcome. For collaboration or inquiries, please contact:

**Developer**: \[POORVAA SRI B]
**GitHub**: [poorvaasri](https://github.com/poorvaasri)

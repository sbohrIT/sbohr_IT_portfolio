Force USB Encryption - Mac OS X
===========================================================
This AppleScript project is designed to detect and force encryption on external USB drives connected to a Mac. 
The script checks for the presence of a USB drive, determines if it is encrypted with FileVault, and prompts the user to create a password if it is not.

File: force_USB_encrypt.scpt

Context
===========================================================
This project was initiated in response to a critical security concern within our organization. 
The widespread use of unmanaged and unencrypted USB drives by employees posed a significant risk to sensitive company information.

***Problem Statement:***
Unencrypted USB drives were being used to store sensitive data, leaving it vulnerable to unauthorized access.
Lack of ownership identification made it difficult to return lost assets, further exacerbating the security risks.

***Project Objective:***
The primary goal of this project is to develop a solution that forces FileVault encryption on any USB drive inserted into enterprise MacBook devices, while also facilitating the return of lost assets.

***By achieving this objective, I aimed to:***
 - Protect sensitive company information from unauthorized access.
 - Ensure compliance with organizational security policies.
 - Streamline the process of returning lost assets, reducing downtime and associated costs.
 - This project addresses a critical security gap and demonstrates our commitment to protecting sensitive information and maintaining the highest standards of data security.

Features
===========================================================
- Detects external USB drives connected to the Mac
- Checks if the USB drive is encrypted with FileVault
- Prompts the user to create a password if the drive is not encrypted
- Encrypts the USB drive with FileVault using the provided password
- Renames the USB drive to match the current username in order to identity owner

Requirements
===========================================================
- Mac OS X 10.9 or later
- AppleScript Editor (built-in)
- Terminal app (built-in)

Installation
===========================================================
- Save the script as an AppleScript file (.scpt) in the ~/Library/Scripts directory.
- Create a new folder action by going to System Preferences > Automator > Folder Actions.
- Select the script from the list of available scripts and click "Add".
- Configure the folder action to run when a USB drive is inserted.

Usage
===========================================================
- Insert a USB drive into your Mac.
- The script will automatically detect the drive and prompt you to create a password if it is not encrypted.
- Enter a password and click "Continue" to encrypt the drive.
- The script will rename the drive to match your current username.

Troubleshooting
===========================================================
- If the script does not detect the USB drive, ensure that the drive is properly connected and configured.
- If the script fails to encrypt the drive, check the Terminal output for errors and try again.
- If you encounter any issues with the script, feel free to open an issue on this repository.

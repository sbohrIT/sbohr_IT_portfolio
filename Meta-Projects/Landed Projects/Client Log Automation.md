# macOS Client Log Automation Script

A robust automation script designed to collect critical system and application logs from macOS devices, optimized for enterprise-scale deployment. Its purpose is to simplify the log gathering process for critical logs needed for helpdesk escalations to Client Platform Engineering.

## Overview

This script automates the collection of diagnostic logs and system information from macOS endpoints, including:
- System diagnostics via `sysdiagnose`
- Chef client logs and configuration data
- Cyberhaven security logs
- Custom CPE (Common Platform Engineering) logs

Deployed to 30,000+ MacBooks worldwide through Chef, this script demonstrates large-scale log management capabilities for enterprise environments.

## Key Features

- **Root Access Verification**: Self-elevates privileges when required
- **User Notification**: Desktop alerts using Facebook's Notifier Functionality
  ![Image description](![Image description](./images/image_name.png)
- **Log Collection**:
  - System diagnostics bundle
  - Chef client run logs
  - Security software diagnostics
  - Custom application logs
- **Data Packaging**:
  - Automatic ZIP compression
  - Size-optimized storage
  - Unique filename generation (timestamp + serial number)
- **Secure Upload**:
  - Direct upload to internal cloud storage (platform used at Meta for code review, code browsing, and code collaboration)
    
## Deployment

**Scale**: Deployed to 30,000+ global MacBooks via Chef  
**Management**: Integrated with Chef configuration management platform  
**Execution**: Runs as part of routine system maintenance policies

## Usage
This script is used to collect appropriate logs from client macOS devices to include in Client Platform Engineering escalations.

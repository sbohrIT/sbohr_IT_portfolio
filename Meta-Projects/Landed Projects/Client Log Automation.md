# macOS CPE Log Automation Script

A robust automation script designed to collect critical system and application logs from macOS devices, optimized for enterprise-scale deployment using Chef configuration management.

## Overview

This script automates the collection of diagnostic logs and system information from macOS endpoints, including:
- System diagnostics via `sysdiagnose`
- Chef client logs and configuration data
- Cyberhaven security logs
- Custom CPE (Common Platform Enumeration) logs

Deployed to 30,000+ MacBooks worldwide through Chef, this script demonstrates large-scale log management capabilities for enterprise environments.

## Key Features

- **Root Access Verification**: Self-elevates privileges when required
- **User Notification**: Desktop alerts using Facebook's Notifier
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
  - Direct upload to internal Phabricator repository
  - JFrog CLI integration

## Deployment

**Scale**: Deployed to 30,000+ global MacBooks via Chef  
**Management**: Integrated with Chef configuration management platform  
**Execution**: Runs as part of routine system maintenance policies

## Prerequisites

- macOS 10.15+ (Catalina)
- Root access privileges
- Chef client 15+
- Cyberhaven security suite
- Required directories:
  - `/opt/facebook/bin/notifier`
  - `/opt/chef-solo/cpe_init/`
  - `/Applications/Cyberhaven.app/`

## Usage

```bash
# Manual execution (typically deployed via Chef)
sudo ./log_collector.sh

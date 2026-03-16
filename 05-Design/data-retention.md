# Data Retention

## Firmware and Running-Configs

Quatrerly or after every major change all infreastructure configs should be backed up. 

At least two firmware versions should be on file, the previous production for rollbacks and the current production firmware. 

## 321 Rule
Data should be saved on a local drive, a local cloud, and a remote cloud. 

This could the the production copy on the machine if it can be retrieved, one on the local Nextcloud instance, and one on a remote cloud, for example a Google Drive or Sharepoint account.

*If it cannot be retrieved from prod have an admin PC store it locally, ensure it doesn't go with that employee. This is a workaround.*

## Telemtry
All logs and telemetry should be archived for at least three days, up to a week if storage permits. 

Reports should be exported and saved externally from monitoring systems every week to a month, and kept for a year. 

#

Backups will be stored on Nextcloud. 

Telemetry will be housed on the same server inside the monitoring service's dedicated volume. 
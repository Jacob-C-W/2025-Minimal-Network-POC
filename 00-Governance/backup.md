# 3-2-1 Rule

• The 3-2-1 backup rule is a common industry standard for enterprise and consumer data retention plans. It's simple. 

#

- 3 saved versions
- 2 on different media
- 1 offsite

#

The strategy is even simpler in practice: 

A production or first save. A backup on a local network cloud. Finally, a backup on someone else's cloud. 

Example, I have a running configuration on my firewall, I have a backup file on the internal cloud (Nextcloud), and I have two backups saved to an external cloud one in the original file type and another in utf-8. 

This may sound like four, but the point is I have a different file type stored in case one deppreciates on modern hardware/software. 

#

Data retention is balenced between needs and capability.  

After any major configuration change the backup should be updated, or should occur at least quarterly-with automated weekly or monthly being preferred. 

Telemetry should be saved for at least three days to a week to ensure data is logged for recovery, troubleshooting, and future policy. 

Reporting should occur weekly to monthly and then be saved for at least a year. 

#

**sources:**
[What is a 3-2-1 Backup Strategy?](https://www.seagate.com/blog/what-is-a-3-2-1-backup-strategy/),[Backup Policy](C:\Users\jwilliams\Documents\Git\JPF-EAC\00-governance\foundation\policy\backup-policy.md), [Me](https://github.com/Jacob-C-W)
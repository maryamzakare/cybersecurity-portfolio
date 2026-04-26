# My Linux Permissions Lab

## What This Project Is About

This project was a Linux system administration and security lab focused on user accounts, groups, home directories, file permissions, and least privilege access control.

The lab scenario involved a company called TulTech Industries, where improper permissions had previously caused sensitive information to be exposed. The goal was to configure permissions correctly and avoid "wide open" access.

## Why I Made It

Linux permissions are important for cybersecurity because a small permission mistake can expose private files, allow unauthorized changes, or create privilege risks.

This lab helped me practice secure configuration from the command line.

## What I Worked On

- Creating Linux users
- Creating Linux groups
- Managing normal users and administrator users
- Configuring home directory permissions
- Setting ownership with users and groups
- Applying least privilege
- Using sudo for administrative tasks
- Configuring collaborative directories safely
- Testing access as different users

## Security Scenario

The lab focused on preventing insecure permissions such as:

```text
777
ugo+rwx

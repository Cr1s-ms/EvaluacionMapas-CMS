# Vulnerabilities Report

## Summary
- Total vulnerabilities found: 4
- High: 2
- Medium: 2

## Details Finding

### 1.- App can be installed on a vulnerable upatched Android version Android 7.0, [minSdk=24]

- Description: This application can be installed on an older version of android that has multiple unfixed
  vulnerabilities. These devices won't receive reasonable security updates from Google.
  Support an Android version => 10, API 29 to receive reasonable security updates.
- Severity: High
- Impact: Elevation of Privilege (EoP), Stagefright vulnerability, Remote Code Execution (RCE):.
- Remediaton: Update to a Supported Android Version, Restrict App Installation on Older Versions, Apply Available Security Patches

### 2.- Debug Enabled For App[android:debuggable=true]

- Description: Debugging was enabled on the app which makes it easier for reverse engineers to hook
  a debugger to it. This allows dumping a stack trace and accessing debugging helper
  classes.
- Severity: High
- Impact: Exposure of Application Code and Logic, Access to Sensitive Data, Execution of Arbitrary Commands, Network Traffic Analysis.
- Remediaton: Disable Debugging in Production Builds, Remove Debugging Code and Logs, Use Secure Network Practices

### 3.- Application Data can be Backed up [android:allowBackup=true]

- Description: This flag allows anyone to backup your application data via adb. It allows users who
  have enabled USB debugging to copy application data off of the device.
  classes.
- Severity: Medium
- Impact: Automatic Backups, Security Concern, Data Restoration.
- Remediaton: Disable Backup if Necessary, Implement Encryption, Control Backup Content.

### 4.- Broadcast Receiver (androidx.profileinstaller.ProfileInstallReceiver) is Protected by a permission, but the protection level of the permission should be
checked. Permission: android.permission.DUMP [android:exported=true]

- Description: A Broadcast Receiver is found to be shared with other apps on the device therefore
  leaving it accessible to any other application on the device. It is protected by a
  permission which is not defined in the analysed application. As a result, the protection
  level of the permission should be checked where it is defined. If it is set to normal or
  dangerous, a malicious application can request and obtain the permission and interact
  with the component. If it is set to signature, only applications signed with the same
  certificate can obtain the permission.
- Severity: Medium
- Impact: Security Risks, Misuse of Permissions, Data Restoration, Protected by Permission.
- Remediaton: Remove or Limit Permissions, Check Dependencies, Implement Local Broadcasts.




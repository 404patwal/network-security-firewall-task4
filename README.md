# Internship Task 4 — Firewall Configuration and Testing

**Analyst:** Avinash Patwal  
**Date:** 26-Sep-2025  
**Task:** Setup and Use a Firewall (Block Telnet Port 23, Verify, and Restore)

---

## 1. Objective
The objective of this task was to configure and test Windows Defender Firewall to block inbound traffic on **Telnet (TCP port 23)**, verify the rule’s effectiveness, and then restore the firewall to its original state. Evidence was collected at each step.

---

## 2. Environment
- Operating System: Windows 10 Pro  
- Tool: PowerShell + Windows Defender Firewall with Advanced Security  

---

## 3. Steps Performed

### Step 1: Listed Current Inbound Rules
Command:
```powershell
Get-NetFirewallRule -Direction Inbound | Select-Object DisplayName, Enabled, Action, Profile


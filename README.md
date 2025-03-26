# Windows-10-11-Activation-Guide
This document provides two methods to activate Windows 10 and 11 in under 40 seconds, compatible with Home, Professional, Education, and Enterprise editions.

# Cautions
**Legality:** These methods bypass Microsoft’s official licensing, potentially violating terms of service and constituting piracy unless you own a valid license.
**Security:**
**PowerShell Method:** Scripts from https://get.activated.win (linked to Microsoft Activation Scripts) may pose risks if compromised. Verify via GitHub: https://github.com/massgravel/Microsoft-Activation-Scripts.
**CMD Method:** Third-party KMS servers (e.g., kms8.msguides.com) could log your IP or introduce vulnerabilities.
## Antivirus may flag these actions.
**Stability:** Unofficial activations may fail after updates or be detected as "non-genuine" by Microsoft.
**Recommendation: **Use only for educational purposes (e.g., in a VM) or troubleshooting with a valid license. Purchase a legitimate key for production use.
**Disclaimer:** Proceed at your own risk; the author is not liable for any issues.

# Notes
## Ensure an internet connection (VPN not required).
**Backup your system before proceeding, especially in production environments.**

## Table of Contents  
1. [Method 1: PowerShell Activation](#method-1-powershell-activation)  
2. [Method 2: Command Prompt Activation](#method-2-command-prompt-activation)  
3. [Cautions](#cautions)  

---

## Method 1: PowerShell Activation  
Activate Windows quickly using PowerShell with administrative privileges.  

```powershell
# Open PowerShell as Administrator and run:
irm https://get.activated.win | iex

After running, select option [1] from the menu and wait a few seconds. Check activation status in **Settings → Update & Security → Activation**.
---

## Method 2: Command Prompt Activation
Manually activate Windows using Command Prompt with KMS keys and server.

```powershell
# Step 1: Open CMD as Administrator and install a KMS client key
slmgr /ipk yourlicensekey

# Step 2: Set KMS server
slmgr /skms kms8.msguides.com

# Step 3: Activate Windows
slmgr /ato


Replace yourlicensekey with the appropriate key from the list below:

Home: TX9XD-98N7V-6WMQ6-BX7FG-H8Q99
Home N: 3KHY7-WNT83-DGQKR-F7HPR-844BM
Home Single Language: 7HNRX-D7KGG-3K4RQ-4WPJ4-YTDFH
Home Country Specific: PVMJN-6DFY6-9CCP6-7BKTT-D3WVR
Professional: W269N-WFGWX-YVC9B-4J6C9-T83GX
Professional N: MH37W-N47XK-V7XM9-C7227-GCQG9
Education: NW6C2-QMPVW-D7KKK-3GKT6-VCFB2
Education N: 2WH4N-8QGBV-H22JP-CT43Q-MDWWJ
Enterprise: NPPR9-FWDCX-D2C8J-H872K-2YT43
Enterprise N: DPH2V-TTNVB-4X9Q3-TJR4H-KHJW4
Check activation status in **Settings → Update & Security → Activation**.

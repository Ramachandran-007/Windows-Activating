```markdown
# 💻 Windows 10/11 Activation Guide (Unofficial) 🔑

**⚠️ Disclaimer:** This guide provides methods for activating Windows 10 and 11. These methods may bypass Microsoft's official licensing and could potentially violate their terms of service. Use these methods at your own risk. The author is not responsible for any consequences arising from their use. It is strongly recommended to purchase a legitimate Windows license for production environments. This guide is provided for educational purposes or troubleshooting in a virtual machine environment with a valid license.

**🚨 Important Cautions:**

* **Legality:** Activating Windows without a valid license may be considered piracy. 🏴‍☠️
* **Security:**
    * PowerShell scripts may pose security risks if obtained from untrusted sources. Always verify the source (e.g., GitHub). 🛡️
    * Third-party KMS servers can potentially log your IP address or introduce vulnerabilities. 🕵️
* **Antivirus:** Your antivirus software may flag these activation methods. 🚨
* **Stability:** Unofficial activations may become invalid after Windows updates or be detected as "non-genuine" by Microsoft. 🛠️
* **Recommendation:** Use these methods only for educational purposes (e.g., in a virtual machine) or troubleshooting with a valid license. 🎓

**📝 Notes:**

* An active internet connection is required. A VPN is generally not needed. 🌐
* It is highly recommended to back up your system before proceeding, especially in production environments. 💾

## 📑 Table of Contents

1.  [Method 1: PowerShell Activation](#method-1-powershell-activation) 🚀
2.  [Method 2: Command Prompt (CMD) Activation](#method-2-command-prompt-cmd-activation) ⌨️
3.  [Cautions](#cautions) ⚠️

---

## 🚀 Method 1: PowerShell Activation

This method uses a PowerShell script to automate the activation process.

```powershell
# Open PowerShell as Administrator and run:
irm [https://get.activated.win](https://get.activated.win) | iex
```

* After running the command, a menu will appear. Select option `[1]` to activate Windows.
* Wait for the process to complete.
* Check the activation status in `Settings -> Update & Security -> Activation`. ✅
* Verify the source of the script by checking the github repo here: https://github.com/massgravel/Microsoft-Activation-Scripts 📦

---

## ⌨️ Method 2: Command Prompt (CMD) Activation

This method uses the Command Prompt and a KMS server to activate Windows.

```powershell
# Step 1: Open CMD as Administrator and install a KMS client key
slmgr /ipk yourlicensekey

# Step 2: Set KMS server
slmgr /skms kms8.msguides.com

# Step 3: Activate Windows
slmgr /ato
```

Replace `yourlicensekey` with the appropriate key from the following list:

* Home: `TX9XD-98N7V-6WMQ6-BX7FG-H8Q99` 🏠
* Home N: `3KHY7-WNT83-DGQKR-F7HPR-844BM` 🏠
* Home Single Language: `7HNRX-D7KGG-3K4RQ-4WPJ4-YTDFH` 🗣️
* Home Country Specific: `PVMJN-6DFY6-9CCP6-7BKTT-D3WVR` 🗺️
* Professional: `W269N-WFGWX-YVC9B-4J6C9-T83GX` 💼
* Professional N: `MH37W-N47XK-V7XM9-C7227-GCQG9` 💼
* Education: `NW6C2-QMPVW-D7KKK-3GKT6-VCFB2` 📚
* Education N: `2WH4N-8QGBV-H22JP-CT43Q-MDWWJ` 📚
* Enterprise: `NPPR9-FWDCX-D2C8J-H872K-2YT43` 🏢
* Enterprise N: `DPH2V-TTNVB-4X9Q3-TJR4H-KHJW4` 🏢

* Check the activation status in `Settings -> Update & Security -> Activation`. ✅
```

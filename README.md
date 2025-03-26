Instant Windows 10 & 11 Activation: 40-Second Solution



Activate Windows 10 and 11 in under 40 seconds! This repository provides two methods compatible with Home, Home N, Home Single Language, Home Country Specific, Professional, Education, and Enterprise editions.

Overview
This guide offers two quick methods to activate Windows 10 and 11 without a purchased license key. Both methods use built-in Windows tools (PowerShell or Command Prompt) and require an internet connection.

Method 1 (Recommended): Uses PowerShell for a streamlined, menu-driven activation.
Method 2: Uses Command Prompt with manual key entry and KMS server setup.
Method 1: PowerShell Activation (Recommended)
Step 1: Open PowerShell
Click the Start or Search icon.
Type PowerShell in the search bar.
Right-click Windows PowerShell and select Run as Administrator.
Alternative: Right-click the Start menu, then choose Windows Terminal (Admin) (Windows 11) or Windows PowerShell (Admin) (Windows 10).

<p align="left"> <img src="https://github.com/user-attachments/assets/5a10538a-c8c2-4934-868b-fd8e910f1f9e" width="540px" alt="Search for PowerShell"> </p>
Step 2: Run as Administrator
Ensure PowerShell opens with administrative privileges (look for "Administrator" in the title bar).

<p align="left"> <img src="https://github.com/user-attachments/assets/1f25dd2a-16db-4053-a45c-aac6f8a9e470" width="540px" alt="Run PowerShell as Administrator"> </p>
Step 3: Execute the Activation Script
Copy this command:

powershell

Collapse

Wrap

Copy
irm https://get.activated.win | iex
Paste it into PowerShell (right-click to paste), then press Enter.

Step 4: Select Activation Option
A menu will appear. Type 1 (for HWID activation) and press Enter. Wait a few seconds for the process to complete.

<p align="left"> <img src="https://github.com/user-attachments/assets/0c3689a1-1595-40b3-97e2-041dac423237" width="540px" alt="PowerShell Activation Menu"> </p>
Step 5: Verify Activation
Press Enter to exit the script.
Close PowerShell.
Check activation status: Settings → Update & Security → Activation.
Congratulations! Your Windows is now activated.

Method 2: Command Prompt (CMD) Activation
Note: Requires an internet connection. A VPN is not needed.

Step 1: Open Command Prompt
Click the Start or Search icon.
Type CMD in the search bar.
Right-click Command Prompt and select Run as Administrator.
Alternative: Right-click the Start menu, then select Command Prompt (Admin).

<p align="left"> <img src="https://github.com/user-attachments/assets/88ac970a-f24b-4acc-82c0-f8e7c0b05249" width="480px" alt="Search for CMD"> </p>
Step 2: Install a KMS Client Key
Use the command:

cmd

Collapse

Wrap

Copy
slmgr /ipk yourlicensekey
Replace yourlicensekey with the appropriate key for your Windows edition from the table below:

Windows Edition	License Key
Home	TX9XD-98N7V-6WMQ6-BX7FG-H8Q99
Home N	3KHY7-WNT83-DGQKR-F7HPR-844BM
Home Single Language	7HNRX-D7KGG-3K4RQ-4WPJ4-YTDFH
Home Country Specific	PVMJN-6DFY6-9CCP6-7BKTT-D3WVR
Professional	W269N-WFGWX-YVC9B-4J6C9-T83GX
Professional N	MH37W-N47XK-V7XM9-C7227-GCQG9
Education	NW6C2-QMPVW-D7KKK-3GKT6-VCFB2
Education N	2WH4N-8QGBV-H22JP-CT43Q-MDWWJ
Enterprise	NPPR9-FWDCX-D2C8J-H872K-2YT43
Enterprise N	DPH2V-TTNVB-4X9Q3-TJR4H-KHJW4
Tip: To check your Windows edition, go to Settings → System → About (under "Windows specifications").

<p align="left"> <img src="https://github.com/user-attachments/assets/1b6401e6-7e63-4351-8a92-fa355dfc30cf" width="480px" alt="Install KMS Key"> </p>
Step 3: Set KMS Server
Run this command to connect to a KMS server:

cmd

Collapse

Wrap

Copy
slmgr /skms kms8.msguides.com
<p align="left"> <img src="https://github.com/user-attachments/assets/9d634454-1c59-47da-874e-bfe575288fe6" width="480px" alt="Set KMS Server"> </p>
Step 4: Activate Windows
Execute:

cmd

Collapse

Wrap

Copy
slmgr /ato
Wait for a confirmation message.

<p align="left"> <img src="https://github.com/user-attachments/assets/5e495d42-6ce5-4884-9de2-96a56efb4343" width="480px" alt="Activate Windows"> </p>
Step 5: Verify Activation
Check the status: Settings → Update & Security → Activation.

<p align="left"> <img src="https://github.com/user-attachments/assets/9ca70137-8e2e-4504-a52d-22f41d959bd7" width="480px" alt="Activation Status"> </p>
Done! Your Windows is activated.

Cautions
[!WARNING]

Before proceeding, consider the following risks and legal implications:

Legality:
These methods bypass Microsoft’s official licensing process, which may violate their terms of service.
Using them without owning a valid license could be considered software piracy, potentially leading to legal consequences depending on your region.
Security Risks:
Method 1: Downloading and running scripts from https://get.activated.win (linked to Microsoft Activation Scripts) could expose your system to malware if the source is compromised. Always verify the script’s integrity (e.g., check the GitHub repo: https://github.com/massgravel/Microsoft-Activation-Scripts).
Method 2: Connecting to third-party KMS servers (e.g., kms8.msguides.com) may log your IP or introduce vulnerabilities.
Antivirus software might flag these actions as suspicious.
Stability:
Unofficial activations may fail after Windows updates or if KMS servers go offline.
Microsoft could detect and deactivate your system, marking it as "non-genuine."
Recommendations:
Use these methods only for educational purposes (e.g., in a virtual machine) or if you own a license and are troubleshooting.
For legitimate use, purchase a Windows license from Microsoft or an authorized retailer to ensure security and support.
Disclaimer: The author of this guide is not responsible for any issues arising from the use of these methods. Proceed at your own risk.

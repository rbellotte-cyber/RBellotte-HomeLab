Raspberry Pi OS Bookworm uses NetworkManager.
Verify SSH access before disconnecting a monitor.
Disable Wi-Fi when deploying fixed infrastructure.
Document before making infrastructure changes.
DHCP reservations are not the same thing as static IP configuration.
Always verify which network management system is active before changing network settings.
Verify static IP configuration survives a reboot.
Use pihole -g to verify blocklists are updating correctly.
Verify SSH access before removing local console access.
Document the network before making infrastructure changes.

## Lessons Learned
## Raspberry Pi Imager

Verify before flashing:
	- Hostname
	- Username
	- Password
	- SSH Settings
	- Wi-Fi SSID
	- Wi-Fi Password

A single typo can require reflashing and rebuilding the system.
# Notepad++ Added to PATH (Surface Pro 11)
## Date
	26-06-18

## Problem
	Notepad++ was installed and could be launched directly from:
		C:\Program Files\Notepad++\notepad++.exe
	However, the command:
		where.exe notepad++
	returned:
		INFO: Could not find files for the given pattern(s). and the command:
		notepad++ Lessons-Learned.md was not recognized.

## Troubleshooting Performed
	1. Verified Notepad++ was installed in:
	   C:\Program Files\Notepad++
	2. Verified notepad++.exe existed.
	3. Opened Environment Variables using:
		Win + R
		sysdm.cpl
	4. Navigated to:
		Advanced → Environment Variables
	5. Edited the User PATH variable.
	6. Added:
		C:\Program Files\Notepad++
	7. Restarted PowerShell.
	8. Command still failed.
	9. Reviewed PATH order and moved the Notepad++ entry lower in the list.
	10. Opened a new PowerShell session.

## Resolution
	After adjusting the PATH order and restarting PowerShell, Windows successfully located Notepad++.
	Verification:
		where.exe notepad++
	returned:
		C:\Program Files\Notepad++\notepad++.exe
	The command:
		notepad++ Lessons-Learned.md
	now works from any repository directory.

## Lessons Learned
	* Verify software location before troubleshooting PATH.
	* PATH changes require opening a new terminal session.
	* PATH order can affect command resolution.
	* Test with where.exe before assuming a program is unavailable.
	* Document the fix immediately after solving the problem.
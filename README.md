# 🧪 Installing VirtualBox & Creating a Windows 10 VM on macOS

This lab documents the process of setting up a Windows 10 virtual machine (VM) using VirtualBox on macOS. This environment will serve as a foundation for future cybersecurity labs, such as Kerberos authentication and endpoint testing.

---

## 🧰 Tools Used

- macOS (host machine)
- VirtualBox
- Windows 10 ISO
- VirtualBox Guest Additions

---

## 🧠 Why This Matters

Cybersecurity professionals often need safe, isolated environments to test security tools, perform system triage, and simulate attacks. Building a lab using VirtualBox on macOS proves resourcefulness and platform flexibility.

---

## ✅ Steps Overview

### Step 1: Why Use VirtualBox on macOS?

VirtualBox gives you a safe, cost free environment to test Windows-based tools without touching your actual machine. Perfect for lab work on a Mac.

- [001 - macOS desktop](./001-macos-desktop-before-virtualbox.png)
- [002 - VirtualBox download page](./002-virtualbox-download-page.png)

---

### Step 2: Installing VirtualBox

Downloaded from the official site and installed on macOS without needing to bypass any security prompts.

- [003 - Installer start](./003-virtualbox-installer-start.png)

---

### Step 3: Creating the VM

- VM Name: `Win10-KerberosClient`  
- OS: Windows 10 (64-bit)  
- RAM: 3072 MB  
- Disk: 50 GB (VDI, dynamically allocated)

- [004 - VM creation settings](./004-vm-creation-settings.png)
- [005 - Memory selection](./005-vm-memory-selection.png)
- [006 - Disk size](./006-vm-hard-disk-settings.png)
- [007 - Disk format](./007-vdi-dynamic-disk.png)

---

### Step 4: Mounting the Windows 10 ISO

Used the official Microsoft ISO and attached it under Storage settings in VirtualBox.

- [008 - VM summary](./008-vm-summary-before-iso.png)
- [009 - Storage before ISO mount](./009-vm-storage-before-iso.png)
- [010 - ISO mounted](./010-vm-storage-mounted-iso.png)

---

### Step 5: Installing Windows 10

Followed setup prompts, skipped Microsoft sign-in, created local user `KerberosClient`, and disabled privacy settings for better lab control.

- [011 - VM booting](./011-vm-booting-up.png)
- [012 - Installation progress](./012-windows-install-progress.png)
- [013 - Setup mode choice](./013-windows-setup-mode-choice.png)
- [014 - User creation](./014-windows-local-account-name.png)

---

### Step 6: Installing Guest Additions

Inserted Guest Additions CD, ran the installer, and rebooted the VM for improved screen resolution and usability.

- [015 - Guest Additions mounted](./015-guest-additions-mounted.png)

---

### Step 7: Creating a Snapshot

Took a snapshot of the clean install state for future rollback.  
Snapshot name: **Clean Install - Guest Additions Installed**

- [016 - Snapshot created](./016-vm-snapshot-created.png)

---

## 🧠 Reflection

Setting up this VM gives me a reliable Windows 10 environment to run cybersecurity labs from my Mac. With snapshots, I can safely simulate attacks, test defenses, and break things without risk.

---

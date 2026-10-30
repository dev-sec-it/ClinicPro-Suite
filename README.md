# ClinicPro Enterprise Suite (v2.4.0)

Professional Clinic Management, Electronic Medical Records (EMR), and Patient Registry desktop software suite engineered by DEV SEC IT.

---

## Overview

ClinicPro Enterprise Suite provides healthcare organizations, clinics, and medical practitioners with an enterprise-grade desktop workstation for day-to-day operations:

- **Patient Registry & EMR:** Electronic Medical Records, demographic tracking, chronic condition flags, and consultation dossiers.
- **Appointments & Waiting Lounge:** Real-time token queuing, doctor schedule mapping, and OPD flow control.
- **Doctor & Staff Management:** Departmental assignments, consulting fees, attendance, and HR operations.
- **Pharmacy & POS Billing:** Itemized invoice generation, inventory tracking, medicine dispensaries, and payment reconciliations.
- **Desktop C# Workstation Theme:** Dedicated Windows desktop user interface with WinForms-style menubar, live StatusStrip, keyboard accelerators (F1-F12), and database health monitors.

---

## Technical Specifications

- **Client Engine:** Native Rust (`tao` + `wry` WebView2) desktop container.
- **Production Runtime:** Standalone Next.js production build bundled inside a single executable.
- **Distribution Model:** Single-binary setup installer (`ClinicPro Suite Setup.exe`).
- **Security:** Zero exposed source code, blocked DevTools/inspection shortcuts (`F12`, `Ctrl+Shift+I`), isolated runtime execution in `%LOCALAPPDATA%\DEV_SEC_IT\.clinic_pro_runtime`.
- **Operating System:** Windows 10, Windows 11 (64-bit).

---

## Installation Guide

1. Download or locate `ClinicPro Suite Setup.exe`.
2. Double-click to run the setup installer.
3. Review the license agreement and select the destination directory (defaults to `%LOCALAPPDATA%\Programs\ClinicPro Suite`).
4. Click **Install**. The installer configures:
   - Standalone `clinic_pro.exe`
   - Desktop shortcut with the high-resolution Stethoscope icon
   - Start Menu entry under `DEV SEC IT`
   - Windows Control Panel uninstaller
5. Click **Finish** to automatically launch ClinicPro Enterprise Suite.

---

## Directory Structure

Upon installation, the application runs from a clean, single-binary footprint:

```text
%LOCALAPPDATA%\Programs\ClinicPro Suite\
├── clinic_pro.exe      (Native single executable with embedded runtime)
└── Uninstall.exe       (Clean uninstallation utility)
```

No loose source files, Node modules, or plain text configuration files are exposed in the user-visible program directory.

---

## Support & Enterprise Contact

For inquiries regarding multi-branch cloud sync, customized database integrations, or technical support:

- **Developer:** DEV SEC IT
- **Official Website:** [devsecit.com](https://devsecit.com)
- **Email:** info@devsecit.com
- **Headquarters:** Raiganj, West Bengal, India


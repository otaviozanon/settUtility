# SETT Utility

Download (Powershell as Administrator)
```bash
iwr da.gd/setttt -OutFile ~\Downloads\s.zip
```

A comprehensive **Windows optimization and gaming performance toolkit** — configure a fresh or existing Windows install for maximum gaming performance.

## Overview

- **Hundreds of registry/system tweaks** across 14 categories (Internet, Power, Game Mode, Memory, Services, GPU, Privacy, etc.)
- **Full revert capability** for every optimization applied
- **WPF GUI dashboard** (`SETTDash.exe`) with one-click "Optimize All"
- **Reference tuning profiles** for CPU/GPU undervolting & overclocking (NVIDIA, AMD, Intel)
- **Process Lasso auto-config** with CPU affinity, priority, and IO rules for 120+ processes
- **Windows Update control** to prevent unwanted restarts

## Structure

| Folder | Description |
|---|---|
| `0_KMS/` | Windows/Office activation & Office installer |
| `1_Optimizer/` | Core engine — GUI dashboard, backup tool, custom power plan |
| `2_Configurations/` | Hardware tuning profiles (GPU, CPU, desktop UI, MSI Utility) |
| `3_ProcessLasso/` | Process Lasso installer & auto-generated ruleset generator |
| `4_WindowsUpdateBlocker/` | Sordum's WUB utility (32/64-bit) |

## Quick Start

1. Run `SETTDash.exe`
2. Click **Optimize All** or pick individual categories
3. Import `2_Configurations/` tuning profiles into MSI Afterburner, Nvidia Profile Inspector, etc.
4. Run `3_ProcessLasso/ConfigGenerator.bat` to auto-generate CPU rules

## Requirements

- **Windows 10/11** (64-bit)
- **PowerShell** run as Administrator
- .NET Framework 4.8 (for WPF dashboard)

> **Disclaimer**: Registry and system tweaks can affect stability. Use the built-in **Revert** buttons to restore defaults if needed. Always create a restore point first

# 📑 OTForge Recovery & Portability Toolkit: Release Review

The markdown documentation is fully formatted and ready to upload into your team repository, Wiki, or project README. 
The Primary error
## Your packages/app/package.json file has its "main" execution entry point configured to search for out/main/install.js 
## or an automated setup framework hook, but your bundler compiles everything to out/main/index.js instead.
---

## 🚀 Overview

The **OTForge Portable Recovery Toolkit** is a collection of four production-ready, driver-agnostic PowerShell automation tools designed to resolve monorepo dependency conflicts, permission locks, text signature corruption, and Electron binary resolution exceptions instantly across different host machines.

## 🛠️ Portability Package Specs

Executing the generator block calculates your root workspace dynamically based on where you trigger it:

*   **⚡ Dynamic Paths Inside**: Every script contains internal shielding loops. Whether executed from a child folder or root layout on `C:` or `D:`, the toolkit auto-detects the active workspace context path (`$PSScriptRoot`) and locks the operational execution parameters straight to that drive.
*   **🛡️ Profile Agnostic**: Bypasses hardcoded directory names by dynamically fetching active user attributes (`$env:USERNAME`) and local folder profile directories (`$env:USERPROFILE`), rendering the toolkit completely shareable across your team.
*   **📦 Archive Ready**: The script generates both the unzipped file components (`.\otforge_portable_toolkit\`) and a unified portable compressed zip package (**`.\otforge_portable_toolkit.zip`**) right in your current working directory.

---

## 🗂️ Toolkit Component Registry


| Tool File Name | Target Sub-System | Architectural Actions |
| :--- | :--- | :--- |
| **`01_Universal_Permissions_And_Scrub.ps1`** | File System & Encodings | Strips Read-Only/Hidden system flags, grants full owner ACL privileges, and scrubs hidden text Byte Order Marks (`%EF%BB%BF`) that crash Vite/PostCSS build chains. |
| **`02_Portable_Monorepo_Align.ps1`** | Workspace Configuration | Corrects strict Type Safety issues (`TS18046`), updates compiler parameters, and locks the application entry execution route to `index.js`. |
| **`03_Dynamic_User_Cache_Harvester.ps1`** | Binary Injection Bypass | Locates and harvests the uncorrupted physical `electron.exe` framework binaries directly from the developer's local AppData system cache. |
| **`04_Universal_Clean_Build_And_Launch.ps1`** | Workspace Execution | Hard-purges dirty compiler files, triggers clean workspace package builds natively, and launches the development runtime server. |

---

## 📖 How to Deploy & Run (For Your Team)

To distribute this workspace utility to another developer, zip up the `otforge_portable_toolkit` folder or hand over the generated `.zip` bundle. They can place it anywhere inside their local `otforge` installation on any drive layout.

### Running the Recovery Sequence:
1. Open a PowerShell terminal as an **Administrator**.
2. Navigate into the toolkit directory.
3. Run the scripts sequentially:

```powershell
# Step 1: Fix folder properties, grant user ownership, and scrub bad JSON encodings
& .\01_Universal_Permissions_And_Scrub.ps1

# Step 2: Fix workspace entry points and handle strict TypeScript typings
& .\02_Portable_Monorepo_Align.ps1

# Step 3: Extract physical Electron binaries out of local Windows AppData caches
& .\03_Dynamic_User_Cache_Harvester.ps1

# Step 4: Wipe outdated compiled folders and launch the stable application
& .\04_Universal_Clean_Build_And_Launch.ps1
```

### 🔒 Fail-Safe Shielding
If a developer accidentally triggers the script from an invalid location (such as their `Downloads` folder), the root verification handler will automatically catch the anomaly, block execution with a yellow alert, and protect their computer files from accidental configuration writes.

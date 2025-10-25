# GetInstalledAddons (.NET tool)

[![NuGet](https://img.shields.io/nuget/v/GetInstalledAddons.Tool.svg)](https://www.nuget.org/packages/GetInstalledAddons.Tool)

**GetInstalledAddons** prints the registry entries that Alibre Design uses to register its add‑ons.

| | |
|---|---|
| **Package ID** | `GetInstalledAddons.Tool` |
| **Command**   | `GetInstalledAddons` |
| **Runtime**   | .NET 8+ (Windows only) |
| **License**   | MIT |

---

## Installation

```bash
dotnet tool install --global GetInstalledAddons.Tool
```

---

## Usage

```bash
GetInstalledAddons
```

### Sample output

```text
GetInstalledAddons - Alibre Design Add-Ons Registry Information
Version 1.0.0.0
Target key : HKLM\SOFTWARE\Alibre Design Add-Ons
------------------------------------------------------------
  AlibreIronPythonConsole                : C:\Program Files\AlibreIronPythonConsole\bin
  B17A4532-3F9C-4706-B1E5-2F70CAF2D4A9   : {8f143eee-765e-4c6f-93c9-59e86be6b92a}
  {8f143eee-765e-4c6f-93c9-59e86be6b92a} : T:\4-alibredesign\PluginExampleDX
  AlibreAddOnProjectManager              : T:\_003-ALIBREPROJECTMANAGER\bin\Release\net481
  {C1F5A9E0-8B61-4ACC-9C2F-F1E493426A6D} : C:\Program Files\AlibreToolkit
  AlibreAddonDevWithLINQPadVBPAddin      : T:\_004-ALIBRELINQPADADDON\AlibreAddonDevWithLINQPadVBPAddin\bin\Debug\net8.0
  MeshImportInsideAlibreDesignAddon      : T:\_004-ALIBRELINQPADADDON\MeshImportInsideAlibreDesignAddon\bin\Debug\net8.0

Press any key to exit...
```

---

### Exit codes

| Code | Meaning |
|------|---------|
| `0`  | Success |
| `1`  | Registry key not found |
| `2`  | Unhandled error |

---

## Building from source

```bash
git clone https://github.com/stephensmitchell/GetInstalledAddons.Tool
cd GetInstalledAddons.Tool
dotnet pack -c Release
```

---

© 2025 Stephen Mitchell – Released under the MIT License.

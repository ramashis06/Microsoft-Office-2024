# Microsoft Office 2024 Installation (LTSC / Perpetual Version)

This repository provides guidance and sample files for installing **Microsoft Office 2024 LTSC** (Long Term Servicing Channel) using the official **Office Deployment Tool (ODT)** from Microsoft.


## Requirements

- Windows 10 / 11 (64-bit recommended)
- Valid license key for Office LTSC 2024
- Internet connection (for initial download; offline install possible afterwards)
- Administrator rights

## Step-by-Step Installation Guide

### 1. Download the Office Deployment Tool

Download the latest version from the official Microsoft page:  
→ [Office Deployment Tool](https://www.microsoft.com/en-us/download/details.aspx?id=49117)

Run the downloaded `.exe` file → Extract the contents to a folder (e.g. `C:\ODT\` or `Desktop\Office2024\`).

You will get:
- `setup.exe`
- Sample `configuration-*.xml` files (you can delete them)

### 2. Create your configuration.xml

The easiest way is to use Microsoft's web-based **Office Customization Tool**:

1. Go to: https://config.office.com/deploymentsettings
2. Choose your preferences:
   - **Architecture**: 64-bit (recommended)
   - **Product**: Select "Office LTSC Professional Plus 2024" or "Office LTSC Standard 2024" (volume license editions)
   - **Update channel**: PerpetualVL2024
   - Language: e.g. English (en-us)
   - Choose which apps to include/exclude (optional)
   - Other settings: accept EULA silently, display level minimal, etc.
3. At the bottom → **Export** → Save as `configuration.xml`

Alternative: Manually edit a text file named `configuration.xml` (see example below).

### 3. Download Office files (optional - for offline install)

Open Command Prompt **as Administrator** and navigate to your ODT or Office2024 folder:

```bash
cd C:\ODT or Office2024
setup.exe /download configuration.xml

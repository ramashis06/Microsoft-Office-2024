# Microsoft Office LTSC Professional Plus 2024 (Volume License)

![Office LTSC 2024](https://img.shields.io/badge/Microsoft-Office%20LTSC%202024-red)
![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-blue)
![License](https://img.shields.io/badge/License-Volume%20(KMS%20%2F%20MAK)-green)

## 📌 Overview

This repository provides a **complete, step-by-step guide** for installing  
**Microsoft Office LTSC 2024 (Professional Plus / Standard)** using the official  
**Microsoft Office Deployment Tool (ODT)**.

This project is suitable for:
- System Administrators
- IT Support Engineers
- Network Operations (NOC)
- Software Quality Assurance (SQA) Engineers
- Enterprise & Lab Environments

---

## 🔍 GitHub SEO Keywords

`Office LTSC 2024`, `Office Deployment Tool`, `ODT install Office`,  
`Office LTSC Professional Plus 2024`, `Volume License Office`,  
`KMS MAK Office activation`, `Offline Office Installation`

---


## 📌 Requirements

- Windows 10 / Windows 11 (64-bit recommended)
- Valid **Office LTSC 2024 Volume License Key**
- Internet connection (required for initial download; offline install supported afterward)
- Administrator privileges

---

## 🚀 Step-by-Step Installation Guide

### Step 1: Create Installation Folder

1. Go to **Local Disk (C:)**
2. Create a new folder named:

## C:\Office2024   


---

### Step 2: Download Office Deployment Tool (ODT)

1. Download the latest **Office Deployment Tool** from the official Microsoft website:  
   👉 https://www.microsoft.com/en-us/download/details.aspx?id=49117
2. Save and extract the files into the **`C:\Office2024`** folder.

<div align="center">
  <img src="Picture/Screenshot 2025-12-24 235454.png?raw=true" width="90%" />
</div>

---

### Step 3: Create Configuration File (configuration.xml)

The easiest way is to use Microsoft’s **Office Customization Tool**.

1. Go to:  
   👉 https://config.office.com/deploymentsettings
2. Configure the following options:
   - **Architecture:** 64-bit (Recommended)
   - **Product:**  
     - Office LTSC Professional Plus 2024 **OR**  
     - Office LTSC Standard 2024
   - **Update Channel:** `PerpetualVL2024`
   - **Language:** English (en-us) or your preferred language
   - **Apps:** Include or exclude apps as needed
   - **Installation Options (Optional):**
     - Accept EULA silently
     - Display level: None / Minimal
3. Scroll down and click **Export**
4. Select **Office Open XML Formats**
5. Save the file as:
### configuration.xml   


6. Place the file inside the **`C:\Office2024`** folder.

<div align="center">
  <img src="Picture/Screenshot 2025-12-24 225605.png?raw=true" width="90%" />
  <img src="Picture/Screenshot 2025-12-25 000844.png?raw=true" width="90%" />
</div>

---

### Step 4: Extract ODT Files

1. Open the downloaded **Office Deployment Tool (.exe)**
2. Click Mouse Right Button and open "Run as Administrator", select the **`C:\Office2024`** folder
3. This will extract files such as:
   - `setup.exe`
   - `configuration.xml`

<div align="center">
  <img src="Picture/Screenshot 2025-12-25 003108.png?raw=true" width="90%" />
</div>

---

### Step 5: Run Installation via Command Prompt

1. Open **Command Prompt**  
2. Right-click → **Run as Administrator**
3. Navigate to the Office2024 folder:

```cmd
cd C:\Office2024
```

<div align="center"> <img src="Picture/Screenshot 2025-12-25 003657.png?raw=true" width="90%" />

 </div>

### 4: Start the Office installation:


```
setup.exe /configure configuration.xml
```


<div align="center"> <img src="Picture/Screenshot 2025-12-25 004202.png?raw=true" width="90%" />

</div>

### ⏱ Installation Time

Usually takes 10–30 minutes
If silent mode is enabled, no user interaction is required   

### ✅Notes

- Ensure you activate Office using a valid LTSC 2024 volume license key
- You can reuse downloaded files for offline installation
- This method is suitable for enterprise and lab environments












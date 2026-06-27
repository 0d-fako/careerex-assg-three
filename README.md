# 📂 Spreadsheet-to-Drive-to-Email Automation

## Overview
This project demonstrates a **3-step linear automation pipeline** built in **n8n**. The workflow captures client data from a Google Sheet, dynamically creates a Google Drive folder, and sends the client an onboarding email containing the folder link.

The goal is to eliminate manual steps in onboarding by automating:
1. Data capture from a spreadsheet.
2. Resource creation in cloud storage.
3. Communication delivery via email.

--

## Business Scenario
When a new client signs a contract, an account manager logs their info into a Google Sheet. Previously, the manager had to:
- Manually create a folder in Google Drive.
- Copy the folder link.
- Compose and send an onboarding email.

This workflow automates the entire process instantly when a new row is added to the sheet.

---

## Workflow Steps

### Step 1: Google Sheets Trigger
- **Node**: `On Row Added`
- **Data Fields Required**:  
  - `Client Name`  
  - `Company Name`  
  - `Email`
- **Action**: Fires whenever a new row is added.

### Step 2: Google Drive Create Folder
- **Node**: `Create Folder`
- **Dynamic Naming**:  

## Walkthrough Video

You can watch the full demo here:  
[▶️ Loom Video Walkthrough](https://www.loom.com/share/8d2c1afc23a14f42888c361d4b100cb4)
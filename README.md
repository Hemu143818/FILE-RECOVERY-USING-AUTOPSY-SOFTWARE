# FILE-RECOVERY-USING-AUTOPSY-SOFTWARE
## name:- k hemanth yadav
## reg no:- 212224100033
## AIM
To use **Autopsy Digital Forensics Tool** to retrieve deleted files from a disk image.

---

## REQUIREMENTS
- **Operating System**: Windows 10/11, macOS, or Linux
- **Tool**: [Autopsy Digital Forensics](https://www.autopsy.com/)  
- **Test Data**: Disk image file (`disk.dd`, `disk.img`, `.E01`)

---

## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Install Autopsy]
    B --> C[Create New Case in Autopsy]
    C --> D[Add Data Source: Disk Image]
    D --> E["Run File System & Data Recovery Modules"]
    E --> F[Locate Deleted Files in Results]
    F --> G[Recover and Export Deleted Files]
```
## DESIGN STEPS:
### Step 1:
Open Autopsy and create a new case with appropriate case details.

### Step 2:
Add a disk image as a data source and let Autopsy analyze the content.

### Step 3:
Navigate to the "Deleted Files" section in Autopsy and examine or recover the deleted files.

## PROGRAM:
### Install Autopsy
```bash
# Download Autopsy from:
# https://www.autopsy.com/
# Install following the setup wizard.
```
### Create a New Case
```
# File → New Case
# Enter Case Name: Deleted_File_Recovery
# Choose Base Directory: C:\Cases\Deleted_File_Recovery
# Click Finish
```
### Add Disk Image
```
# Add Data Source → Disk Image or VM File
# Browse to: C:\forensics\disk.dd
# Click Next
```
### Run Ingest Modules
```# Select:
# - File System Analysis
# - Keyword Search (optional)
# - Data Recovery / Carving
# Click Finish
```
### Locate Deleted Files
```
# Navigate to 'Deleted Files' section in the tree view
# Review metadata (size, hash, timestamps)
```
### Export Deleted Files
```
# Right-click → Extract File(s)
# Save to: C:\forensics\Recovered_Files\
```

## OUTPUT:
Recovered Deleted File List and Details
<img width="1044" height="931" alt="Screenshot 2025-08-22 091543" src="https://github.com/user-attachments/assets/ff30d718-0957-4864-be0a-793d41ecc382" />
<img width="1919" height="1198" alt="Screenshot 2025-08-22 092145" src="https://github.com/user-attachments/assets/7d8427c3-ca8b-4f72-a659-0960ff003fbf" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 092244" src="https://github.com/user-attachments/assets/623a42b4-75f8-4ba0-a316-2691ecfd4f72" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 092307" src="https://github.com/user-attachments/assets/59794f5d-272f-4acf-8617-9b1a9bad4d4f" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 092340" src="https://github.com/user-attachments/assets/d389fb9a-aa7b-44d9-a02e-3fe6f7036d55" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 092353" src="https://github.com/user-attachments/assets/0c29030d-b4a4-4687-a303-e5c1afc684a5" />
<img width="1918" height="1199" alt="Screenshot 2025-08-22 092410" src="https://github.com/user-attachments/assets/143ba5ee-dc0c-4d48-8f70-4f2793345aac" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 092423" src="https://github.com/user-attachments/assets/a135cce5-9eaa-4ac9-8524-0e254558a00a" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 092435" src="https://github.com/user-attachments/assets/123ac555-f513-45a0-a8a7-fd7b9bfc5a8d" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 092450" src="https://github.com/user-attachments/assets/c879f766-648f-43cc-b8c0-79721f1b11ff" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 092501" src="https://github.com/user-attachments/assets/5c4d8342-d66d-4e06-832b-073f69d34d6c" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 092518" src="https://github.com/user-attachments/assets/46a5ab7b-3f1a-4edd-9168-38c649dabbbe" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 092621" src="https://github.com/user-attachments/assets/bee44b9e-3a35-4347-98ba-41c7bf0ed02b" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 092907" src="https://github.com/user-attachments/assets/82e79a8f-fd8e-4391-976b-e559db662ac0" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 092935" src="https://github.com/user-attachments/assets/ef77521a-1e86-4b97-9e09-6474c4ea0452" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 092948" src="https://github.com/user-attachments/assets/59a2bb7d-6d63-4044-911b-a5e3662f0a84" />
<img width="1018" height="675" alt="Screenshot 2025-08-22 092959" src="https://github.com/user-attachments/assets/b3cd9121-ca37-4492-b9d8-573d011c32c0" />
<img width="956" height="738" alt="Screenshot 2025-08-22 093012" src="https://github.com/user-attachments/assets/f97ad7c6-595a-4dc8-a56d-f1bbde802e45" />
<img width="614" height="418" alt="Screenshot 2025-08-22 093023" src="https://github.com/user-attachments/assets/0d71c412-8683-45db-9802-abd76ea60193" />
<img width="1919" height="1199" alt="Screenshot 2025-08-22 093952" src="https://github.com/user-attachments/assets/52bd68d1-ce63-4dbd-867c-51a33f33758c" />


## RESULT:
Deleted files were successfully retrieved and analyzed using Autopsy.

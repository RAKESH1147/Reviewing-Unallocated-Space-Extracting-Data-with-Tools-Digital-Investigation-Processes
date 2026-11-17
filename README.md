<img width="1913" height="1127" alt="image" src="https://github.com/user-attachments/assets/a277834f-835c-4786-954f-885f77ebb338" /># Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT:
<img width="1917" height="1137" alt="image" src="https://github.com/user-attachments/assets/eef5ad93-c25b-43ff-be71-2d0605487c3f" />

<img width="1917" height="1135" alt="image" src="https://github.com/user-attachments/assets/a6e53f3b-954b-413b-b9d9-48ffc3658400" />

<img width="1917" height="1138" alt="image" src="https://github.com/user-attachments/assets/ecd49417-5da6-4257-b5ff-7b949fff1f15" />

<img width="1913" height="1127" alt="image" src="https://github.com/user-attachments/assets/189bb5e3-555c-49cb-abf6-1d3b5d7d6c1a" />

<img width="1917" height="1135" alt="image" src="https://github.com/user-attachments/assets/6b1efc19-8f67-43ff-a6ef-0b6eb74ca436" />

<img width="1917" height="1132" alt="image" src="https://github.com/user-attachments/assets/70f8dcac-7921-467a-baec-480464541d2e" />

<img width="1917" height="1127" alt="image" src="https://github.com/user-attachments/assets/7f62a690-ac77-46b9-ad84-b196975afc65" />

<img width="1917" height="1143" alt="image" src="https://github.com/user-attachments/assets/16443d93-4df0-4c78-bf29-e3edba516be9" />

<img width="1917" height="1150" alt="image" src="https://github.com/user-attachments/assets/6322bdd5-183a-4fb1-a338-0816364a97b5" />

<img width="1917" height="1136" alt="image" src="https://github.com/user-attachments/assets/53e8f936-8612-4a7e-86ae-b82f189d0b34" />

<img width="1917" height="1150" alt="image" src="https://github.com/user-attachments/assets/231cdab2-30f4-44a5-877c-bea65417ee72" />



Unallocated Space Analysis and Extracted Data Report

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.


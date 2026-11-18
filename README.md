
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

<img width="1917" height="1143" alt="image" src="https://github.com/user-attachments/assets/16443d93-4df0-4c78-bf29-e3edba516be9" />

<img width="1917" height="1150" alt="image" src="https://github.com/user-attachments/assets/6322bdd5-183a-4fb1-a338-0816364a97b5" />

<img width="1917" height="1136" alt="image" src="https://github.com/user-attachments/assets/53e8f936-8612-4a7e-86ae-b82f189d0b34" />

<img width="1916" height="1150" alt="image" src="https://github.com/user-attachments/assets/22a30089-4c67-4267-b6b7-b37c59468f2e" />

<img width="1911" height="1130" alt="image" src="https://github.com/user-attachments/assets/73eac9ad-d85c-4232-a301-875598c63579" />

<img width="1917" height="1135" alt="image" src="https://github.com/user-attachments/assets/169fbc8d-79e0-4cbd-8175-1e37183803a1" />

<img width="1917" height="1140" alt="image" src="https://github.com/user-attachments/assets/da003f81-dbd4-49aa-b8e4-c08477419758" />

<img width="1917" height="1141" alt="image" src="https://github.com/user-attachments/assets/8e778b1c-1eeb-40dd-84e5-c2586814f0fe" />

<img width="1917" height="1133" alt="image" src="https://github.com/user-attachments/assets/beecbb56-78ad-471d-9857-2917b8c2797d" />

<img width="1917" height="1138" alt="image" src="https://github.com/user-attachments/assets/b2c29c0d-b9f7-4988-a7f3-5f0e4829749e" />

<img width="1917" height="1135" alt="image" src="https://github.com/user-attachments/assets/9eff3a05-36fe-4bc8-93e9-69ac7c9600e5" />

<img width="1917" height="1136" alt="image" src="https://github.com/user-attachments/assets/f58affe7-92d7-44ef-8860-6a7a7e26e0fa" />

<img width="1917" height="1137" alt="image" src="https://github.com/user-attachments/assets/0ec5417f-7c77-446c-83db-3b44dd84f401" />

<img width="1917" height="1112" alt="image" src="https://github.com/user-attachments/assets/74ec3024-7f37-445e-a800-31a677994aa1" />

<img width="1917" height="1132" alt="image" src="https://github.com/user-attachments/assets/d6a894d3-d412-46ff-9f05-0279c0dc7077" />

<img width="1917" height="1130" alt="image" src="https://github.com/user-attachments/assets/15e1b743-3a22-4900-99bc-401e8c0ac724" />
<img width="1913" height="1127" alt="image" src="https://github.com/user-attachments/assets/a277834f-835c-4786-954f-885f77ebb338" />Processes
<img width="1917" height="1142" alt="image" src="https://github.com/user-attachments/assets/916f9695-af76-4b96-8c92-53aee3cb1d27" />

<img width="1917" height="1127" alt="image" src="https://github.com/user-attachments/assets/56a54682-e100-429c-b968-9c824277ea0f" />

<img width="1917" height="1135" alt="image" src="https://github.com/user-attachments/assets/13e7f8bb-c721-434d-b8e7-24f00616474b" />

<img width="1917" height="1135" alt="image" src="https://github.com/user-attachments/assets/0d96ca66-5ecd-4c3b-84b6-534e3a3306aa" />

<img width="1917" height="1143" alt="image" src="https://github.com/user-attachments/assets/61ec43d1-6a58-46e4-9af5-be34c73914a8" />

<img width="1917" height="1135" alt="image" src="https://github.com/user-attachments/assets/2eee78fc-4af5-46c3-8b2c-283c39434d15" />

<img width="1917" height="1128" alt="image" src="https://github.com/user-attachments/assets/d3c646da-83e7-4451-8640-4ce84e70e0ad" />

<img width="1917" height="1135" alt="image" src="https://github.com/user-attachments/assets/844e864c-1100-44c4-b3e7-42ea3befcca8" />

<img width="1917" height="1133" alt="image" src="https://github.com/user-attachments/assets/80d91461-d09a-4dea-939d-e4ea89412404" />


Unallocated Space Analysis and Extracted Data Report

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.


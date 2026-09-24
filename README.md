# 🔐 NETWORKWALKS-B083F-Week-3-Password-Cracking-Essentials

This repository contains the documentation, step-by-step task execution, and screenshots for the **Week 3 (Password Cracking Essentials)** practical lab, part of the Cybersecurity and Ethical Hacking program at [Networkwalks Academy](https://networkwalks.com).

---

## 📋 Lab Overview

The primary objective of this lab is to extract cryptographic hashes from protected document formats and crack them using both native application utilities and web-based specialized tools on a Windows environment.

### 🎯 Learning Objectives
* Download, install, and configure local cracking tools (JTR and Johnny GUI).
* Extract valid hash values from encrypted PDF files using remote and local parsers.
* Operate automated cracking tools using graphical user interfaces.
* Execute web-based client-side hashing and cracking routines.
* Verify successful recovery by decrypting secured data elements.

---

## 🛠️ Environment & Tools

The lab execution relies on the following tools and platform links specified in the task sheets:

* **Operating System:** Windows PC / Laptop
* **Applications:** John the Ripper (JTR) & Johnny GUI (`johnny.exe`)
* **Web Services:**
  * [OnlineHashCrack PDF Extractor](https://onlinehashcrack.com)
  * [Networkwalks Hash Calculator](https://networkwalks.comhash-calculator/)
  * [Networkwalks Password Cracker](https://networkwalks.comproject-task-lab-password-cracking-with-networkwalks-tools/)

---

## 🚀 Practical Lab Tasks

### 🔹 TASK 1: Password Cracking with JTR (John the Ripper)
This task focuses on extracting document hashes via an online resource and performing a localized brute-force attack using the standard graphical interface for John the Ripper (Johnny).

#### Step-by-Step Execution:
1. **Tool Setup:** Downloaded and installed the JTR program on the Windows PC, then opened the graphical interface using `johnny.exe`.
2. **Hash Extraction:** Opened the hash website and uploaded the encrypted file `My Locked PDF1.pdf` to the [OnlineHashCrack PDF Hash Extractor](https://onlinehashcrack.com).
3. **Staging:** Selected and copied the generated hash value from the output section. Pasted the hash into Notepad and saved it locally as `hash1.txt`.
4. **Cracking Execution:** 
   * Returned to Johnny GUI and clicked on **'Open password file'**.
   * Browsed to the newly created `hash1.txt` file and selected Open.
   * Clicked on **'Start new attack'** to begin processing the file.
5. **Result Verification:** The tool successfully cracked the PDF file password. 
   * **Cracked Password:** `good-luck`
   * **Validation:** Opened the encrypted PDF file, entered the cracked password `good-luck`, and verified the document successfully unlocked.

#### 📸 Task 1 Evidence & Screenshots
![Johnny GUI Cracking Success](screenshots/johnny_success.png)
![Unlocked PDF Proof](screenshots/pdf1_unlocked.png)



---

### 🔹 TASK 2: Password Cracking with Networkwalks Tools
This task demonstrates an alternative browser-centric method using purely client-side local script processing tools to obtain the hash and crack the password profile on a Windows laptop without external installations.

#### Step-by-Step Execution:
1. **Resource Gathering:** Downloaded the encrypted file `My Locked PDF1.pdf` to the laptop from the official [Networkwalks Lab Page](https://networkwalks.comproject-task-lab-password-cracking-with-networkwalks-tools/).
2. **Local Parsing:** Opened the [Networkwalks Hash Calculator](https://networkwalks.comhash-calculator/) in the web browser and uploaded the locked PDF. The tool locally parsed the file and generated a hash value starting with `$pdf$...`.
3. **Cracking Execution:** Copied the full hash value, pasted it directly into the Networkwalks Password Cracker tool interface, and started the web attack.
4. **Result Verification:** Waited for the tool to finish processing all attempts until the match was found on the screen.
   * **Cracked Password:** `password1`
   * **Validation:** Opened the locked PDF file, entered the cracked password `password1`, and confirmed the PDF file opened successfully. The lab task was completed.

#### 📸 Task 2 Evidence & Screenshots
*(Insert your browser Hash Calculator/Cracker success screenshots and opened PDF proofs below)*
<!-- Place screenshots here -->


---

## 📂 Repository Structure

```text
├── hashes/                # Contains hash1.txt extracted from the documents
├── screenshots/           # Step-by-step visual proofs showing Johnny GUI and Web Cracker outputs
├── documents/             # Sample files (e.g., My Locked PDF1.pdf) used during the lab
└── README.md              # Project documentation file (This file)
```

---

## 📝 Submission Guidelines

To ensure your practical lab is validated by the technical grading team and lead instructor [Waqas Karim (CCIE)](https://linkedin.com), complete the following checklist:

* [ ] Place all required screenshots showing successful hash decryptions inside the `/screenshots` directory.
* [ ] Verify that both recovered keys (**`good-luck`** and **`password1`**) are clearly highlighted in your final submission.
* [ ] Ensure no personal or sensitive data is uploaded along with the test hashes.

---
## ⚖️ Legal & Ethical Disclaimer

*All content, materials, and technical activities within this repository were performed strictly for educational purposes and authorized credential auditing inside lab sandboxes provided by Networkwalks Academy. Unauthorized testing or malicious use of these techniques against external targets without explicit prior written consent is strictly illegal.*

---
⭐️ *Course delivered by [Networkwalks Academy](https://networkwalks.com). If this lab documentation structure was helpful for your grading and studies, please consider dropping a star on this repository!*

# cupid-secret-vault
TryHackMe room write-up: Cupid's Secret Vault – walkthrough, methodology, and learnings.
# Cupid's Secret Vault - TryHackMe Write-up

**Room:** Cupid's Secret Vault  
**Platform:** TryHackMe  
**Difficulty:** Easy/Medium (adjust as per your experience)  
**Author:** Ezzeddine Meskhi  

---

## Objective

The goal of this room is to explore a web-based challenge and understand HTTP requests, headers, and hidden paths.

---

## Walkthrough

### Step 1: Discover the Vault
- Accessed the main URL: `http://10.66.162.218:5000/cupids_secret_vault/`  
- Observed the web page and interesting hints in the source code (like font-family and HTML structure).

### Step 2: Directory Busting
- Used `ffuf` to enumerate directories under `/cupids_secret_vault/`.  
- Found a hidden `administrator` page: `/cupids_secret_vault/administrator`.

### Step 3: Administrator Page
- The administrator page had a login form with `username` and `password` fields.  
- Observed POST requests and tried potential payloads.

### Step 4: Analysis
- Explored HTTP headers, methods, and potential hidden endpoints.  
- Learned about common techniques like header manipulation and brute-force enumeration.

---

## Tools Used

- `curl` for HTTP requests  
- `ffuf` for directory fuzzing  
- Web browser for manual inspection  
- Basic HTML source code analysis

---

## Learnings

- Understanding HTTP headers and methods is critical for web enumeration.  
- Directory busting can reveal hidden endpoints.  
- Analyzing HTML source can provide subtle hints for exploitation.  

---

*This repository contains only the methodology and notes. No flags or sensitive content are included.*

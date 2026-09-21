# NETWORKWALKS-BO83-WK3-PM1-CYBERSECURITY-PASSWORD-CRACKING-WITH-JTR

# Week 3: Password Cracking with John the Ripper and Networkwalks Tools

## Overview
This repository contains documentation, lab notes, and configuration files for the **Week 3 Password Cracking** module. The lab focuses on analyzing credential security, extracting file hashes, and performing dictionary-based attacks using **John the Ripper (Johnny GUI)** and the **Networkwalks Password Cracker** utility[cite: 1, 2, 4].

---

## Tools & Environment
* **John the Ripper / Johnny:** Graphical interface for offline password hash analysis and cracking[cite: 1].
* **Networkwalks Password Cracker:** Web-based simulator for running dictionary attacks against PDF security hashes.
* **WPS Office:** Document viewer used for testing unlocked files and retrieving completion flags[cite: 1, 4].

---

## Lab Execution & Workflow

### Part 1: Offline Cracking with Johnny (John the Ripper)
1. **Target Identification:** Loaded the target PDF file hashes (`$pdf$4*4*128*...`) into Johnny to identify the proper format structure[cite: 1].
2. **Wordlist Attack Configuration:** Set up dictionary-based parameters to cycle through common passwords and phrases.
3. **Execution & Results:** Successfully recovered multiple target passwords (`good-lock`, `password1`, `1qaz2wsx`)[cite: 1, 5, 6].
4. **Flag Validation:** Unlocked the target PDF files to capture module flags[cite: 4]:
   * `nw{cybersecurity_flag_captured_2608}`[cite: 9]
   * `nw{networkwalks_flag_260821_1}`[cite: 8]
   * `nw{networkwalks_persistence_jtr_270521}`[cite: 4]

### Part 2: Online Cracking with Networkwalks
1. **Hash Submission:** Extracted and pasted target PDF hashes into the Networkwalks Password Cracker interface.
2. **Attack Execution:** Deployed the built-in 100-word dictionary list to check matches dynamically.
3. **Verification:** Monitored live feedback status until a positive match (`1qaz2wsx`) was confirmed[cite: 7].

---

## Security Takeaways
* Dictionary attacks highlight the vulnerability of predictable passphrases and human behavioral patterns in choosing keys.
* Implementing strong complexity requirements, long passphrases, and robust salting/hashing algorithms significantly mitigates these risks.

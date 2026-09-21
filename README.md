# NETWORKWALKS-BO83-WK3-PM1-CYBERSECURITY-PASSWORD-CRACKING-WITH-JTR


# Week 3: Password Cracking Lab

Hey everyone! Welcome to my repository for the Week 3 lab. This week, we focused on password cracking techniques, looking closely at how attackers test and break weak credentials using tools like John the Ripper (with the Johnny GUI) and the Networkwalks Password Cracker.

---

## What I Used

* **John the Ripper / Johnny:** The GUI frontend I used to load up PDF hashes and run offline dictionary attacks.


* **Networkwalks Password Cracker:** An online lab tool used to test and match password hashes against wordlists.


* **WPS Office:** What I used to open up the locked PDF files once I figured out the passwords.



---

## How I Did It

### Part 1: Offline Cracking with Johnny

1. First, I loaded the target PDF hash (`$pdf$4*4*128*...`) into Johnny so it could recognize the PDF hash format.


2. I set up a dictionary/wordlist attack to let the tool cycle through common options.
3. After running the attack, I successfully recovered a few passwords like `good-lock`, `password1`, and `1qaz2wsx`.


4. Using those passwords, I opened up the locked files and grabbed my flags:


* `nw{cybersecurity_flag_captured_2608}`

* `nw{networkwalks_flag_260821_1}`

* `nw{networkwalks_persistence_jtr_270521}`




### Part 2: Online Cracking with Networkwalks

1. I copied the PDF hash over to the Networkwalks Password Cracker tool.


2. I selected their built-in wordlist (100 passwords) and kicked off the cracking process.


3. I watched the live logs update until it successfully found a match (`1qaz2wsx`).


4. Finally, I used that password to unlock the document and verify everything worked.



---

## What I Learned

This lab was a great reminder of why strong passwords matter so much. If people use common or predictable words, dictionary attacks can crack them in seconds. Using long passphrases and proper password complexity makes a huge difference!

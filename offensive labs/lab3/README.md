This project demonstrates the methodology for auditing password strength on encrypted files. Faced with a locked ZIP archive, I bypassed the need for manual guessing by converting the file's encryption into a crackable hash format. This lab highlights the speed at which weak passwords can be compromised using dictionary attacks.

Technical Process:

Hash Extraction: Used zip2john to strip the password hash from the encrypted secure.zip file.

Dictionary Attack: Fed the extracted hash into John the Ripper, utilizing the standard rockyou.txt wordlist to automate the cracking process.

Result: Successfully recovered the weak password (pass123) in under a second, decrypted the archive, and retrieved the hidden flag (THM{...}).

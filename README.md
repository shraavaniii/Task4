**COMPANY**: CODTECH IT SOLUTIONS  
**NAME**: SHRAVANI ACHAL HENDRE  
**INTERN ID**: CT08DTU  
**DOMAIN**: CYBERSECURITY AND ETHICAL HACKING  
**BATCH DURATION**: 25th Dec to 25th Jan  
**MENTOR NAME**: NEELA SANTOSH 

**OVERVIEW OF THE PROJECT:**

Key Features:
1. AES-256 Encryption:

Encryption:  
- Utilizes AES (Advanced Encryption Standard) in CBC (Cipher Block Chaining) mode with a 256-bit key.
- Incorporates PKCS7 padding to ensure the plaintext is a multiple of the block size.
- Encrypts files and saves them with a .enc extension.

Decryption:  
- Decrypts previously encrypted files using the same key derivation method.  
- Removes padding after decryption to restore the original plaintext.  
- Saves the decrypted file without the .enc extension.  

2. Key Derivation:
- Uses PBKDF2-HMAC-SHA256 (Password-Based Key Derivation Function 2) to derive a secure encryption key from the user's password.
- Includes a random 16-byte salt for each encryption process to enhance security and prevent rainbow table attacks.
- Performs 100,000 iterations to make brute-force attacks computationally expensive.

4. Initialization Vector (IV):
- Generates a unique 16-byte IV for each encryption operation, ensuring that the same plaintext encrypted multiple times results in different ciphertexts.
- The IV is stored alongside the salt and ciphertext in the encrypted file.

5. Graphical User Interface (GUI):
- Built using Tkinter, providing a simple interface for file selection and password entry.
- Includes buttons for encrypting and decrypting files, enhancing usability for non-technical users.
- Displays success and error messages using message boxes, guiding the user through the process.

6. File Selection:
- Employs a file dialog to allow users to easily select files for encryption or decryption.
- Ensures the selected file path is processed securely and appropriately.

Example Usage:

Encryption:
- The user opens the tool, enters a password, and selects a file to encrypt.
- The tool encrypts the file using AES-256, appends .enc to the file name, and saves it.
- A success message is displayed, confirming the file has been encrypted.

Decryption:
- The user selects an encrypted .enc file and provides the correct password.
- The tool decrypts the file, removes the .enc extension, and saves the original content.
- A success message is displayed, confirming the file has been decrypted.

Security Considerations:
- Strong Encryption: AES-256 is a widely recognized standard for secure encryption, providing a high level of security.
- Secure Key Derivation: The use of PBKDF2 with a salt and multiple iterations significantly enhances the difficulty of brute-force attacks.
- Random Initialization Vector: Ensures the same data produces different encrypted outputs, adding an additional layer of security.

Use Cases:
- Data Protection: Ideal for users needing to securely store or transmit sensitive files.
- User-Friendly Encryption: Provides a straightforward method for encryption and decryption, even for users with minimal technical expertise.
- Portable Security: The GUI-based tool can be used across different systems, making it convenient for various environments.

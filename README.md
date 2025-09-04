# Decrypted-a-classified-file-using-AES-256-CBC-and-OpenSSL-with-PBKDF2-
Decrypted a classified file using AES-256-CBC and OpenSSL with PBKDF2 in a LabEx cybersecurity challenge.

# 🕵️ OpenSSL Decryption Challenge – LabEx

In this beginner-level cybersecurity challenge, I acted as a **cybersecurity analyst** tasked with decrypting a classified file using **OpenSSL**, symmetric encryption, and a known password. This challenge focused on proper **key management** and the application of **AES-256-CBC** decryption with PBKDF2.

---

## 🎯 Challenge Objective

- Decrypt a file (`classified.enc`) using the password: `S3cur3P@ssw0rd!`
- Use the **AES-256-CBC** algorithm with **PBKDF2** key derivation
- Save the output as `decrypted.txt`
- Verify the success of decryption (optionally using checksum)

---

## 🛠️ Lab Environment

- **Directory**: `~/project`
- **Tool**: OpenSSL (CLI)
- **Encryption Scheme**: AES-256-CBC + PBKDF2
- **Password**: `S3cur3P@ssw0rd!`

---

## 🔧 Decryption Command Used

```bash
openssl enc -aes-256-cbc -d -in classified.enc -out decrypted.txt -pbkdf2 -pass pass:S3cur3P@ssw0rd!

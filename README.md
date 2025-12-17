# 🔐 DocuWallet

<div align="center">

![DocuWallet Version](https://img.shields.io/badge/version-4.1.0-blue.svg)
![React Native](https://img.shields.io/badge/React%20Native-0.81.5-61DAFB.svg)
![Expo SDK](https://img.shields.io/badge/Expo-~54.0-000020.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Platform](https://img.shields.io/badge/platform-Android%20%7C%20iOS-lightgrey.svg)

**A secure, offline-first document and credential manager with end-to-end encryption**

</div>

---

## 📖 Overview

DocuWallet is a privacy-focused mobile application that allows you to securely store, manage, and organize your sensitive documents and credentials. Built with a zero-knowledge architecture, your data never leaves your device unless you explicitly create an encrypted backup.

### 🎯 Key Highlights

- **🔒 Military-Grade Encryption**: AES-256 encryption for all stored data
- **🔐 Biometric Authentication**: Face ID, Touch ID, and fingerprint support
- **📴 Offline-First**: Works completely offline - no internet required
- **🗂️ Document Management**: Store ID cards, passports, licenses, and more
- **🔑 Secure Vault**: Password manager for credentials, bank accounts, and sensitive notes
- **📊 Smart Organization**: Categorize documents with custom types and tags
- **💾 Encrypted Backups**: Create password-protected backups with SHA-256 integrity verification
- **🌗 Dark Mode**: Beautiful adaptive UI with light and dark themes

---

## ✨ Features

### 📄 Document Storage
- **Multiple Document Types**: Support for ID cards, passports, driver's licenses, insurance, medical records, and more
- **File Attachments**: Attach PDF and images files to documents
<!-- - **Expiry Tracking**: Get notified before documents expire -->
- **Quick Search**: Fast full-text search across all documents
<!-- - **Batch Operations**: Select and manage multiple documents at once -->
- **PDF Generation**: Export vaults as pdf

### 🔐 Secure Vault
Store sensitive information securely:
- **Passwords & Logins**: Username, password, and security questions
- **Bank Accounts**: Account numbers, IFSC/SWIFT codes, account holder details
- **Credit Cards**: Card numbers, CVV, expiry dates (encrypted)
- **Secure Notes**: Private notes and important information
- **Wi-Fi Passwords**: Network credentials with security type
- **Email Accounts**: Email credentials and recovery information
- **Software Licenses**: License keys and activation codes
- **Web Shortcuts**: Add your favorite web shortcuts

### 🛡️ Security & Privacy
- **Zero-Knowledge Architecture**: Your encryption key never leaves your device
- **Biometric Lock**: Secure app access with Face ID, Touch ID, or fingerprint
- **Auto-Lock**: Configurable timeout when app goes to background
- **Failed Attempt Protection**: Temporary lockout after multiple failed authentications
- **Secure Storage**: Encryption keys stored in device keychain/keystore
- **No Cloud Dependency**: All data stored locally on your device

### 💾 Backup & Restore
- **Encrypted Backups**: Password-protected backups with AES-256 encryption
- **Data Integrity Verification**: SHA-256 checksums ensure backup/restore completeness
- **Flexible Storage**: Save backups to any location using Storage Access Framework (Android 10+)
- **Cross-Device Restore**: Restore your data on any device with your backup file and password
- **Automatic File Handling**: Files are automatically included in backups and restored

### 📊 Statistics & Insights
- **Document Statistics**: Track total documents, expiring items, and categories
- **Visual Overview**: Color-coded statistics for quick insights
- **Expiry Management**: View and manage expired and expiring documents
- **Vault Analytics**: Overview of secure items by type

---

## 🔒 Security

DocuWallet implements multiple layers of security:

### Encryption
- **AES-256-CBC**: Industry-standard encryption for all data
- **Unique Master Key**: Generated on first launch, stored in secure hardware
- **Per-Item Encryption**: Each document and vault item encrypted individually
- **File Encryption**: Attached files encrypted before storage

### Authentication
- **Biometric Authentication**: Support for Face ID, Touch ID, and fingerprint
- **Device PIN/Password**: Fallback to device credentials
- **Failed Attempt Lockout**: Temporary lockout after 5 failed attempts
- **Session Management**: Configurable auto-lock on background

### Privacy
- **Offline-First**: No internet connection required
- **No Analytics**: Zero tracking or telemetry
- **No Third-Party Services**: No external dependencies for core functionality
- **Local Storage Only**: All data stored on device

### Backup Security
- **Password-Protected**: Backups encrypted with separate password
- **Key Derivation**: PBKDF2 key derivation with salt
- **Integrity Verification**: SHA-256 checksums verify data integrity
- **Normalized Checksums**: File paths excluded from verification for portability

---

<!-- ## 🖼️ Screenshots

<div align="center">

| Home Screen | Vault | Document Details | Settings |
|------------|-------|------------------|----------|
| *Document management* | *Secure credentials* | *Encrypted storage* | *Security settings* |

</div>

--- -->

## 🚀 Getting Started (User Guide)

### First Launch
1. **Security Setup**: Enable biometric authentication (recommended)
2. **Master Key Generation**: App automatically generates encryption key
3. **Grant Permissions**: Allow camera and storage access for full functionality

### Adding Documents
1. Tap **+** button on home screen
2. Select document type (Identity, Vehicle, Health, etc.)
3. Fill in details and attach files
4. Save - all data is automatically encrypted

### Using Secure Vault
1. Navigate to **Vault** tab
2. Tap **+** to create new secure item
3. Choose template (Wifi Credential, Email Account, Bank Account, etc.)
4. Enter sensitive information
5. Save - everything is encrypted immediately

### Creating Backups
1. Go to **Settings** → **Backup & Restore**
2. Tap **Create Backup**
3. Enter a strong backup password (min 8 characters)
4. Choose save location
5. Backup file (.docuwallet) is encrypted and verified

### Restoring Backups
1. Go to **Settings** → **Backup & Restore**
2. Tap **Restore from Backup**
3. Select your .docuwallet file
4. Enter backup password
5. Confirm restore (existing data will be replaced)
6. Data integrity is automatically verified

---

## 🔐 Security Best Practices

### For Users
- ✅ Enable biometric authentication
- ✅ Use a strong backup password (different from device PIN)
- ✅ Store backup files in a secure location
- ✅ Regularly update your backups
- ✅ Don't share your device while app is unlocked
- ❌ Never share your backup password

<!-- ### For Developers
- ✅ Never log sensitive data (even in development)
- ✅ Use `__DEV__` checks for debug logs
- ✅ Test encryption/decryption thoroughly
- ✅ Validate all user inputs
- ✅ Handle errors gracefully without exposing details
- ✅ Keep dependencies updated for security patches -->

---

## 👨‍💻 Author

**Anuj Kulal**

- GitHub: [@Anujkulal](https://github.com/Anujkulal)
- Website: [docuwallet.netlify.app](https://docuwallet.netlify.app)

---

## ⚠️ Disclaimer

DocuWallet is designed for personal use to securely store sensitive information. While the app implements industry-standard encryption and security practices, users are responsible for:
- Creating strong backup passwords
- Securing their device with PIN/biometric authentication
- Safely storing backup files
- Understanding the risks of digital data storage

**The developer is not responsible for any data loss, security breaches, or misuse of the application.**

---

<!-- ## 📧 Support

If you encounter any issues or have questions:
- Open an issue on [GitHub Issues](https://github.com/Anujkulal/docuwallet-app-release/issues)
- Check existing issues for solutions
- Provide detailed information (device, OS version, steps to reproduce)

--- -->

<div align="center">

**Made with ❤️ for privacy-conscious users**

⭐ **Star this repo if you find it helpful!** ⭐

</div>

# Secret Encrypter

**Live Demo:** [https://danishsayyad.github.io/Secret-Encrypter/](https://danishsayyad.github.io/Secret-Encrypter/)

A privacy-focused, client-side text encryption and decryption web application. Secret Encrypter allows you to securely encrypt and decrypt text using custom keys, with all data stored locally on your device.

## Screenshots

### Login Page
![Login Page](screenshots/login.png)
*Please add a screenshot of the login page here*

### Encryption Interface
![Encryption Interface](screenshots/encrypt.png)
*Please add a screenshot of the encryption/decryption interface here*

### Stored Texts
![Stored Texts](screenshots/texts.png)
*Please add a screenshot of the texts storage tab here*

## Features

### Security & Privacy
- **100% Client-Side Processing**: All encryption, decryption, and storage happens in your browser
- **No Server Communication**: Your data never leaves your device
- **SHA-256 Password Hashing**: Secure password storage using industry-standard hashing
- **Key-Based Encryption**: Each text requires a unique encryption key
- **Local Storage Only**: All data stored in browser's local storage

### Authentication System
- First-time password setup with confirmation
- Secure login for returning users
- Password visibility toggle for easy verification
- Reset password functionality (clears all stored data)
- Automatic session management

### Encryption & Decryption
- Simple toggle between Encrypt and Decrypt modes
- Custom encryption key support (minimum 4 characters)
- XOR cipher with Base64 encoding
- Real-time text processing
- Clear input/output fields

### Text Storage Management
- Save encrypted texts with custom titles
- View stored texts with inline viewer
- Individual delete functionality for each text
- Wipe All feature to clear entire storage
- Confirmation prompts for destructive actions

## Technology Stack

- **HTML5**: Semantic markup and structure
- **CSS3**: Modern styling with animations and transitions
- **Vanilla JavaScript**: No frameworks, pure DOM manipulation
- **Web Crypto API**: SHA-256 password hashing
- **Local Storage API**: Client-side data persistence

## Project Structure

```
Secret-Encrypter/
├── index.html              # Main application interface
├── pages/
│   ├── login.html          # Authentication page
│   └── about.html          # Project information
├── script/
│   ├── auth.js             # Authentication logic
│   └── app.js              # Core encryption/decryption logic
├── style/
│   ├── main.css            # Home page styling
│   ├── auth.css            # Login page styling
│   └── about.css           # About page styling
├── assets/
│   ├── icon.svg            # High-resolution icon
│   └── icon-small.svg      # Favicon
└── README.md
```

## Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- JavaScript enabled

### Installation & Usage

1. Clone the repository:
```bash
git clone https://github.com/DanishSayyad/Secret-Encrypter.git
```

2. Open `index.html` in your web browser, or visit the [live demo](https://danishsayyad.github.io/Secret-Encrypter/)

3. On first visit, create a master password to protect your encrypted texts

4. Start encrypting and storing your sensitive information!

## How It Works

### First Time Setup
1. Visit the application
2. Create a master password (will be hashed and stored locally)
3. Confirm your password
4. Access the main interface

### Encrypting Text
1. Enter the text you want to encrypt
2. Provide an encryption key (minimum 4 characters)
3. Click "Encrypt"
4. Save the encrypted text with a title for later access

### Decrypting Text
1. Toggle to "Decrypt" mode
2. Paste your encrypted text
3. Enter the same key used for encryption
4. Click "Decrypt" to reveal the original text

### Managing Stored Texts
1. Navigate to the "Texts" tab
2. View all your saved encrypted texts
3. Click "View" to see any stored text
4. Use "Delete" to remove individual texts
5. Use "Wipe All" to clear entire storage

## Security Considerations

- **Master Password**: Your master password is hashed using SHA-256 before storage. However, it's crucial to remember it as there's no recovery mechanism.
- **Encryption Keys**: Keys are NOT stored with encrypted texts. You must remember the key used for each encryption.
- **Local Storage**: Data persists in browser local storage. Clearing browser data will delete all stored information.
- **Encryption Strength**: This application uses XOR cipher, suitable for casual privacy but not for highly sensitive data requiring military-grade encryption.

## Privacy Policy

Secret Encrypter is committed to your privacy:

- Does not collect any personal information
- Does not transmit any data to external servers
- Does not use cookies or tracking
- Does not require internet connection after initial load
- All processing happens entirely in your browser

## Browser Compatibility

- Chrome/Edge 60+
- Firefox 57+
- Safari 11+
- Opera 47+

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/DanishSayyad/Secret-Encrypter/issues).

## Developer

**Danish Sayyad**

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Built with vanilla JavaScript for maximum compatibility
- Designed with privacy and security as top priorities
- Inspired by the need for simple, trustworthy encryption tools

---

**Remember**: This application is designed for casual privacy needs. For highly sensitive information, consider using enterprise-grade encryption solutions.

# PublicSafe

**Your Browser, Your Safe Space**

PublicSafe is a free and open-source browser extension focused on privacy, encryption, and user control. It provides client-side encryption tools designed to help users protect sensitive information before it leaves their browser. PublicSafe is built around transparency, security, accessibility, and community-driven development.

The project follows a privacy-first philosophy with a zero-knowledge design, local key management, and open-source code that can be independently audited by anyone.

## Goals

- Protect user privacy through client-side encryption.
- Give users complete control over their encryption keys.
- Provide simple, user-friendly security tools.
- Remain transparent through open-source development.
- Support modern browsers through a shared codebase.
- Eliminate unnecessary data collection and telemetry.
- Create accessible privacy tools for everyone.

## Features

### Encryption Features

- Client-side encryption before data transmission.
- AES-256-GCM encryption support.
- X25519 key exchange support.
- Ed25519 digital signature support.
- Secure text encryption and decryption.
- Secure note encryption.
- Encrypted message generation.
- Encrypted data sharing tools.
- Secure secret storage utilities.
- Encryption integrity verification.
- SHA-256 hashing utilities.
- Password-based encryption support.
- Key derivation using PBKDF2.
- Argon2id support where available.

### Browser Protection Features

- Browser-integrated encryption tools.
- Form data encryption utilities.
- Secure clipboard encryption and decryption.
- Protection for sensitive browser input.
- Secure copy-and-paste workflows.
- Browser privacy dashboard.
- Security status monitoring.
- Encryption activity indicators.
- Site-level privacy controls.
- Trusted site management.
- Security notifications.

### File Protection Features

- Local file encryption.
- Local file decryption.
- Encrypted file exports.
- Encrypted file imports.
- Secure file sharing preparation.
- Large file encryption support.
- Multiple file processing.
- Integrity verification for encrypted files.

### Key Management Features

- Local key generation.
- Public and private key management.
- Key import and export tools.
- Encrypted key backups.
- Recovery key generation.
- Key rotation support.
- Multiple identity support.
- Secure key storage.

### Privacy Features

- Zero-knowledge architecture.
- No mandatory user accounts.
- No centralized key storage.
- No telemetry.
- No tracking.
- No analytics collection.
- Local-first design.
- User-controlled encryption.
- Transparent security model.
- Open auditability.

### User Experience Features

- One-click setup.
- Guided onboarding.
- Simple encryption workflows.
- Accessibility-focused design.
- Keyboard navigation support.
- Responsive user interface.
- Dark mode support.
- Light mode support.
- User-friendly security indicators.
- Minimal configuration requirements.

### Browser Support

- Google Chrome
- Chromium
- Microsoft Edge
- Mozilla Firefox
- Brave
- Opera
- Vivaldi

### Developer Features

- TypeScript codebase.
- Modular architecture.
- Web Crypto API integration.
- Manifest V3 support.
- Extension API abstraction layer.
- Automated testing.
- Continuous integration support.
- Security-focused development practices.
- Contributor-friendly project structure.
- Comprehensive documentation.

## Technology Stack

### Frontend

- TypeScript
- HTML5
- CSS3
- Web Components
- Manifest V3

### Cryptography

- Web Crypto API
- AES-256-GCM
- X25519
- Ed25519
- SHA-256
- PBKDF2
- Argon2id (where supported)

### Storage

- IndexedDB
- Browser Storage APIs
- Local-first architecture

### Development Tools

- Vite
- ESLint
- Prettier
- Vitest
- Playwright
- GitLab CI/CD

### Documentation

- Markdown
- OpenAPI Specifications
- Automated Documentation Generation

## Security Principles

- Privacy by default.
- Security by design.
- Open-source transparency.
- Zero-knowledge architecture.
- Local key ownership.
- No mandatory cloud services.
- No hidden data collection.
- User-controlled security decisions.
- Publicly auditable codebase.

## Contributing

Contributions, bug reports, feature requests, documentation improvements, accessibility enhancements, and security reviews are welcome.

Please review the project's contributing guidelines before submitting pull requests.

---

## Specification Branding License (SBL)
### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/publicsafe/](https://roxanneardary.com/publicsafe/)

---

## License & Notice Requirements

PublicSafe is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- PublicSafe specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

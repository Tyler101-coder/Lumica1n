# 🔒 Lumica1n

**Lumica1n** is a security-focused Apple Configuration Profile project designed to help strengthen device security using Apple's supported management framework.

> Security hardening for iPhone, iPad, and Mac.

## What is Lumica1n?

Lumica1n provides security-focused `.mobileconfig` profiles that can be installed on supported Apple devices to enforce stronger security settings and best practices.

Unlike jailbreak tools, Lumica1n operates entirely within Apple's supported ecosystem.

## Features

### 🛡️ Strong Passcode Policies

- Enforce complex passcodes
- Minimum password length requirements
- Alphanumeric password support
- Failed-attempt protections
- Password aging policies

### 🔐 Device Security

- Encourage secure device configuration
- Support managed restrictions
- Reduce exposure to common security risks
- Deploy using Apple-approved methods

### 📱 Apple Ecosystem Support

- iPhone
- iPad
- Mac
- Apple Vision Pro (payload dependent)

## Installation

1. Download the desired `.mobileconfig` profile.
2. Open the file on your Apple device.
3. Navigate to **Settings → Profile Downloaded**.
4. Review the profile contents.
5. Tap **Install**.
6. Authenticate when prompted.

## Repository Layout

```text
Lumica1n/
├── README.md
├── LICENSE
├── Profiles/
│   └── Lumica1nSecurity.mobileconfig
└── Assets/
```

## Goals

Lumica1n aims to:

- Improve Apple device security
- Promote security best practices
- Simplify profile deployment
- Remain fully compatible with Apple's security model

## Not a Jailbreak

Lumica1n does **not**:

- Jailbreak devices
- Bypass Activation Lock
- Remove iCloud protection
- Modify iOS or iPadOS system files
- Install unauthorized software
- Circumvent Apple's security mechanisms

## Privacy

Lumica1n:

- Does not collect personal information
- Does not transmit analytics
- Does not access user data
- Does not track device activity

## Verification

Before installing:

- Review the profile contents.
- Verify the repository source.
- Inspect the XML configuration if desired.
- Test on a non-production device.

## License

MIT License

## Disclaimer

Configuration profiles can enforce settings but cannot alter protected operating system behavior. Always review profile contents before installation.

**Lumica1n** is intended to improve security while remaining within Apple's supported configuration profile framework.

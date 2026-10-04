# ⚡ Endpo

**A modern, high-performance, offline-first API development and testing workbench for developers.**

Endpo is a desktop API development tool built with **Tauri, React, and Rust**, designed for developers who want a fast, lightweight, privacy-focused workspace for building, testing, documenting, and managing APIs.

> 🚧 **Early Release**
>
> Endpo is actively under development. Features, UI, and functionality may change between releases. Feedback and bug reports are welcome.

---

## 📌 Current Release

**Version:** `v1.0.1`  
**Status:** Active Development  
**Platforms:** Windows · macOS

For previous versions and detailed release notes, see the project's **GitHub Releases** and `CHANGELOG.md`.

---

## 🔍 What is Endpo?

Endpo is an **offline-first API development and testing desktop application**.

It provides a developer-focused workspace for working with APIs locally while supporting optional cloud synchronization for supported workflows.

### Supported API Technologies

- REST
- GraphQL
- WebSocket
- gRPC
- Server-Sent Events (SSE)

### Core Principles

- ⚡ Fast and lightweight
- 📴 Offline-first
- 🔐 Local-first data
- 🔄 Optional cloud synchronization
- 🛠 Developer-focused workflow
- 🔒 Security-conscious development

---

# ✨ Features

## 🚀 Fast Desktop Experience

Endpo is built using **Rust, Tauri, and React** to provide a modern native desktop experience with a lightweight application architecture.

## 📴 Offline-First

Endpo is designed to work locally without requiring a permanent internet connection.

Your API collections, environments, request history, and supported workspace data can be used locally.

## 🔐 Local Data Protection

Endpo uses local storage for its offline-first workflow.

Where encryption is enabled, local application data is protected using the application's encrypted storage mechanism.

> Security and encryption mechanisms may evolve between releases. Refer to the source code and release documentation for the implementation used by a specific version.

## 🌐 Multi-Protocol API Testing

| Protocol | Support |
|---|---|
| REST | ✅ |
| GraphQL | ✅ |
| WebSocket | ✅ |
| gRPC | ✅ |
| Server-Sent Events | ✅ |

## 🔄 Optional Cloud Synchronization

Cloud synchronization is optional and is designed to support workflows such as:

- Multi-device access
- Team collaboration
- Workspace synchronization
- Cloud-backed workspace workflows

The desktop application is designed around a **local-first workflow**, while synchronization can be enabled when required.

## 📦 Automatic Updates

Endpo supports application updates through its release/update infrastructure.

Release artifacts can be cryptographically signed to provide an additional layer of integrity verification.

---

# 🖥️ Supported Platforms

### Windows

- Windows x64

### macOS

- Apple Silicon
- Intel

Linux support may be introduced in a future release.

---

# 📥 Download

Download Endpo only from the project's official release channels.

### GitHub Releases

The recommended way to obtain Endpo is through the project's official GitHub Releases.

> Always verify that the downloaded version matches the corresponding release before installing.

---

# 🛡️ Security & Trust

Endpo is a developer tool that may be used with API requests, environments, authentication configuration, and other potentially sensitive development data.

For that reason, transparency is an important part of the project.

## 🔎 Source Code Transparency

The repository is publicly available so developers can inspect the application and understand how Endpo works.

Users can review the project's implementation, configuration, dependencies, and release-related files directly from the repository.

> Public source availability is provided for transparency and inspection. It does not mean that the software is open-source or freely licensed for redistribution.

---

## 🔏 Release Signing

Endpo releases may include cryptographic signatures.

The release process uses **Minisign-based signing** where configured to provide an additional mechanism for verifying release artifacts.

A valid signature can help establish that a release artifact corresponds to the expected signed release.

> A valid signature does not guarantee that software is completely free of bugs or vulnerabilities. It verifies the integrity/authenticity of the signed artifact against the project's verification key.

---

# 🧪 Virus & Malware Verification

No software project should ask users to blindly trust an executable.

If you are concerned about a downloaded Endpo release:

### 1. Download from the official source

Use the official GitHub release or officially documented distribution channel.

### 2. Check the version

Make sure the downloaded file corresponds to the intended Endpo release.

### 3. Inspect the source

The project source code is publicly available for inspection.

### 4. Verify the release signature

When signature files are provided, users can verify the release using the project's published Minisign public key.

### 5. Scan the downloaded file

Users may independently scan the installer or application using their preferred security tools.

> Endpo does not claim that any software is completely free from vulnerabilities or malicious behavior. The purpose of source availability and release verification is to make independent evaluation easier.

---

# 🪟 Windows Installation

## Download

Download the latest Windows installer:

```text
Endpo_<version>_x64-setup.exe
```

## Microsoft Defender SmartScreen

Windows may display:

> **Windows protected your PC**

This can occur with applications that have limited or new reputation information with Microsoft SmartScreen.

A SmartScreen warning does **not by itself establish that an application contains malware**.

Before proceeding:

1. Confirm that the installer came from the official release source.
2. Verify the version.
3. Review the release information.
4. If Windows shows the warning, select **More info** to inspect the application details.

> Do not bypass security warnings for installers obtained from unknown or unofficial sources.

---

# 🍎 macOS Installation

Download the appropriate Endpo release for your Mac:

```text
Endpo_<version>_aarch64.dmg
```

or the Intel build when provided.

## Install

1. Open the `.dmg` file.
2. Drag **Endpo.app** into the **Applications** folder.
3. Launch Endpo.

## macOS Gatekeeper

macOS may display a message such as:

> "Cannot be opened because the developer cannot be verified."

This can occur when an application downloaded from the internet has not been recognized by Apple's Gatekeeper/reputation system.

If you have verified that the application came from the official release source:

### Method 1 — Finder

1. Open **Applications**.
2. Right-click **Endpo.app**.
3. Select **Open**.
4. Review the security prompt.
5. Select **Open** if you trust the verified release.

### Method 2 — Privacy & Security

1. Attempt to launch Endpo.
2. Open **System Settings**.
3. Go to **Privacy & Security**.
4. Review the security message.
5. Use **Open Anyway** if you have verified the release.

> Avoid disabling macOS security protections for applications downloaded from unknown sources.

---

# 🔐 Privacy

Endpo follows a **local-first** approach.

The basic API development workflow is designed to operate locally.

Depending on the features you use, information may remain on your device or may be synchronized through configured cloud functionality.

Potentially sensitive development information may include:

- API requests
- API responses
- Collections
- Environments
- Headers
- Authentication configuration
- Request history
- Workspace data

Users should avoid storing production credentials or sensitive secrets unless they understand how and where that information is stored.

---

# ☁️ Local-First & Cloud Sync

Endpo is designed around the following high-level concept:

```text
        Endpo Desktop
              │
              ▼
       Local Workspace
              │
       ┌──────┴──────┐
       │             │
    Offline       Optional
     Usage        Cloud Sync
```

The local workspace is designed to remain useful without requiring constant cloud connectivity.

Cloud synchronization is an optional capability for supported workflows.

> Internal synchronization mechanisms, database schemas, and backend implementation details are intentionally not documented in the public README.

---

# 🧰 Built With

Endpo is built using modern desktop and web technologies:

- **Tauri** — Desktop application framework
- **Rust** — Native application layer
- **React** — User interface
- **TypeScript** — Frontend development
- **SQLite** — Local-first storage
- **PostgreSQL** — Cloud synchronization storage

The exact implementation may evolve between releases.



# 🐛 Report a Bug

Found a problem?

Please open a GitHub Issue and include:

- Endpo version
- Operating system
- Architecture
- Steps to reproduce
- Expected behavior
- Actual behavior
- Relevant logs
- Screenshots, if useful

### ⚠️ Never include sensitive information

Do not publish:

- API keys
- Passwords
- Access tokens
- Private URLs
- Database credentials
- Production secrets
- Personal or confidential data

in a public issue.

---

# 💡 Feature Requests

Have an idea for Endpo?

Open a feature request and explain:

- What problem the feature solves
- Why it would be useful
- How you expect it to work
- Any relevant examples

Community feedback helps shape future versions of Endpo.

---

# 💬 Discussions & Community Feedback

GitHub Issues and Discussions can be used for:

- Questions
- Bug reports
- Feature requests
- Product feedback
- Improvement suggestions
- Release discussions

The project aims to make Endpo easier to evaluate, test, and improve through public feedback.

---

# 🔒 Security Vulnerabilities

If you discover a potential security vulnerability, please **do not publicly disclose sensitive exploit details in a GitHub Issue**.

Use the project's private security reporting mechanism when available.

A useful security report should include:

- Affected version
- Vulnerability description
- Reproduction steps
- Potential impact
- Suggested mitigation, if available

---

# 📦 Releases

Each Endpo release may contain platform-specific application packages and release metadata.

Typical releases may include:

```text
Windows
├── Endpo_<version>_x64-setup.exe
└── Release verification files

macOS
├── Endpo_<version>_aarch64.dmg
├── Endpo_<version>_x64.dmg
└── Release verification files
```

For complete release information, use the corresponding GitHub Release.

---

# 📋 Changelog

Release-specific changes are documented separately in:

```text
CHANGELOG.md
```

The changelog should contain:

- New features
- Improvements
- Bug fixes
- Breaking changes
- Security-related changes
- Known issues

---

# 📄 License

Endpo is **proprietary software**.

The source repository may be publicly visible for transparency, inspection, feedback, and development purposes.

Public source visibility does **not** grant permission to:

- Redistribute Endpo
- Sell Endpo
- Rebrand Endpo
- Modify and redistribute Endpo
- Use Endpo commercially outside the applicable license terms

See the repository's `LICENSE` file for the complete terms.

---

# ⭐ Why Endpo?

Endpo is built around a simple idea:

> **API development should be fast, local, transparent, and developer-friendly.**

Endpo combines a lightweight desktop experience with an offline-first workflow and optional cloud capabilities.

If you are interested in the project:

**Inspect it. Try it. Test it. Report issues. Share feedback.**

---

# 📌 Project Status

**Active Development**

Endpo is continuously evolving. Some features may be experimental or incomplete.

For the latest information, check:

- GitHub Releases
- Issues
- Discussions
- Changelog
- Repository commits

---

**Built with ❤️ using Rust, Tauri, and React.**

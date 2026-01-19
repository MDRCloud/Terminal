# MDRCloud Terminal

[![MDRCloud](https://img.shields.io/badge/MDRCloud-Terminal-3B4A98?style=flat-square&logo=cloud&logoColor=white)](#)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](#)

> **Based on [Termix](https://github.com/Termix-SSH/Termix)** - An open-source SSH terminal and server management platform

#### Top Technologies

[![React Badge](https://img.shields.io/badge/-React-61DBFB?style=flat-square&labelColor=black&logo=react&logoColor=61DBFB)](#)
[![TypeScript Badge](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&labelColor=black&logo=typescript&logoColor=3178C6)](#)
[![Node.js Badge](https://img.shields.io/badge/-Node.js-3C873A?style=flat-square&labelColor=black&logo=node.js&logoColor=3C873A)](#)
[![Vite Badge](https://img.shields.io/badge/-Vite-646CFF?style=flat-square&labelColor=black&logo=vite&logoColor=646CFF)](#)
[![Tailwind CSS Badge](https://img.shields.io/badge/-TailwindCSS-38B2AC?style=flat-square&labelColor=black&logo=tailwindcss&logoColor=38B2AC)](#)
[![Docker Badge](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&labelColor=black&logo=docker&logoColor=2496ED)](#)
[![SQLite Badge](https://img.shields.io/badge/-SQLite-003B57?style=flat-square&labelColor=black&logo=sqlite&logoColor=003B57)](#)
[![Radix UI Badge](https://img.shields.io/badge/-Radix%20UI-161618?style=flat-square&labelColor=black&logo=radixui&logoColor=161618)](#)



# MDRCloud Terminal

**MDRCloud Terminal** is an open-source, self-hosted all-in-one server management platform based on Termix. It provides a multi-platform
solution for managing your servers and infrastructure through a single, intuitive interface. MDRCloud Terminal offers SSH terminal
access, SSH tunneling capabilities, remote file management, and many other tools.

> **Note:** This is a rebranded version of [Termix](https://github.com/Termix-SSH/Termix) for MDRCloud.

# Features

- **SSH Terminal Access** - Full-featured terminal with split-screen support (up to 4 panels) with a browser-like tab system. Includes support for customizing the terminal including common terminal themes, fonts, and other components
- **SSH Tunnel Management** - Create and manage SSH tunnels with automatic reconnection and health monitoring
- **Remote File Manager** - Manage files directly on remote servers with support for viewing and editing code, images, audio, and video. Upload, download, rename, delete, and move files seamlessly
- **Docker Management** - Start, stop, pause, remove containers. View container stats. Control container using docker exec terminal. It was not made to replace Portainer or Dockge but rather to simply manage your containers compared to creating them.
- **SSH Host Manager** - Save, organize, and manage your SSH connections with tags and folders, and easily save reusable login info while being able to automate the deployment of SSH keys
- **Server Stats** - View CPU, memory, and disk usage along with network, uptime, and system information on any SSH server
- **Dashboard** - View server information at a glance on your dashboard
- **RBAC** - Create roles and share hosts across users/roles
- **User Authentication** - Secure user management with admin controls and OIDC and 2FA (TOTP) support. View active user sessions across all platforms and revoke permissions. Link your OIDC/Local accounts together.
- **Database Encryption** - Backend stored as encrypted SQLite database files. View [docs](https://docs.termix.site/security) for more.
- **Data Export/Import** - Export and import SSH hosts, credentials, and file manager data
- **Automatic SSL Setup** - Built-in SSL certificate generation and management with HTTPS redirects
- **Modern UI** - Clean desktop/mobile-friendly interface built with React, Tailwind CSS, and Shadcn. Choose between dark or light mode based UI.
- **Languages** - Built-in support ~30 languages (bulk translated via Google Translate, results may vary ofc)
- **Platform Support** - Available as a web app, desktop application (Windows, Linux, and macOS), and dedicated mobile/tablet app for iOS and Android.
- **SSH Tools** - Create reusable command snippets that execute with a single click. Run one command simultaneously across multiple open terminals.
- **Command History** - Auto-complete and view previously ran SSH commands
- **Command Palette** - Double tap left shift to quickly access SSH connections with your keyboard
- **SSH Feature Rich** - Supports jump hosts, warpgate, TOTP based connections, SOCKS5, password autofill, etc.

# Planned Features

See [Projects](https://github.com/orgs/Termix-SSH/projects/2) for all planned features. If you are looking to contribute, see [Contributing](https://github.com/Termix-SSH/Termix/blob/main/CONTRIBUTING.md).

# Installation

Supported Devices:

- Website (any modern browser on any platform like Chrome, Safari, and Firefox)
- Windows (x64/ia32)
  - Portable
  - MSI Installer
  - Chocolatey Package Manager
- Linux (x64/ia32)
  - Portable [(AUR available)](https://aur.archlinux.org/packages/termix-bin)
  - AppImage
  - Deb
  - Flatpak
- macOS (x64/ia32 on v12.0+)
  - Apple App Store
  - DMG
  - Homebrew
- iOS/iPadOS (v15.1+)
  - Apple App Store
  - ISO
- Android (v7.0+)
  - Google Play Store
  - APK

Visit the Termix [Docs](https://docs.termix.site/install) for more information on how to install Termix on all platforms. Otherwise, view
a sample Docker Compose file here:

```yaml
services:
  termix:
    image: ghcr.io/lukegus/termix:latest
    container_name: termix
    restart: unless-stopped
    ports:
      - "8080:8080"
    volumes:
      - termix-data:/app/data
    environment:
      PORT: "8080"

volumes:
  termix-data:
    driver: local
```

# Support

If you need help or want to request a feature with Termix, visit the [Issues](https://github.com/Termix-SSH/Support/issues) page, log in, and press `New Issue`.
Please be as detailed as possible in your issue, preferably written in English. You can also join the [Discord](https://discord.gg/jVQGdvHDrf) server and visit the support
channel, however, response times may be longer.

# Screenshots

<p align="center">
  <img src="./repo-images/Image 1.png" width="400" alt="Termix Demo 1"/>
  <img src="./repo-images/Image 2.png" width="400" alt="Termix Demo 2"/>
</p>

<p align="center">
  <img src="./repo-images/Image 3.png" width="400" alt="Termix Demo 3"/>
  <img src="./repo-images/Image 4.png" width="400" alt="Termix Demo 4"/>
</p>

<p align="center">
  <img src="./repo-images/Image 5.png" width="400" alt="Termix Demo 5"/>
  <img src="./repo-images/Image 6.png" width="400" alt="Termix Demo 6"/>
</p>

<p align="center">
  <img src="./repo-images/Image 7.png" width="400" alt="Termix Demo 7"/>
  <img src="./repo-images/Image 8.png" width="400" alt="Termix Demo 8"/>
</p>

<p align="center">
  <img src="./repo-images/Image 9.png" width="400" alt="Termix Demo 9"/>
  <img src="./repo-images/Image 10.png" width="400" alt="Termix Demo 110"/>
</p>

<p align="center">
  <video src="https://github.com/user-attachments/assets/88936e0d-2399-4122-8eee-c255c25da48c" width="800" controls>
    Your browser does not support the video tag.
  </video>
</p>
Some videos and images may be out of date or may not perfectly showcase features.

# License

Distributed under the Apache License Version 2.0. See LICENSE for more information.

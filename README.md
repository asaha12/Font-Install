# Linux Font Installer 🖋️

A simple set of commands to manually install `.ttf` TrueType fonts system-wide on Linux.

## Quick Start

If you have downloaded font files in your Downloads folder and want to make them available to all users and applications, run the following commands:

### 1. Create the Font Directory
First, ensure the local shared font directory exists:

```bash
sudo mkdir -p /usr/local/share/fonts
```

### 2. Copy the Fonts

Copy all `.ttf` files from your Downloads folder to the system font directory:

```bash
sudo cp ~/Downloads/*.ttf /usr/local/share/fonts/

```

### 3. Rebuild the Font Cache

Force the system to scan the new directory and update the cache so the fonts appear in your applications:

```bash
sudo fc-cache -f -v

```

---

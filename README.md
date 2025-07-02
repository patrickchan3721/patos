# PatOS
PatOS - Small Linux Rescue Boot Disk

# 🐧 PatOS — Lightweight Live Linux Boot ISO

**PatOS** is a minimal, fast-booting live Linux ISO designed for flexibility, recovery, and customization. It provides a clean Linux environment without installation, perfect for troubleshooting, testing, or building custom workflows.

## 🔧 Features

- ✅ Boots on most x86_64 systems (BIOS & UEFI supported)
- ⚡ Small ISO size for fast booting and portability
- 🧰 Includes essential CLI tools: `bash`, `curl`, `ssh`, `fdisk`, and more
- 🛠 Modular layout for easy customization or remastering
- 💾 Optional persistence/overlay support (if enabled)
- 🧪 Ideal for VMs, USB boot, or bare-metal testing

## 🚀 Use Cases

- 🔍 System recovery or diagnostics
- 🔒 Secure browsing or ephemeral sessions
- 🧪 Hardware compatibility testing
- 👨‍💻 Demos, development, or automation platforms

## 📦 ISO Details

| Property       | Value                  |
|----------------|------------------------|
| Architecture   | x86_64                 |
| Boot Support   | BIOS + UEFI            |
| Init System    | [init type, e.g. `sysvinit`, `systemd`, `busybox`] |
| Kernel Version | [your kernel version]  |
| ISO Size       | ~[ISO size] MB         |

## 🖥️ Boot Instructions

1. Flash the ISO to a USB drive (e.g., with `dd` or [balenaEtcher](https://www.balena.io/etcher/))
2. Boot from USB or load into a VM
3. You’ll be dropped into a ready-to-use shell or desktop environment (if GUI is included)

```bash
# Example flash command (DANGEROUS — double-check device!)
sudo dd if=mylinux.iso of=/dev/sdX bs=4M status=progress && sync

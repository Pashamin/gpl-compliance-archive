---
icon: file-zip
label: Debian Kernel Config (amd64)
---

[!badge variant="ghost" icon="globe" text="Читать на русском"](/system-utils/debian-config-amd64/)

# Debian Linux Kernel Configuration (amd64)

This archive contains Linux kernel configuration files for Debian (`amd64` architecture), including the main config, cloud-optimized profile (`cloud-amd64`), and test profile (`test`).

---

### 📥 Download

[!button variant="primary" icon="download" text="Download Archive (zip/tar)"](https://github.com/Pashamin/gpl-compliance-archive/raw/refs/heads/downloads/linux-debian-latest-debian-config-amd64.zip)

---

### 📋 Specifications & Metadata

- **Package:** `linux-debian-latest-debian-config-amd64`
- **Architecture:** `amd64`
- **License:** GPL-2.0 / GPL-3.0
- **SHA-1 Checksum:** `f3a5e3d1b2ae0620ab43213e82268c6248a3c12a`

---

### 📂 Archive Contents

| File / Directory | Description |
| :--- | :--- |
| `debian/config/amd64/config` | Main Linux kernel configuration for amd64 |
| `debian/config/amd64/config.cloud-amd64` | Optimized configuration for cloud VMs |
| `debian/config/amd64/config.test` | Test build profile |
| `debian/config/amd64/defines.toml` | Build definitions and metadata (TOML) |

---

### 🛠 Usage Instructions

=== Unpack Archive
```bash
# Extract tar.gz archive
tar -xvf linux-debian-latest-debian-config-amd64.tar.gz

# Navigate to the configuration folder
cd linux-debian-latest-debian-config-amd64/debian/config/amd64/
=== Apply Configuration to Kernel Source
# Copy main config to kernel source root
cp config /path/to/linux-source/.config

# Update and verify configuration parameters
cd /path/to/linux-source/
make olddefconfig
===
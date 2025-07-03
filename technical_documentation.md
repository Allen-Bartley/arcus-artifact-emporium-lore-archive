# 🧮 Recovered Files – Technical Conversion Process

This document describes the step-by-step methodology used to recover and convert legacy Microsoft Works documents into modern `.docx` format for archival and presentation purposes. The original materials originated from a long-running forum-based RPG project and were stored in legacy file formats that are no longer natively supported.

---

## ⚙️ Environment & Preparation

- **Virtualization**: Utilized an existing Windows 7 Ultimate virtual machine set up in VirtualBox.
- **Legacy Software**: Acquired an ISO of *Microsoft Works* from the Internet Archive and mounted it onto the VM.
- **Installation**: Installed Microsoft Works Word Processor within the VM to enable file opening and editing of `.wps` documents.

---

## 📤 File Acquisition & ISO Creation

- Original RPG files were compiled into a dedicated folder.
- Used **ImgBurn** to create a custom ISO image from the folder contents.
- Mounted the ISO as a virtual disc within the VM for file access.

---

## 📝 File Conversion Workflow

- Opened legacy `.wps` files in *Microsoft Works Word Processor*.
- Saved each file in the modern `.docx` format using the 2007 compatibility option.

---

## 🔌 File Transfer Challenges & Solutions

- **Initial Attempt**: Tried transferring files via Google Drive inside the VM, but encountered persistent connectivity issues.
- **Alternative Approach**:
  - Connected a USB drive formatted in FAT32 for compatibility between host and guest systems.
  - Enabled USB passthrough so the VM could detect and interact with the USB device.
  - Archived all converted `.docx` files into a ZIP and transferred them to the host computer via USB.

---

## ✅ Post-Conversion Verification

- Opened each `.docx` file on the host system using Microsoft Word to confirm formatting integrity and readability.
- Files were then uploaded to GitHub and summarized within the [converted_file_index.md](converted_file_index.md) for archival reference.

---

## 🗂️ Notes on File Organization

- The `/converted` folder contains cleaned and documented `.docx` files for readability.
- The `/legacy_originals` folder includes the original Microsoft Works files for historical reference.
- All flavor summaries and lore annotations are styled for accessibility and light roleplay immersion, while keeping technical documentation separate for resume reviewers and archivists.

---

This recovery process required the integration of virtualization, legacy software compatibility, file system configuration, and data transfer troubleshooting. It demonstrates a multi-disciplinary approach to digital preservation and retroactive documentation.

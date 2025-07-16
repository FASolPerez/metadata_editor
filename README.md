# metadata_editor
Interactive system for generating and applying metadata to curated image galleries, using XMP + Python + CLI logic.

**Metadata Editor** is a modular and interactive system for generating and applying image metadata using a clean `.xmp` template and a Python-based command-line interface.

This project is part of a larger toolkit for preparing curated photo galleries, particularly those involving symbolic or AI-generated visual content.

---

## 🎯 Purpose

This repository is designed as a *public-facing portfolio component*, showcasing the architecture and logic behind a local metadata editing tool.

The actual data (e.g. images, series descriptions, filenames) is handled privately and locally. This repo provides the open structure for how to:

- Manage reusable metadata for thematic series
- Insert Creative Commons licenses into image headers
- Maintain authorship, licensing, and attribution through XMP standards
- Operate via a clean terminal workflow

---

## 🧬 How It Works

1. Start from a universal `template.xmp` with all fields empty.
2. Run the upcoming Python script `metadata_editor.py` (to be added).
3. The script will prompt you for:
   - Title
   - Author name
   - Keywords
   - Description (auto-saved by series)
   - Series name (with history + auto-save)
   - License (selected from a predefined list)
4. It updates the XMP metadata of the selected image using tools like `exiftool`.

---

## 📁 Repo Structure


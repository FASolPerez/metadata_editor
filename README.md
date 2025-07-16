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
***structured documentation***


---

## 📄 XMP Template Fields

The included `template.xmp` defines these fields in compliance with the Dublin Core and XMP Rights namespaces:

| Field                     | Purpose                          |
|---------------------------|----------------------------------|
| `dc:title`                | Image title                      |
| `dc:creator`              | Author/creator name              |
| `dc:description`          | Description of the image         |
| `dc:subject`              | Keywords (tags)                  |
| `xmpRights:WebStatement`  | Author's website                 |
| `xmpRights:Marked`        | Copyright flag (set to true)     |
| `xmpRights:UsageTerms`    | Text describing license type     |
| `cc:license`              | URL to official license document |

---

## 🔐 License

This repository is licensed under the [MIT License](LICENSE), allowing free use, modification, and sharing of the included template and script logic.

> Note: This repository does **not** include personal metadata, private descriptions, or actual image files. The tool is intended to be used **locally**, ensuring full control over sensitive or creative data.

---

## ✍️ Author

**Fernando Alberto Sol Pérez**  
[fernandoalbertosolperez.com](https://fernandoalbertosolperez.com)

---

## 🧩 Future Directions

- Add `metadata_editor.py` for interactive CLI editing
- Integrate batch processing
- Add CLI-based gallery manager for symbolic series
- Optional GUI layer using Tkinter or web interface


# My Abstract Library
A professional, boilerplate structure for sharing knowledge libraries via the Abstract Folder Obsidian plugin.

[![GitHub Sponsor](https://img.shields.io/badge/sponsor-me-orange.svg?style=flat-square&logo=github-sponsors)](https://github.com/sponsors/your-username)
[![PayPal](https://img.shields.io/badge/PayPal-00457C?style=flat-square&logo=paypal&logoColor=white)](https://paypal.me/your-username)
[![Wise](https://img.shields.io/badge/Wise-00b9ff?style=flat-square&logo=wise&logoColor=white)](https://wise.com/pay/me/your-username)

## Content Overview
This vault is structured to leverage the "Abstract Folder" plugin's virtual hierarchy. By using the `parent` property in your note's frontmatter, you can organize your knowledge without being constrained by the physical file system.



## Setup Instructions
To install this library into your Obsidian vault:

1. Open **Obsidian Settings**.
2. Navigate to **Abstract Folder** > **Library Catalog**.
3. Click **View Catalog** and then navigate to **Manage Catalogs**.
4. Under **Manage Standalone Library**, paste the URL of this repository:
   `https://github.com/your-username/abstract-library-template`
   and click add.
5. This library will now appear in your **Abstract View**.

## Security & Content Guidelines
To ensure a safe experience for all users, the Abstract Folder plugin implements a robust security layer. Please adhere to the following guidelines when curating your library:

### 1. File Type Restrictions
Only standard, safe file formats are synchronized. Avoid including files with unsupported extensions as they will be blocked.
- **Allowed:** `.md`, `.txt`, `.json`, `.csv`, `.canvas`, and standard images (`.png`, `.jpg`, etc.).
- **Blocked:** `.css` files, executable scripts, and the `.obsidian/` folder are strictly blocked for security reasons (to prevent UI spoofing and configuration overwrites).

### 2. Markdown Sanitization
The plugin automatically neutralizes executable code blocks within Markdown files to prevent malicious scripts from running in a subscriber's vault.
- **Neutralized Blocks:** `dataviewjs`, `Templater`, and `CustomJS` blocks are renamed or wrapped to disable execution while remaining readable as text.
- **HTML Sanitization:** `<script>` tags are stripped or wrapped in HTML comments.

### 3. File Size Limit
Individual files must be under **10MB**. Files exceeding this limit will be skipped during synchronization to prevent storage bloat.

## For Curators (Engine 2)
Do NOT use `library.json` to trigger updates. When you want to push new notes to your subscribers, you must bump the version and timestamp inside `manifest.json`.


---
*Created with the [Abstract Library Template](https://github.com/RahmaniErfan/abstract-library-template)*

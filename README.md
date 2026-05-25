# Hwadam PhotoPin Flow Simulator

Created: 2026-05-26 00:22 KST

This folder is a standalone Netlify deployment package for sharing the Hwadam PhotoPin development flow with the customer and collaborators.

## Purpose

- Visualize the end-to-end process:
  - customer QR scan
  - app developer app UUID/session request
  - our backend session/lock/capture flow
  - preview delivery
  - final result delivery
- Show the process like a delivery tracking screen.
- Keep developer payload/response details available in a debug panel.

## Safety Boundary

This folder must not include:

- original customer photos
- meeting audio
- planning spreadsheets
- proposal PDFs/PPTX/DOCX files
- local backend code that requires private environment variables
- credential files or `.env` files

The simulator is static and uses dummy data only.

## Netlify Settings

- Build command: empty
- Publish directory: `.`
- Entry file: `index.html`

## Recommended GitHub Flow

Create a separate private repository for this folder only, for example:

```text
hwadam-photopin-simulator
```

Do not push the entire `hwadam_photo` workspace to GitHub.

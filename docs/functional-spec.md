# Functional Specification – PDF Automation Tool

## 1. Overview

This document defines the core features for the initial versions of the
PDF automation tool based on pdfme.

The focus is on a small but complete flow:

1. User opens the web app
2. Selects a document type (e.g., Invoice or Certificate)
3. Enters basic data in a form
4. Clicks a button to generate and download a PDF

---

## 2. User Roles

- End User:
  - Small business owner, freelancer, instructor, etc.
  - Uses the web UI to generate PDFs

- Administrator / Developer (me):
  - Maintains templates
  - Updates the app and releases new versions

---

## 3. Initial Document Types (MVP)

1. **Invoice (Simple)**
   - Fields:
     - Sender name / address
     - Client name / address
     - Invoice date
     - Invoice number
     - Item list (description + amount)
     - Total amount

2. **Certificate (Simple)**
   - Fields:
     - Recipient name
     - Course or event name
     - Date
     - Signature text / organization name

(Version `v0.1.0` may only support a static sample with some of these fields.
Dynamic item lists can be added in later versions.)

---

## 4. Core Features (MVP)

### 4.1 Template Selection

- A dropdown or buttons to choose:
  - Invoice
  - Certificate

### 4.2 Data Input Form

- Simple form corresponding to the selected template
- Validation:
  - Required fields: basic presence check
  - No complex validation in MVP

### 4.3 PDF Generation

- When user clicks "Generate PDF" or "Download":
  - For MVP:
    - Use pdfme in the frontend
    - Use a predefined template JSON
    - Generate PDF synchronously and trigger download
  - Later:
    - Call backend API for generation

### 4.4 Download Behavior

- Browser starts downloading `invoice.pdf` or `certificate.pdf`
- No login required in MVP

---

## 5. Non-Functional Requirements (MVP)

- The app should work in modern browsers (Chrome, Edge, Firefox)
- Basic mobile responsiveness (not perfect, but usable)
- Clear error message if PDF generation fails
- English UI first; later versions may support Japanese labels

---

## 6. Future Extensions (Beyond MVP)

- Multi-page invoices with dynamic rows
- Template editor UI for advanced users
- User accounts and saved templates
- Branding (upload logo, change colors)
- Integration with external systems (e.g., form tools or booking systems)

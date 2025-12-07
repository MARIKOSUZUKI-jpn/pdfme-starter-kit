# Project Scope – PDF Automation Tool (pdfme × React × Node.js)

## 1. Background

Many small businesses, freelancers, and educators need to generate
consistent, branded PDF documents (invoices, certificates, receipts, etc.),
but existing tools are either:

- too technical (developer-only libraries)
- too limited (simple invoice generators)
- or too heavy/expensive (enterprise PDF services)

This project aims to provide a developer-friendly and designer-friendly
PDF generation starter kit built on top of pdfme.

## 2. Goal

Build an open-source starter kit and demo application that:

- allows non-technical users to generate branded PDFs through a simple UI
- demonstrates how to integrate pdfme with React and Node.js
- can be extended into a commercial service or client work (Coconala, freelance, etc.)
- can be used as a portfolio piece for software engineering roles in Canada

## 3. Target Users

Primary:

- Freelancers and small business owners (coaches, instructors, beauty salons, etc.)
- Designers who want to offer PDF templates with automation

Secondary:

- Developers who want a clean example of pdfme integration
- Hiring managers / recruiters evaluating my skills

## 4. In Scope (What this project WILL cover)

- React-based frontend with:
  - template selection (e.g., Invoice, Certificate)
  - simple form input
  - live or near-live preview of the PDF
  - one-click download

- Node.js backend with:
  - basic API for generating PDFs using pdfme
  - simple logging and error handling

- Documentation:
  - architecture overview
  - setup instructions
  - basic usage guide

## 5. Out of Scope (for initial versions)

- Multi-tenant user management / authentication
- Advanced template editing like full drag-and-drop builder
- Payment integration (Stripe, etc.)
- Large-scale performance optimization

These can be considered for later versions after the MVP.

## 6. Success Criteria

The project is considered successful if:

- A user can open the demo, select a template, input data, and download a PDF.
- The project is publicly available on GitHub with clear documentation.
- The structure is clean enough to be explained in an interview.
- At least one real person (client, friend, small business) can use it for their document.

## 7. Deliverables

- GitHub repository with:
  - frontend (React + Vite)
  - backend (Node.js + Express)
  - docs/ directory with specifications and architecture
- Live demo deployment (e.g., Vercel + simple backend hosting)
- Versioned releases (tags) starting from `v0.1.0` (MVP)

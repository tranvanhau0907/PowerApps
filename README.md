# PowerApps
PowerApps Des
# 📄 PowerApps PCF - PDF Signature Viewer Control

# 🎬 Demo
📺 [Watch on YouTube](https://youtu.be/3lE_X1GEidA)

## 🧩 Overview
**PDF Signature Viewer** is a custom PowerApps Component Framework (PCF) control that allows users to:
- Upload and preview PDF files directly inside a Power Apps Canvas App.
- Navigate, zoom, and view all pages of the PDF document.
- Create, move, and resize a **signature box** to capture signature position (X, Y, Width, Height, Page).
- Automatically send back signature data and file content (Base64) to Power Apps for further processing or digital signing flows.

This component is built using **TypeScript** and **PDF.js** for rendering and interaction.

---

## 🚀 Features
✅ Upload local PDF file and render it with smooth scrolling  
✅ Zoom In / Zoom Out / Reset Zoom  
✅ Page navigation and “Go To Page” input  
✅ Add, move, resize, and remove signature box  
✅ Auto-sync signature box coordinates to Power Apps  
✅ Return PDF file (Base64) and metadata via output properties  

---

| Property Name | Type | Usage | Description |
|----------------|------|--------|--------------|
| `fileName` | SingleLine.Text | output | PDF file name |
| `fileContent` | SingleLine.Text | bound | Base64 content of uploaded PDF |
| `signatureX` | Decimal | output | X-coordinate (relative position %) |
| `signatureY` | Decimal | output | Y-coordinate (relative position %) |
| `signatureWidth` | Decimal | output | Signature box width (relative %) |
| `signatureHeight` | Decimal | output | Signature box height (relative %) |
| `signaturePage` | Whole Number | output | Page number containing signature |
| `errorMessage` | SingleLine.Text | output | Error / info messages |
| `messageType` | SingleLine.Text | output | Message type (`info`, `warning`, `error`) |

# MarkdownConverter 📝

> **Single-file, 100% local Markdown converter directly in your browser.**

`MarkdownConverter` runs entirely on the client side to instantly convert your Markdown files or pasted text into beautiful, clean HTML, print-ready PDFs, or native Microsoft Word (.docx) documents. No server, no installation, maximum privacy.

---

## 🔒 100% Local, Private & Secure

Because `MarkdownConverter` is built as a single, self-contained HTML/CSS/JavaScript file, it requires no external backend server and values your privacy.

* **Run Anywhere, 100% Offline:** Open the file in any modern web browser. No internet connection, local server setups, or complex command-line configurations are required.
* **No Data Uploads:** Your sensitive documents never touch a server. All tokenization, parsing, formatting, and file exports are executed purely in your browser's local memory.
* **No Tracking or Cookies:** Zero tracking scripts, zero web analytics, and zero cookies.

---

## ✨ Features

* **Multi-Format Output:** Export your Markdown into three distinct formats in just one click:
  * 🌐 **Save as HTML:** Generates clean, responsive HTML (including Microsoft-specific namespaces for optimal readability in Word).
  * 📄 **Save as PDF:** Renders highly polished, A4-formatted PDF files with custom margin and scaling configurations.
  * 🟦 **Save as Word (.docx):** Converts Markdown structures directly into native MS Word documents using a custom AST-to-Docx lexer.
* **Direct Lexer Parsing:** Bypasses error-prone HTML conversion back-and-forth by parsing Markdown directly via `marked` tokens. This preserves inline stylings (bold, italic, inline code) seamlessly during native Word generation.
* **Robust Markdown Elements Support:**
  * **Headings:** Auto-mapped headings from H1 to H6.
  * **Lists:** Fully supports bulleted lists and natively handles numbered lists (auto-generating sequential counters for MS Word).
  * **Tables:** Beautifully formatted Markdown tables are fully rebuilt into native MS Word table structures with customized padding and header highlighting.
  * **Code Blocks:** Syntax-friendly code formatting (`monospace` fonts and custom styling).
  * **Blockquotes & Horizontal Rules:** Elegant indentation and dividers matching the UI style.
* **Clean UI & Split Views:**
  * Drag-and-drop file uploads (supports `.md`, `.txt`, `.markdown`).
  * Instant raw text-input field with a fluid UI workspace.
  * Live responsive Preview mode that switches seamlessly back to the editor.
* **A4 Print Optimized:** Includes dedicated `@media print` stylesheets to ensure manual browser printing yields flawless, margins-synchronized paper outputs.

---

## 📦 Bundled Libraries & Licenses

This project integrates three world-class open-source libraries (licensed under MIT), which are referenced at the bottom of the HTML file:

1. **[Marked](https://github.com/markedjs/marked)** (v18.1.1) – For lightning-fast Markdown tokenization and HTML rendering.
2. **[html2pdf.js](https://github.com/eKoopmans/html2pdf.js)** (v0.10.1) – For stable, client-side PDF rendering using html2canvas and jsPDF.
3. **[Docx.js](https://github.com/dolanmiu/docx)** (v8.5.0) – For generating native Microsoft Word documents from scratch.



### 🌐 Switching to CDN (Optional)

If you prefer to use a Content Delivery Network (CDN), you can simply replace the inline-bundled library code near the bottom of the HTML file with these script tags:

```html
<!-- Alternative: Load libraries via jsDelivr CDN -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/marked/18.1.1/lib/marked.umd.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/docx@8.5.0/build/index.umd.min.js"></script>
```

---

## 📄 License

This project is licensed under the **MIT License**. You can find the licensing details in the `LICENSE` file.

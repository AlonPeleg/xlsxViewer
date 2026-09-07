# CSV / XLSX Viewer & Table Comparison Tool

A lightweight, client-side web application designed for fast, seamless viewing, filtering, searching, and comparing of tabular data files (`.csv`, `.tsv`, `.xlsx`, `.xls`). Built using pure JavaScript, CSS, and HTML with no heavy backend dependencies, it runs entirely in your browser.

**Live Demo:** [https://alonpeleg.github.io/xlsxViewer/](https://alonpeleg.github.io/xlsxViewer/)

---

## Overview & Key Functionality

### 📊 Tabular Data Viewer
- **Multi-Format Support:** Parse and render `.csv`, `.tsv`, `.txt`, `.xlsx`, and `.xls` files.
- **Multi-Sheet Navigation:** Full tabbed support for Excel workbooks with multiple sheets.
- **Interactive Data Inspection:**
  - Fast sorting by clicking on column headers with numeric and alphanumeric detection.
  - Search highlighting with real-time result match counters.
  - "Only matches" filter to focus strictly on matching data rows.
  - Automatic data-type styling for Numbers, Booleans, and Dates, along with Right-to-Left (RTL) text auto-detection for languages like Hebrew and Arabic.
  - Flexible layout modes including Stacked View vs. Grid View and a Focus/Fullscreen overlay mode.

### 🔍 Table Comparison (Diff Utility)
- **Side-by-Side Table Comparison:** Compare datasets across two editable panels (Panel A vs. Panel B).
- **Direct Cell Editing:** Click and edit any cell directly inside the grid with full keyboard navigation using `Tab`, `Shift+Tab`, and `Enter`.
- **Visual Diff Highlighting:** Instantly identify added rows, removed rows, changed cell values, and exclusive columns.
- **Dual Diff Views:** Toggle between a unified difference list and a side-by-side comparison view.
- **Panel Controls:** Add or remove rows and columns on the fly, toggle header row treatment, and save modified panels back into the primary viewer.

### 📤 Export & Utility Options
- **Multi-Format Copy:** Quick-copy active sheet contents to clipboard as CSV, JSON, or Markdown table syntax.
- **File Downloads:** Export modified tables directly to `.csv` or `.xlsx` format.
- **Local Persistence:** Retains loaded datasets in browser `localStorage` across page refreshes.

---

## How to Use

### Loading Files
1. **Drag & Drop or Upload:** Use the upload icon in the top toolbar or drop `.csv`, `.tsv`, or `.xlsx` files anywhere onto the drop zone.
2. **Text Paste:** Copy raw CSV or TSV data, paste it directly into the top text box, and click **Add Table**.

### Comparing Datasets
1. Click on the **Compare** tab in the top header navigation.
2. Load data into **Panel A** and **Panel B**:
   - Select panel targets using file chips.
   - Drag and drop file chips directly onto Panel A or Panel B.
   - Click **start a blank one** to build a table manually.
3. Edit cell values, adjust columns or rows, and click **Compare Panels** to generate the diff analysis.

# VTUSync — VTU Results Archive

> A clean and responsive web interface for accessing **Visvesvaraya Technological University (VTU)** examination result portals from one convenient location.

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5\&logoColor=white)](#)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3\&logoColor=white)](#)
[![Responsive](https://img.shields.io/badge/Design-Responsive-success)](#)
[![VTUSync](https://img.shields.io/badge/VTUSync-Results-111827)](https://vtusync.in)

---

## 📌 Overview

**VTUSync Results Archive** is a lightweight, responsive static webpage designed to help VTU students quickly find examination result portals.

Instead of searching through multiple VTU result pages, students can select their examination and directly access the appropriate official result portal.

The current implementation includes examination results from **2025 to 2026**, with support for regular results, CBCS, Non-CBCS, and revaluation portals where available.

---

## ✨ Highlights

| Feature                | Description                                       |
| ---------------------- | ------------------------------------------------- |
| 🎓 **VTU Results**     | Centralized access to examination result portals  |
| 🔗 **Official Links**  | Redirects directly to VTU's result infrastructure |
| 🆕 **Latest Result**   | Highlights the most recently added examination    |
| 🔄 **Revaluation**     | Dedicated revaluation links where available       |
| 📚 **CBCS / Non-CBCS** | Supports different result portals                 |
| 🧮 **SGPA / CGPA**     | Quick access to VTUSync calculators               |
| 📖 **Result Guide**    | Explains VTU result nomenclature                  |
| 📱 **Responsive**      | Optimized for desktop, tablet, and mobile         |
| ⚡ **Lightweight**      | Pure HTML and CSS with no framework dependency    |

---

## 🎯 Purpose

The goal of this project is simple:

> **Make VTU result links easier for students to find and access.**

The page acts as a convenient directory while keeping the actual result processing and result data on the official VTU infrastructure.

---

## 🖥️ Interface

The page follows a modern **dark Soft UI / Claymorphism-inspired design** featuring:

* Clean result cards
* Rounded action buttons
* Subtle depth and shadows
* Latest-result highlighting
* Responsive layouts
* Color-coded result categories
* Compact information sections

The main result archive uses individual cards for each examination and groups links into categories such as **Regular** and **Revaluation**.

---

## 📚 Result Archive

The current archive contains:

### May – June 2026

* Main Result Portal
* CBCS
* Revaluation — CBCS

### December 2025 – January 2026

* Main Result Portal
* CBCS
* Revaluation — CBCS

### Makeup Examination 2025

* CBCS

### Silver Jubilee July 2025

* Main Result Portal
* CBCS
* Non-CBCS

### June / July 2025

* Main Result Portal
* CBCS
* Revaluation — CBCS

The **May–June 2026 examination** is currently highlighted as the latest result entry.

---

## 🧩 Technology Stack

This project intentionally keeps the technology stack simple.

```text
HTML5
CSS3
CSS Custom Properties
Flexbox
CSS Grid
Media Queries
CSS Animations
```

### No Framework Required

There is currently no dependency on:

* Bootstrap
* Tailwind CSS
* React
* Vue
* Angular
* jQuery

This makes the project easy to deploy on almost any static hosting platform.

---

## 📁 Project Structure

```text
vtusync-results/
│
├── index.html
└── README.md
```

All styling is currently contained within `index.html`, making the project portable and easy to deploy. The document contains the complete page structure, styling, responsive rules, and result links.

---

## 🚀 Run Locally

### Option 1 — Open Directly

Simply open:

```text
index.html
```

in any modern web browser.

### Option 2 — VS Code

Install the **Live Server** extension and select:

```text
Open with Live Server
```

The page will open in your browser automatically.

### Option 3 — Local HTTP Server

Using Python:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

---

## 🔗 Adding a New Result

To add a new examination, create another result card inside the result list.

Example structure:

```html
<article class="vtusync-result-card">

    <div class="vtusync-result-top">
        <div>
            <h3>New Examination 2026</h3>
        </div>

        <span class="vtusync-result-year">
            2026
        </span>
    </div>

    <div class="vtusync-result-group">

        <h4>Regular</h4>

        <div class="vtusync-result-actions">

            <a
                href="OFFICIAL_RESULT_URL"
                target="_blank"
                rel="noopener noreferrer"
                class="vtusync-result-btn vtusync-result-btn-primary">
                Main Page
            </a>

        </div>

    </div>

</article>
```

Replace `OFFICIAL_RESULT_URL` with the appropriate official VTU result URL.

---

## 🎨 Design System

The interface uses CSS custom properties for the primary design tokens.

```css
:root {
    --cs-color-primary: #ffffff;
    --cs-color-secondary: #a1a1aa;
    --cs-layout-background: #18181b;
    --cs-color-border: #27272a;
    --cs-color-button: #27272a;
}
```

This makes the visual design easier to customize without modifying every component individually.

---

## 📱 Responsive Behaviour

The interface adapts to different screen sizes using CSS media queries.

### Desktop

* Two-column information sections
* Spacious result cards
* Horizontal action buttons

### Tablet

* Result groups collapse where required
* Information cards become single-column

### Mobile

* Compact cards
* Smaller typography
* Flexible buttons
* Reduced spacing
* Single-column layout

The page includes dedicated breakpoints at approximately **800px, 600px, and 380px**.

---

## 🧮 VTUSync Student Tools

The results page also provides quick access to VTUSync's calculation tools:

### SGPA Calculator

Calculate semester grade point average.

### CGPA Calculator

Calculate cumulative grade point average.

Both tools are linked directly from the results page.

---

## 📖 VTU Result Nomenclature

The page provides a quick reference for commonly displayed result statuses.

| Code     | Meaning                                 |
| -------- | --------------------------------------- |
| `P / PP` | Pass / Pass in Non-Credit Subject       |
| `F / NP` | Fail / Not Passed in Non-Credit Subject |
| `A`      | Absent                                  |
| `W`      | Withheld                                |
| `X / NE` | Not Eligible                            |

These definitions are included directly in the page's result nomenclature section.

---

## 📝 How to Check VTU Results

The page provides a simple three-step workflow:

```text
┌──────────────────────────────┐
│  1. Visit Official VTU Site  │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│  2. Choose Your Scheme       │
│     CBCS / Non-CBCS          │
└──────────────┬───────────────┘
               ↓
┌──────────────────────────────┐
│  3. Enter USN + Captcha      │
└──────────────┬───────────────┘
               ↓
        View Your Result
```

The instructions specifically guide students to select the appropriate scheme and enter their **University Seat Number (USN)** and captcha.

---

## 🔐 Security & External Links

External result links use:

```html
target="_blank"
rel="noopener noreferrer"
```

This ensures external pages open in a new tab while preventing the newly opened page from accessing the originating window through `window.opener`.

---

## ⚠️ Disclaimer

> **VTUSync is not affiliated with Visvesvaraya Technological University (VTU).**

The result links displayed on this project belong to the official VTU result infrastructure.

VTUSync does not control:

* VTU result availability
* VTU server uptime
* Result publication dates
* Result data
* Official VTU website changes

The page explicitly informs users that VTUSync does not control the official VTU result portal.

**For educational and informational purposes only.**

---

## 🤝 Contributing

Contributions are welcome.

### Recommended Contribution Workflow

```text
Fork
  ↓
Create Branch
  ↓
Make Changes
  ↓
Test
  ↓
Commit
  ↓
Push
  ↓
Pull Request
```

Before submitting a pull request:

* Verify all result URLs.
* Check the page on mobile.
* Maintain the existing naming conventions.
* Keep the interface responsive.
* Avoid unnecessary dependencies.

---

## 🌐 VTUSync

Part of the **VTUSync** ecosystem for VTU students.

**Website:**
https://vtusync.in

Useful student resources include:

* VTU Results
* SGPA Calculator
* CGPA Calculator
* Previous Year Questions
* Study Materials
* Scheme of Valuation
* VTU Updates

---

## 📄 License

This project is provided for **educational and informational purposes**.

The official VTU result portals and their respective content remain the property of their respective owners.

---

## ⭐ Support the Project

If this project is useful to you:

* ⭐ Star the repository
* 🍴 Fork the project
* 🐛 Report issues
* 💡 Suggest improvements
* 🤝 Contribute improvements

---

<p align="center">
  Made for VTU Students ❤️
</p>

<p align="center">
  <strong>VTUSync</strong> · Simplifying VTU Resources
</p>

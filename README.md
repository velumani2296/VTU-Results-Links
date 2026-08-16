# VTUSync – VTU Results Archive

A modern, responsive **VTU Results Archive** page developed for [VTUSync](https://vtusync.in). It provides students with quick access to various **Visvesvaraya Technological University (VTU)** examination result portals, including regular results, CBCS, Non-CBCS, and revaluation results.

The interface is designed with a clean **modern Soft UI / Claymorphism-inspired design** and is optimized for desktop, tablet, and mobile devices.

---

## ✨ Features

* 📚 **VTU Result Archive**

  * Centralized collection of VTU examination result links.
  * Results organized by examination period and year.

* 🔗 **Official VTU Result Links**

  * Links directly to the official VTU results portal.
  * Opens result portals in a new browser tab.

* 🎓 **CBCS & Non-CBCS Support**

  * Separate links for CBCS results.
  * Non-CBCS result links where available.

* 🔄 **Revaluation Results**

  * Dedicated revaluation result links for supported examinations.

* 🆕 **Latest Result Highlight**

  * The latest examination is visually highlighted with a "Latest" badge.
  * Includes an updated-date indicator.

* 🧮 **SGPA & CGPA Calculators**

  * Quick access to VTUSync SGPA Calculator.
  * Quick access to VTUSync CGPA Calculator.

* 📖 **VTU Result Nomenclature**

  * Explains commonly used result abbreviations:

    * `P / PP` – Pass / Pass in Non-Credit Subject
    * `F / NP` – Fail / Not Passed in Non-Credit Subject
    * `A` – Absent
    * `W` – Withheld
    * `X / NE` – Not Eligible

* 📝 **How to Check Results**

  * Simple three-step guide for students:

    1. Visit the official VTU results website.
    2. Select the appropriate scheme.
    3. Enter USN and captcha.

* 📱 **Responsive Design**

  * Desktop-friendly layout.
  * Tablet optimization.
  * Mobile-friendly cards and buttons.
  * Additional optimization for small-screen devices.

* 🎨 **Modern UI**

  * Soft UI / Claymorphism-inspired cards.
  * Rounded buttons.
  * Subtle shadows and hover effects.
  * Animated result status indicator.
  * Responsive typography using CSS `clamp()`.

---

## 📅 Currently Included Results

The current page contains result links for:

| Examination                     |    Year |
| ------------------------------- | ------: |
| May – June 2026 Exam            |    2026 |
| Dec 2025 – Jan 2026 Exam        | 2025–26 |
| Makeup Exam                     |    2025 |
| Silver Jubilee July Examination |    2025 |
| June / July Examination         |    2025 |

The latest section is currently marked as **May – June 2026 Exam**, with regular, CBCS, and revaluation links where available.

---

## 🛠️ Technologies Used

* **HTML5**
* **CSS3**
* **CSS Custom Properties**
* **CSS Grid**
* **CSS Flexbox**
* **CSS Media Queries**
* **Responsive Web Design**
* **CSS Animations**
* **External Links**

No JavaScript framework or external CSS framework is required for the current page.

---

## 📁 Project Structure

```text
.
├── index.html
└── README.md
```

The current implementation keeps the HTML structure and styling in a single `index.html` file.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/your-repository.git
```

### 2. Open the project

Navigate into the project directory:

```bash
cd your-repository
```

### 3. Run the page

Since this is a static HTML project, no build process is required.

Simply open:

```text
index.html
```

in your web browser.

You can also use **VS Code Live Server** for local development.

---

## 🔗 Result Link Management

Each result button is an HTML anchor element pointing directly to the corresponding VTU result portal.

Example:

```html
<a
    href="https://results.vtu.ac.in/indexMJ26.php"
    target="_blank"
    rel="noopener noreferrer"
    class="vtusync-result-btn vtusync-result-btn-primary">
    Main Page
</a>
```

When adding a new result:

1. Create a new result card.
2. Add the examination name and year.
3. Add the official VTU result URL.
4. Add CBCS/Non-CBCS links if applicable.
5. Add revaluation links if available.
6. Mark the latest examination appropriately.

---

## 🎨 Design

The interface uses a modern dark Soft UI / Claymorphism-inspired design.

### Main Design Elements

* Rounded result cards
* Pill-shaped buttons
* Subtle neumorphic shadows
* Animated "Latest" indicator
* Responsive two-column layouts
* Mobile-first adjustments
* Consistent typography
* Color-coded result categories

The stylesheet also defines reusable CSS variables for primary colors, borders, backgrounds, buttons, shadows, and fonts.

---

## 📱 Responsive Breakpoints

The page includes dedicated responsive styles for:

* **Desktop**
* **Tablet**
* **Mobile**
* **Small mobile devices**

At widths below `800px`, multi-column sections collapse into single-column layouts. Additional adjustments are applied below `600px` and `380px` for smaller devices.

---

## 🧮 VTUSync Tools

The results page provides quick access to:

* **SGPA Calculator**
* **CGPA Calculator**

These tools are linked to the corresponding VTUSync calculator pages.

---

## 📖 How Students Can Check Results

The page provides the following workflow:

```text
Visit Official VTU Results Website
              ↓
       Choose Scheme
              ↓
       Enter USN + Captcha
              ↓
         View Results
```

Students are instructed to select the appropriate CBCS or Non-CBCS option depending on their academic scheme.

---

## ⚠️ Disclaimer

This project is **not affiliated with Visvesvaraya Technological University (VTU)**.

The result links redirect users to the official VTU result portal. VTUSync does not control the availability, content, or operation of the official VTU website.

> **Not affiliated with VTU. For Educational Purposes Only.**

---

## 🤝 Contributing

Contributions and improvements are welcome.

If you find an incorrect or outdated result link:

1. Fork the repository.
2. Update the relevant result link.
3. Test the link.
4. Commit your changes.
5. Create a Pull Request.

For UI improvements, please maintain the existing responsive behavior and accessibility of the page.

---

## 📌 Important Notes

* Result links point to external VTU infrastructure.
* VTU may change or disable result URLs at any time.
* Always verify the result information from the official VTU portal.
* The result archive should be updated whenever new examination results are released.
* Do not enter sensitive information on unofficial websites.

---

## 🌐 VTUSync

**VTUSync** provides various tools and resources for VTU students, including:

* VTU Results
* SGPA Calculator
* CGPA Calculator
* Study Materials
* Previous Year Questions
* Scheme of Valuation
* Academic Updates

Website: **https://vtusync.in**

---

## 📄 License

This project is intended for educational and informational purposes.

If you are publishing a modified version of this project, retain the appropriate attribution and disclaimer where applicable.

---

### ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.

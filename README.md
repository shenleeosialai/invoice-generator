#  Responsive Invoice Generator (HTML → PDF)

A clean, professional, **client‑ready invoice generator** built with **pure HTML, CSS, and JavaScript**.
Designed to look **exactly the same on desktop and mobile**, with PDF export, editable fields, and payment status indicators.

---

## ✨ Features

*  **Professional invoice layout** (desktop-grade, non-breaking)
*  **Mobile-friendly without layout changes** (horizontal scroll when needed)
*  **Inline editable fields** (company info, client info, notes, terms)
*  **Company logo support** (top-left)
*  **Automatic total calculation** (tax already included)
*  **Paid / Unpaid status badge**
*  **Dynamic item rows** (add / remove items)
*  **Real-time total & balance due updates**
*  **One-click PDF export** using `html2canvas` + `jsPDF`
*  **Modern UI** (blue header, light table body `#f9fafb`)

---

##  Design Philosophy

This project intentionally **does NOT collapse or redesign the layout on mobile**.

✔ Invoices must retain structure for printing, sharing, and accounting
✔ Mobile users can scroll horizontally without losing context
✔ The desktop design is preserved pixel-for-pixel

This mirrors real-world tools like **Zoho, Stripe, and QuickBooks** but free since i did not want to pay for subs.

---

##  Tech Stack

* **HTML5** – semantic structure
* **CSS3** – modern layout & responsiveness
* **Vanilla JavaScript** – calculations & interactions
* **html2canvas** – HTML → image rendering
* **jsPDF** – PDF generation

No frameworks. No dependencies. No build steps.

---

##  Project Structure

```text
invoice-generator/
│
├── index.html        # Main invoice file
├── logo.png          # Your company logo (replace with your own)
└── README.md         # Project documentation
```

---

##  Getting Started

### 1️ Clone the repository

```bash
git clone https://github.com/shenleeosialai/invoice-generator.git
cd invoice-generator
```

### 2️ Add your logo

Replace `logo.png` with your own logo:

* Recommended format: **PNG or SVG**
* Transparent background preferred
* Max height: `60px`

---

### 3️ Open in browser

Simply open `index.html`:

```bash
xdg-open index.html
# or double-click the file
```

---

## How to Use

1. Edit company & client details directly on the page
2. Add or remove invoice items
3. Quantities and prices auto-calculate totals
4. Toggle **PAID / UNPAID** status
5. Click **Download PDF** to export

The generated PDF is **print-ready and client-safe**.

---

## Mobile Behavior (Important)

* Layout remains **identical to desktop**
* No stacking, hiding, or card views
* Horizontal scrolling enabled on small screens

This ensures invoices remain:

* Legible
* Structured
* Accountant-friendly

---

## Customization Options

You can easily:

* Change currency (KES / USD / EUR)
* Auto-mark invoice as **PAID when balance = 0**
* Add invoice numbers or prefixes
* Lock editing before PDF export
* Integrate with **Django / Flask / Node.js** backends

---

## Limitations

* No backend persistence (client-side only)
* Data resets on page refresh

> Ideal for freelancers, small businesses, and internal tools

---

## Author

**Shenlee osialai**
Full-Stack Developer

---

## License

This project is licensed under the **MIT License**.

You are free to:

* Use
* Modify
* Distribute
* Commercialize

Attribution appreciated but not required.

---

## ⭐ Support

If you find this useful:

* Star the repository
* Fork it
* Suggest improvements

---

> Built for real-world invoices. Clean. Reliable. Professional.

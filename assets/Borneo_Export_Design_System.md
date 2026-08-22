# Borneo Export - Design System & AI Generation Prompts

Dokumen ini mendefinisikan panduan visual (Design System) yang diekstrak dari referensi gaya desain yang diberikan (soft glassmorphism, clean layout, professional medical/corporate look) dan diadaptasi untuk platform B2B ekspor komoditas "Borneo Export". Dokumen ini juga berisi prompt spesifik untuk men-generate kode UI di AI Builder (seperti Google Stitch, v0, dll).

## 1. Design System & Visual Language

### A. Color Palette (Diambil dari Referensi)
Palet warna ini memberikan kesan profesional, bersih, dapat dipercaya (trustworthy), dan bernuansa alam/maritim yang cocok untuk komoditas ekspor.

| Role | Color Name | Hex Code | Usage |
| :--- | :--- | :--- | :--- |
| **Primary** | Ocean Teal | `#429b9c` | Tombol CTA utama, icon, border aktif, elemen highlight. |
| **Secondary / Bg** | Soft Cyan | `#e3f2f2` | Background Hero section, background section alternatif. |
| **Surface** | Pure White | `#ffffff` | Background Card, form input, floating navbar. |
| **Text Primary** | Charcoal | `#1a1a1a` | Heading (H1, H2, H3), teks utama yang butuh kontras tinggi. |
| **Text Secondary** | Slate Gray | `#666666` | Paragraf deskripsi, placeholder teks, sub-heading. |

### B. Typography
* **Font Family:** 'Inter' atau 'Plus Jakarta Sans' (San-serif bersih dan modern).
* **H1 (Hero Title):** 48px - 56px, Bold (700), Line height 1.2, Warna: Charcoal.
* **H2 (Section Title):** 32px - 36px, Semi-Bold (600), Line height 1.3, Warna: Charcoal.
* **H3 (Card Title):** 20px - 24px, Medium (500), Line height 1.4, Warna: Charcoal.
* **Body Text:** 16px, Regular (400), Line height 1.6, Warna: Slate Gray.

### C. Spacing System & Layout
* **Grid System:** 12-column layout, max-width 1200px.
* **Spacing Scale (8pt grid):** 8px, 16px, 24px, 32px, 48px, 64px, 96px.
* **Section Padding:** Top/Bottom 80px - 100px untuk ruang napas (whitespace) yang luas seperti referensi.

### D. Component Inventory (Styling Attributes)
* **1. Cards (Produk / Layanan):** Background: `#ffffff`. Border-radius: 24px (Soft & Modern). Box-shadow: `0 10px 25px rgba(0, 0, 0, 0.05)` (Soft drop shadow). Padding: 24px.
* **2. Glassmorphic Filter/Info Bar (Seperti di Hero):** Background: `rgba(255, 255, 255, 0.6)`. Backdrop-filter: `blur(12px)`. Border: `1px solid rgba(255, 255, 255, 0.4)`. Border-radius: 20px. Box-shadow: `0 8px 32px rgba(66, 155, 156, 0.1)`.
* **3. Buttons (CTA):** Background: `#429b9c` (Primary). Text: White. Border-radius: 50px (Pill shape). Padding: 12px 24px. Font-weight: Medium. Shadow: Soft shadow teal. Hover state: `#357d7e`.

---

## 2. Prompts untuk AI Code Generator (Google Stitch / v0 / Claude)

*Instruksi: Copy-paste blok teks di bawah ini satu per satu ke dalam AI tool untuk menghasilkan halaman web yang konsisten dan tidak terlihat seperti template AI murahan.*

### Page 1: Home (Beranda)
```text
Role: You are an expert Frontend Developer and UI/UX Designer.
Task: Build the "Home" page for a B2B Export website named "Borneo Export".

Design Style Strict Guidelines:
- Avoid generic AI styles. Use a clean, modern, slightly soft/glassmorphic UI inspired by modern medical/fintech apps but applied to nature/export.
- Color Palette: Primary CTA (#429b9c - Ocean Teal), Backgrounds (#e3f2f2 - Soft Cyan & #ffffff), Text (#1a1a1a & #666666).
- Typography: Inter or similar modern sans-serif.
- Shapes: Large rounded corners (border-radius: 24px for large cards, fully rounded pills for buttons). Soft, diffuse drop shadows. Lots of whitespace.

Structure & Content:
1. Header/Navbar: Floating navbar, white background with soft shadow, pill-shaped. Logo on left, links (Home, About, Catalog, Quality, Shipping, Contact) in middle, "Request Quotation" button (#429b9c) on right.
2. Hero Section: 
   - Split layout or large clean background.
   - Headline: "Premium Commodities from the Heart of Borneo to the World" (Bold, Dark).
   - Subheadline: High-quality natural resources directly sourced from Kotabaru.
   - Overlapping the bottom of the hero area: A glassmorphic bar (backdrop-blur, semi-transparent white, large border-radius) containing 3 quick USP icons & text (Direct from Local Producers, Verified Quality, Seamless Export Process).
3. Top Products (Best Sellers) Section:
   - Section Title: "Featured Export Commodities".
   - Grid layout of 3 large, soft-rounded cards. 
   - Card content: High-quality image placeholder, Title (e.g., Dried Fish, Damar Resin, Spices), short description, and a subtle "View Details" text link with an arrow.
4. CTA Section:
   - Large rounded section with a Soft Cyan background (#e3f2f2).
   - Text: "Ready to scale your supply chain with premium commodities?"
   - Button: Large, pill-shaped, Ocean Teal button saying "Request for Quotation".
```

### Page 2: About Us (Tentang Kami)
```text
Role: Expert Frontend Developer.
Task: Build the "About Us" page for "Borneo Export". Maintain the exact design system from previous instructions (Teal #429b9c, rounded-2xl cards, soft shadows, inter font, lots of whitespace).

Structure & Content:
1. Page Header: Simple, clean header with Soft Cyan background (#e3f2f2). Title: "Our Story & Origins".
2. Company Profile Section:
   - Two-column layout. Left: High-quality professional image placeholder (office or nature). Right: Text detailing Borneo Export as an aggregator and official representative of Kotabaru's MSMEs (UMKM). Use elegant typography.
3. The Kotabaru Story Section:
   - Full-width layout. A visually striking timeline or 3-column feature grid explaining the natural wealth of Kotabaru, its strategic location in South Kalimantan, and its history of commodity trading.
4. ESG & Social Impact Section:
   - A distinct section (perhaps with a subtle Teal background and white text, or white cards on Teal background).
   - Focus on storytelling: "Empowering Local Communities." 
   - 3 large icon cards: 'Fair Trade for Farmers', 'Sustainable Fishing', 'Boosting Local Economy'.
   - Add a compelling closing paragraph about how buying from Borneo Export empowers local producers.
```

### Page 3: Product Catalog (Katalog Kurasi)
```text
Role: Expert Frontend Developer.
Task: Build the "Product Catalog" page for "Borneo Export". Keep the UI very clean, data-heavy but readable. B2B buyers need clear specs. Use the established design system (#429b9c primary, 24px border-radius for containers).

Structure & Content:
1. Header & Filters:
   - Title: "Curated Export Commodities".
   - Below title, a glassmorphic filter bar (Pill shapes) for categories: All, Marine & Fishery, Agriculture, Handicrafts.
2. Product Grid:
   - A clean 3-column grid of Product Cards.
   - Product Card Design: White background, 16px border-radius, soft shadow.
   - Card Content:
     * Product Image Placeholder (aspect-video, top rounded).
     * Product Name (e.g., "Premium Damar Resin (Agathis Dammara)") in bold.
     * A clean data table or list inside the card:
       - HS Code: 1301.90
       - Supply Capacity: 20 MT/Month
       - MOQ: 1 MT
     * A full-width bottom button: "View Specifications" (Ghost button style with Teal text).
3. Implement a modal or expandable section design (just the UI) for what happens when "View Specifications" is clicked (showing moisture content, sizing, packaging details).
```

### Page 4: Quality & Certifications
```text
Role: Expert Frontend Developer.
Task: Build the "Quality & Certifications" page for "Borneo Export". The goal is to build extreme trust with international B2B buyers. 

Structure & Content:
1. Page Header: Title "Uncompromising Quality & Global Standards".
2. Quality Control Process:
   - A step-by-step horizontal or vertical timeline layout. 
   - Steps: 1. Harvesting/Catching by MSMEs, 2. Sorting & Grading, 3. Quality Testing, 4. Secure Packaging.
   - Use clean, modern icons in Teal circles for each step.
3. Certifications Grid:
   - A section displaying "Supported Certifications by Our Partners".
   - A grid of logo placeholders inside clean white, soft-shadowed cards. (HACCP, Halal, BPOM, ISO). 
4. Export Documents Section:
   - A visually appealing list or grid showing the documents Borneo Export provides.
   - Use a checklist icon for: Commercial Invoice, Packing List, Bill of Lading, Certificate of Origin, Phytosanitary Certificate.
   - Wrap this in a light Soft Cyan (#e3f2f2) rounded container to highlight its importance.
```

### Page 5: How We Work / Shipping
```text
Role: Expert Frontend Developer.
Task: Build the "How We Work & Shipping" page for "Borneo Export". Emphasize logistical professionalism.

Structure & Content:
1. Step-by-Step Flow (The Process):
   - Title: "Seamless Export Process".
   - A 5-step process visual (use large numbers with Teal typography).
   - 1. Inquiry & RFQ -> 2. Sample Delivery -> 3. Contract & Payment -> 4. Production & QC -> 5. Shipping.
   - Style them as interconnected cards or a winding path.
2. Trade Terms & Logitics:
   - Two-column section. 
   - Left Column: "Supported Incoterms". List FOB (Banjarmasin/Kotabaru Port), CIF, EXW with clear, brief explanations of each.
   - Right Column: "Payment Terms". List T/T (Telegraphic Transfer) and L/C (Letter of Credit).
   - Use UI elements like checkmarks and subtle box highlights for readability.
```

### Page 6: Contact Us & RFQ
```text
Role: Expert Frontend Developer.
Task: Build the "Contact & Request for Quotation (RFQ)" page for "Borneo Export". This is the main conversion page.

Structure & Content:
1. Two-Column Layout (Split Screen style or side-by-side cards).
2. Left Column (Contact Info):
   - Title: "Let's Build a Partnership".
   - Office Address: Kotabaru, South Kalimantan, Indonesia (Include a styled Google Maps placeholder image).
   - Email: sales@borneoexport.com (Clickable styling).
   - WhatsApp CTA: A prominent, large button (using WhatsApp green or matching the Teal design system) saying "Chat on WhatsApp Business".
3. Right Column (B2B RFQ Form):
   - A clean, modern form inside a white card with 24px border-radius and soft drop shadow.
   - Fields needed:
     * Full Name
     * Company Name
     * Corporate Email
     * Country of Origin (Dropdown)
     * Interested Product (Dropdown)
     * Expected Volume (Input with unit dropdown like MT/Kgs)
     * Additional Messages (Textarea)
   - Submit Button: Large Ocean Teal (#429b9c) pill-shaped button "Submit Request".
```

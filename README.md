# Aariwork Studio — Haute Handcrafted Hand Embroidery Atelier 🪡✨

A bespoke, luxury boutique web application built with **React (Vite)**, **Framer Motion**, and **custom luxury CSS design tokens**. Designed specifically for modern brides, connoisseurs of Indian silks, and bespoke handcraft enthusiasts.

> **"Where Every Stitch Tells a Story"**

---

## 🏛️ Brand & Aesthetic Direction

- **Luxury Boutique Look**: Evoking the quiet opulence of traditional Mughal and South Indian Maggam ateliers.
- **Color Palette**:
  - Royal Deep Maroon (`#4A0E17`, `#751428`)
  - Authentic Metallic Zari Gold (`#D4AF37`, `#FDE68A`, `#996515`)
  - Warm Ivory Silk & Champagne Cream (`#FDFBF7`, `#F6F1E9`)
  - Midnight Velvet Charcoal (`#0D080A`, `#160D12`)
- **Typography**:
  - Headings: `Cormorant Garamond` & `Playfair Display` (Google Fonts)
  - Body: `Plus Jakarta Sans` (Google Fonts)
- **Artisanal Embroidery Motifs**:
  - Golden running-stitch dashed card borders
  - Thread-line dividers with centered gold zari star medallions
  - Shimmering metallic zari sheen effects
  - Custom golden hooked Aari needle cursor with dynamic trailing thread effect

---

## 🌟 Key Features & Architecture

### 1. Header & Navigation (`Navbar.jsx`)
- **Sticky Frosted Glass**: Seamless transition from transparent on the hero section to solid frosted glass on scroll.
- **Monogram Emblem**: Golden needle & zari thread circle logo.
- **Live Section Tracking**: Smooth scroll navigation with animated gold underline indicators.
- **Dark / Light Mode**: Instant one-click toggle with persisted preference in `localStorage`.
- **Wishlist Counter Badge**: Displays count of bookmarked pieces and triggers the slide-out Wishlist Drawer.
- **Mobile Menu**: Fullscreen animated drawer with quick CTA access.

### 2. Parallax Hero Section (`Hero.jsx`)
- **Big Headline**: *"Where Every Stitch Tells a Story"*.
- **Subtext & Trust Highlights**: 100% Hand-stitched on wooden adda, pure zari & authentic kundan.
- **Dual CTAs**: "Commission Custom Order" & "View Bridal Collection".
- **Visual Showcase**: Stitched image frame with floating artisan badges (*"78 Artisan Hours"*, *"Master Karigar Signed"*).

### 3. Heritage Brand Story (`AboutSection.jsx`)
- Narrative of the centuries-old Aari / Maggam needlecraft tradition.
- Core pillars: Bespoke Khaka Blueprint, Heirloom Materials Only, Artisan Dignity & Fair Wages.
- **Live Animated Counters**:
  - **1,200+** Designs Made
  - **450+** Happy Brides
  - **15+** Years of Craft Mastery
  - **100%** Handcrafted (Zero Machines)

### 4. Filterable Collection Grid (`CollectionsSection.jsx`)
- **Category Filter Tabs**: `All Silhouettes`, `Bridal`, `Blouse`, `Saree`, `Lehenga`, `Kids`.
- **Search & Sort**: Real-time keyword filter + sorting by craft hours, price, or featured status.
- **Quick View Lightbox Modal (`LightboxModal.jsx`)**:
  - High-res image display with zoom
  - Detailed specs: Artisan duration, needle technique (e.g. 3D Zardozi, Cutwork, Kundan), recommended fabrics
  - Direct *"Commission This Silhouette"* trigger
- **Wishlist Heart Toggle**: Bookmark any design with instant persistence.

### 5. "How We Work" Interactive Timeline (`ProcessSection.jsx`)
- Interactive 5-step craftsmanship journey:
  1. *Bespoke Consultation & Silhouette*
  2. *Khaka Blueprint & Motif Drafting*
  3. *Adda Mounting & Aari Stitching*
  4. *Couture Lining, Padding & Finishing*
  5. *Heirloom Packaging & Global Dispatch*
- Connected by an animated glowing gold thread track with Karigar secret notes for each phase.

### 6. Custom Order Consultation Studio (`CustomOrderSection.jsx`)
- Comprehensive design commission form:
  - Personal Details (Name, Phone/WhatsApp, Email, City)
  - Garment Silhouette (Bridal Blouse, Saree Border, Royal Lehenga, etc.)
  - Budget Tier (₹6,500 – ₹60,000+)
  - Event Date & Silk fabric arrangement
  - **Multi-image upload preview** with drag & drop support, file size/name chips, and removal
  - Special motif requests & notes
- Client-side validation with real-time feedback.
- **Celebration Success State**:
  - Generates bespoke booking docket ID (e.g., `AARI-2026-8941`)
  - Fires golden celebratory confetti using `canvas-confetti`
  - Direct *"Open Docket in WhatsApp"* button pre-filled with all order specifications.

### 7. Testimonials Carousel (`TestimonialsSection.jsx`)
- Auto-sliding carousel (with pause on hover).
- Verified bride stories from Chennai, Hyderabad, Bengaluru, Udaipur, and London.
- 5-Star gold rating, client photos, and commissioned outfit badges.

### 8. Pricing & Packages (`PricingSection.jsx`)
- 3 distinct investment cards:
  - **Festive Grace** (₹6,500 / 24–36 craft hours)
  - **Royal Heritage** (₹16,500 / 48–70 craft hours — *Most Coveted Ribbon*)
  - **Maharani Bridal Exclusive** (₹32,000+ / 90–160 craft hours)
- Features checklist and *"Select Package"* action that pre-fills the consultation form.

### 9. FAQ Accordion (`FaqSection.jsx`)
- Smooth height transitions powered by Framer Motion.
- Answers to crucial client questions on fabric courier, Pinterest designs, international delivery, and alterations.

### 10. Studio Atelier & Contact (`ContactSection.jsx` & `Footer.jsx`)
- Chennai Atelier address, fabric courier receiving desk, and visiting schedule.
- Interactive Google Maps embed preview.
- **"The Atelier Gazette" Newsletter**: Client-side validated email subscription.
- **Floating WhatsApp Button**: With online artisan pulse ring and quick chat tooltip.

### 11. Extra Features
- **Page-Load Stitching Animation (`PageLoader.jsx`)**: Golden needle drawing the monogram and brand name.
- **Custom Cursor (`CustomCursor.jsx`)**: Hooked Aari needle head with trailing golden zari thread (auto-disabled on touch screens).
- **Global Wishlist Drawer (`WishlistDrawer.jsx`)**: Accessible anywhere via navbar heart icon.
- **Multi-Route React Router**:
  - `/` — Single-page luxury scroll
  - `/collections` — Dedicated catalog view
  - `/custom-order` — Dedicated commission studio
  - `/about` — Dedicated heritage story
  - `/wishlist` — Dedicated saved collection review

---

## 📁 Clean Folder Structure

```
aariwork-studio/
├── public/
│   └── favicon.svg                  # Luxury hooked needle gold SVG favicon
├── src/
│   ├── assets/                      # Brand assets & icons
│   ├── components/
│   │   ├── common/
│   │   │   ├── Button.jsx           # Luxury button variants (gold, maroon, outline)
│   │   │   ├── Button.css
│   │   │   ├── SectionTitle.jsx     # Ornate section heading with thread divider
│   │   │   ├── SectionTitle.css
│   │   │   ├── CustomCursor.jsx     # Golden hooked needle cursor & thread trail
│   │   │   ├── CustomCursor.css
│   │   │   ├── PageLoader.jsx       # Initial SVG stitching page load animation
│   │   │   ├── PageLoader.css
│   │   │   ├── LightboxModal.jsx    # Fullscreen product quick-view modal
│   │   │   ├── LightboxModal.css
│   │   │   ├── WishlistDrawer.jsx   # Slide-out wishlist sidebar
│   │   │   ├── WishlistDrawer.css
│   │   │   ├── WhatsAppButton.jsx   # Floating WhatsApp button with pulse ring
│   │   │   └── WhatsAppButton.css
│   │   ├── layout/
│   │   │   ├── Navbar.jsx           # Sticky nav, theme switch, wishlist trigger
│   │   │   ├── Navbar.css
│   │   │   ├── Footer.jsx           # Atelier info, newsletter, social links
│   │   │   └── Footer.css
│   │   └── home/
│   │       ├── Hero.jsx             # Hero headline, CTAs, floating badges
│   │       ├── Hero.css
│   │       ├── AboutSection.jsx     # Heritage story & live animated counters
│   │       ├── AboutSection.css
│   │       ├── CollectionsSection.jsx # Filterable grid & search
│   │       ├── CollectionsSection.css
│   │       ├── ProcessSection.jsx   # 5-step interactive timeline
│   │       ├── ProcessSection.css
│   │       ├── CustomOrderSection.jsx # Consultation form & image preview
│   │       ├── CustomOrderSection.css
│   │       ├── TestimonialsSection.jsx # Auto-sliding client carousel
│   │       ├── TestimonialsSection.css
│   │       ├── PricingSection.jsx   # 3 investment tiers
│   │       ├── PricingSection.css
│   │       ├── FaqSection.jsx       # Animated accordion
│   │       ├── FaqSection.css
│   │       ├── ContactSection.jsx   # Atelier details & Google Map embed
│   │       └── ContactSection.css
│   ├── context/
│   │   ├── ThemeContext.jsx         # Dark / Light theme provider (persisted)
│   │   └── WishlistContext.jsx      # Wishlist state provider (localStorage)
│   ├── data/
│   │   ├── collections.json         # 12 handcrafted bridal items with full specs
│   │   ├── testimonials.json        # Authentic client stories & ratings
│   │   ├── pricingPackages.json     # 3 investment tiers & deliverables
│   │   ├── processSteps.json        # 5-step timeline data & karigar secrets
│   │   └── faqs.json                # Comprehensive bridal FAQs
│   ├── pages/
│   │   ├── HomePage.jsx             # Full seamless landing page
│   │   ├── CollectionsPage.jsx      # Dedicated catalog route
│   │   ├── CustomOrderPage.jsx      # Dedicated consultation route
│   │   ├── AboutPage.jsx            # Dedicated heritage route
│   │   └── WishlistPage.jsx         # Dedicated wishlist route
│   ├── App.jsx                      # Root router & providers assembly
│   ├── App.css                      # Layout rules
│   ├── index.css                    # Master luxury design system & CSS variables
│   └── main.jsx                     # Vite entry point
├── index.html                       # SEO meta tags, Google Fonts & Open Graph
├── package.json
└── README.md
```

---

## 🚀 Setup & Running Locally

### Prerequisites
- [Node.js](https://nodejs.org/) (v18 or higher recommended)
- [npm](https://www.npmjs.com/) (v9 or higher)

### Installation Steps

1. **Open terminal** and navigate into the project directory:
   ```bash
   cd d:\myproject\aariwork-studio
   ```

2. **Install dependencies**:
   ```bash
   npm install --legacy-peer-deps
   ```

3. **Start the development server**:
   ```bash
   npm run dev
   ```

4. **Open your browser** and visit:
   ```
   http://localhost:5173/
   ```

5. **Build for production** (optional):
   ```bash
   npm run build
   ```

---

## 💎 Design Highlights

- **Pure Handcraft Theme**: Zero boilerplate templates; every component is custom-crafted to reflect traditional Indian Maggam craftsmanship.
- **No Backend Required**: Pure client-side React with mock JSON data, `localStorage` persistence, and client-side form validation.
- **Full Mobile Responsiveness**: Seamless experience across mobile phones, tablets, and widescreen desktop displays.
- **Instant WhatsApp Handoff**: Deep links with pre-formatted inquiry dockets directly connecting clients to the studio's WhatsApp desk.

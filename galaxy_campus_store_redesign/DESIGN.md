---
name: Galaxy Campus Store Redesign
colors:
  surface: '#f8f9fb'
  surface-dim: '#d9dadc'
  surface-bright: '#f8f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#edeef0'
  surface-container-high: '#e7e8ea'
  surface-container-highest: '#e1e2e4'
  on-surface: '#191c1e'
  on-surface-variant: '#424655'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f3'
  outline: '#737687'
  outline-variant: '#c3c5d8'
  surface-tint: '#0052dd'
  primary: '#004fd6'
  on-primary: '#ffffff'
  primary-container: '#2167ff'
  on-primary-container: '#fcfaff'
  inverse-primary: '#b4c5ff'
  secondary: '#5400c3'
  on-secondary: '#ffffff'
  secondary-container: '#7000ff'
  on-secondary-container: '#ddcdff'
  tertiary: '#006379'
  on-tertiary: '#ffffff'
  tertiary-container: '#007e99'
  on-tertiary-container: '#f5fcff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dbe1ff'
  primary-fixed-dim: '#b4c5ff'
  on-primary-fixed: '#00174c'
  on-primary-fixed-variant: '#003daa'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#d1bcff'
  on-secondary-fixed: '#23005b'
  on-secondary-fixed-variant: '#5700c9'
  tertiary-fixed: '#b4ebff'
  tertiary-fixed-dim: '#3cd7ff'
  on-tertiary-fixed: '#001f27'
  on-tertiary-fixed-variant: '#004e5f'
  background: '#f8f9fb'
  on-background: '#191c1e'
  surface-variant: '#e1e2e4'
typography:
  h1-display:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '800'
    lineHeight: '1.2'
  h2-title:
    fontFamily: Pretendard
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.4'
  h3-subtitle:
    fontFamily: Pretendard
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
  body-main:
    fontFamily: Pretendard
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  body-sm:
    fontFamily: Pretendard
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-caps:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
  price-display:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '700'
    lineHeight: '1'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-margin: 20px
  stack-gap: 24px
  inline-gap: 12px
  card-padding: 20px
  section-padding: 40px
---

## Brand & Style

This design system targets Gen-Z Korean university students, bridging the gap between Samsung’s corporate reliability and the vibrant, trend-setting energy of campus life. The aesthetic is **Modern Minimalist with Glassmorphism**, prioritizing high-fidelity visual depth without clutter. 

The emotional goal is to feel "Premium yet Relatable." By utilizing semi-transparent layers, organic gradients, and precise typography, the UI moves away from a utility-first look toward a lifestyle-centric experience. The interface should feel like a high-end digital editorial tailored specifically for the academic and social journeys of a student.

## Colors

The palette centers on **Samsung Blue (#2167FF)**, but evolves it through the addition of **Electric Violet** and **Cyber Cyan**. These colors are primarily used in gradients to create a sense of movement and energy.

- **Primary:** Samsung Blue is the anchor, used for key actions and brand identification.
- **Secondary/Tertiary:** Used for high-impact promotional banners, badges, and "Community" highlights to differentiate from the "Store" sections.
- **Surface:** A "Cool Grey" base (#F8F9FB) ensures the white glass cards pop.
- **Accents:** High-saturation gradients are reserved for "Exclusive Student Offers" (단독 혜택) to drive conversion.

## Typography

The system uses a dual-font strategy to balance readability with a modern tech aesthetic. 

1.  **Pretendard:** The primary typeface for all Korean text. It is a variable font that ensures perfect legibility across all weights. Use `Medium (500)` for standard body text and `Bold (700)` for section headers.
2.  **Plus Jakarta Sans:** Reserved for English brand names (Galaxy, Buds, Book), numbers (Prices, Dates), and UI labels. This creates a geometric, "global" feel that resonates with tech-savvy students.

**Information Hierarchy:** Use `h1-display` for hero promotions like "개강 맞이 특가" (Back-to-school specials). Use `price-display` for all numerical currency values to make them stand out as tactile units.

## Layout & Spacing

The layout follows a **Fluid Grid** system tailored for mobile-first consumption. 

- **Margins:** A generous 20px side margin prevents content from feeling cramped.
- **Rhythm:** A base-8 scale is used. Vertical spacing between different sections (e.g., from "Store" to "Community") should be a consistent 40px to provide visual breathing room.
- **Grouping:** Use 12px for internal element spacing (icon to text) and 24px for component stacking (card to card).

## Elevation & Depth

This design system rejects traditional heavy shadows in favor of **Glassmorphism and Tonal Layering**.

- **Backdrop Blur:** All primary modals and bottom navigation bars must use a `20px` backdrop-filter blur with a `white/80%` opacity fill.
- **The "Inner Glow":** Cards should feature a 1px white border with 20% opacity. This simulates a glass edge, making the card look distinct against vibrant background gradients.
- **Soft Shadows:** Only used for floating action buttons (FAB) or primary product cards. Use a very large blur (30px) with a low opacity (8%) tinted with the Primary Blue color rather than pure black.

## Shapes

The shape language is "Organic Geometric." 

- **Standard Elements:** Buttons and input fields use a `0.5rem` (8px) radius.
- **Containers:** Product cards and community posts use a `1rem` (16px) radius to feel approachable and modern.
- **Feature Banners:** Large promotional headers use a `1.5rem` (24px) radius on bottom corners to create a "container" feel that leads the eye downward into the content.

## Components

- **Buttons:** Primary buttons use the `gradient_primary`. Secondary buttons should be transparent with a `1px` stroke or a light blue tint (10% opacity).
- **Glass Cards:** Used for product listings. They must include a subtle internal gradient and the "inner glow" border defined in the Elevation section.
- **Chips (Filter/Category):** Use "Pill" shapes. Active states use the Samsung Blue fill with white text; inactive states use a light grey stroke.
- **Bottom Navigation:** Fixed glass bar with blur. Active icons use a subtle glow effect underneath. Labels: 홈 (Home), 스토어 (Store), 커뮤니티 (Community), 프로필 (Profile).
- **Community Post Cards:** Minimalist layout. Use `body-sm` for the content preview and `label-caps` for metadata like "3분 전" (3 mins ago) or "조회수 1.2k" (Views 1.2k).
- **Input Fields:** Search bars should be "Super-Rounded" (Pill) with a search icon and the placeholder text "캠퍼스 단독 혜택을 찾아보세요" (Search for exclusive campus benefits).
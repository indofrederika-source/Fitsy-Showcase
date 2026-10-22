# Fitsy — Street-Editorial Fashion Archive & Digital Wardrobe

<div align="center">

<img src="icon-192x192.png" alt="Fitsy Logo" width="120" />

### **The tactile, high-fashion wardrobe curation platform and aesthetic style community.**  
*Infused with the rebellious energy of Gachiakuta street graffiti and the avant-garde couture elegance of JoJo's Bizarre Adventure.*

[![Next.js](https://img.shields.io/badge/Next.js-16.4-black?logo=next.js)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.0-61dafb?logo=react)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-3178c6?logo=typescript)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-v4-38bdf8?logo=tailwindcss)](https://tailwindcss.com/)
[![Tone.js](https://img.shields.io/badge/Audio-Tone.js-f59e0b)](https://tonejs.github.io/)
[![Framer Motion](https://img.shields.io/badge/Motion-Framer_Motion-ff0055?logo=framer)](https://www.framer.com/motion/)
[![Supabase](https://img.shields.io/badge/Supabase-PostgreSQL-3ecf8e?logo=supabase)](https://supabase.com/)
[![Capacitor](https://img.shields.io/badge/Capacitor-Mobile-119eff?logo=capacitor)](https://capacitorjs.com/)

[**🚀 Try Live Web Application (fitsy.vercel.app)**](https://fitsy.vercel.app) • [Product Overview](#-product-overview) • [Visual Identity](#-visual-identity--design-philosophy) • [Motion & Audio Engine](#-cinematic-physics-motion--procedural-audio-engine) • [Key Features](#-key-features) • [Architecture](#-architecture--technologies) • [Author](#-author--connect)

</div>

---

## 🌟 Product Overview

**Fitsy** is a modern fashion-technology platform designed to transform how individuals catalog, style, and share their physical wardrobes. Moving beyond generic, sterile SaaS interfaces, Fitsy blends high-end editorial magazine layout architecture with underground street-art dynamism.

Whether digitizing garments with on-device computer vision, crafting spatial editorial moodboards, experimenting with the multi-tier outfit builder, or sharing daily looks within a curated fashion community, Fitsy delivers an uncompromising, tactile experience across desktop, mobile web, and native mobile environments.

Experience the live application: **[fitsy.vercel.app](https://fitsy.vercel.app)**

---

## ⚡ Visual Identity & Design Philosophy

### *"Street-Editorial Manga Brutalism" (50% Gachiakuta × 50% JoJo's Bizarre Adventure)*

Fitsy rejects template-driven minimalist software tropes in favor of an artistic visual language built from two complementary counter-cultures:

1. **50% Gachiakuta (Brutalist Streetwear & Graffiti Energy):**
   * **Wildstyle Dripping Tag Brandmark**: A fluid graffiti handstyle logo with dripping spray paint physics (*paint drips*) dynamically synchronized with the interactive brand button.
   * **Die-Cut Contrast & Angular Framing**: Chamfered borders, deep ink-line accents, and razor-sharp editorial card cuts inspired by street sticker slaps.
   * **Atmospheric Micro-Mist**: Ultra-lightweight, 60–120 FPS GPU-optimized aerosol spray particles triggered during high-engagement interactions.

2. **50% JoJo's Bizarre Adventure (Haute-Couture Editorial & Atelier Hardware):**
   * **Runway Magazine Architecture**: High-contrast editorial typography, balanced whitespace, and asymmetrical dossier layouts inspired by high-fashion spreads.
   * **Tactile Hardware Elements**: Realistic morphing garment buttons (flannel, forged iron, industrial brushed metal, and high-saturation pigments).
   * **Haute-Couture Alabaster Canvas**: Pure white upgraded to an elegant, warm archival paper tone (`#F9F8F5`), framed with deep obsidian ink strokes (`#0E0E12`).
   * **Sleek Silhouette Iconography**: Tailored garment silhouettes for the 7 primary navigation hubs and 9 clothing categories.

---

## 💫 Cinematic Physics Motion & Procedural Audio Engine

Fitsy is engineered to feel like a living, tactile instrument rather than a static webpage. Every motion curve is driven by calibrated spring physics, and every interaction is rewarded with low-latency procedural audio:

### 🎬 High-Fidelity Physics & Motion System
* **Dynamic Rotating Brand Hardware**: The signature header button features interactive 360° spring-physics rotation with material morphing (flannel weave, forged raw iron, and bold editorial dyes).
* **Synchronized Paint-Flow Typography**: When the brand button morphs, the graffiti "FITSY" wordmark smoothly transitions its fill and dripping paint drops to match the new colorway in real time.
* **Fluid Sliding Outfit Builder**: The outfit customizer replaces abrupt state swaps with smooth horizontal sliding transitions. Garment boxes sit centered, flanked by internal left/right arrow controls for intuitive, frictionless piece cycling.
* **Magnetic Micro-Interactions**: Garment cards and interactive chips react to cursor weight with subtle spring elevation (`translateY(-2px)`) and elastic press squish (`scale(0.97)`).
* **Strict Modal Scroll Isolation**: Integrated Lenis kinetic smooth scrolling paired with zero-bleed modal scroll locks (`data-lenis-prevent`) prevents the underlying background from scrolling when exploring inspect panels or modals.
* **60–120 FPS GPU Compositing**: Animations strictly target `transform`, `opacity`, and GPU layers (`will-change: transform`) to prevent CPU reflows and eliminate layout thrashing.

### 🔊 Procedural Zero-Asset Sound Engine (Tone.js + Web Audio API)
Fitsy synthesizes its entire SFX palette algorithmically in the browser without downloading bulky MP3/WAV audio files:
* 💨 **Aerosol Spray Paint Mist**: NoiseSynth frequency sweep simulating real spray-can mist on filter selections and tag interactions.
* 🧵 **Crisp Fabric & Coat Whip**: Filtered pink and brown noise bursts capturing the tactile snap of tailored denim and outerwear.
* ⚡ **Tactile Zipper Tick & Slide**: Rapid descending pitch micro-clicks mimicking metal bag zippers and hardware fasteners.
* ✨ **Specular Crystal Chime**: FM-synthesized harmonic arpeggio (E6 → B6 → G#7) accentuating jewelry and luxury accessories.
* 👞 **Resonant Footwear Stomp**: Sub-bass membrane synth impact (G0) giving physical weight and grounding to boots and sneakers.
* 🔘 **Hardware Button Clink**: Dual-tone metallic resonance upon button rotation and material shifts.
* 💥 **Editorial Pose Impact**: Visceral, low-frequency cinematic boom celebrating outfit saves, lookbook exports, and archival milestones.

---

## 🚀 Key Features

### 1. 👗 Smart Wardrobe Digitization & Neural Vision
* **On-Device Background Removal**: Automatically segments clothing from raw user photos into transparent studio cutouts directly in the browser via WebAssembly & neural vision pipelines.
* **9 Primary Clothing Categories**: Comprehensive organizational taxonomy encompassing **Tops**, **Bottoms**, **Outerwear**, **Footwear**, **Bags**, **Accessories**, **Underwear / Nightwear**, **Full Body**, and **Swimwear**.
* **3-Tier Deep Taxonomy**: Granular categorization structure accommodating sub-types and hyper-specific garment cuts.
* **Dominant Color Extraction**: Intelligent pixel analysis extracts exact dominant color palettes and HEX codes for seamless wardrobe searching.
* **Fluid Multi-Currency Pricing**: Responsive price tagging supporting international currency standards with automated thousands-separators.

### 2. 🔘 Interactive Brand Hardware & Dynamic Morphing Engine
* **Rotating Physical Button**: An interactive garment button in the primary header that dynamically morphs across tactile material variants (cloth textures, forged iron/steel, and saturated editorial dyes) with kinetic spring rotation.
* **Synchronized Logo Color Flow**: The wildstyle dripping graffiti wordmark seamlessly follows the button's active material colorway.
* **Zero-Latency Dashboard Return**: Clicking the wordmark instantly brings the user back to the primary dossier view.

### 3. 🎨 Hierarchical Outfit Studio & Spatial Moodboard
* **Expanded Dual-Panel Outfit Builder**: Centered garment canvas flanked by integrated navigation controls and fluid sliding category transitions.
* **Aspect-Ratio Preserved HD Export**: 100% pixel-accurate moodboard rendering and export engine—eliminating image stretching or canvas distortion.
* **Freeform Canvas Studio**: Layering, rotation, scaling, and z-index ordering for custom fashion lookbooks.
* **Strict Flat Garment Cutouts**: Pure editorial styling without artificial drop shadows, preserving authentic clothing lines.

### 4. 🌐 Editorial Fashion Community & Social Archive
* **Explore Discovery Feed**: Curated, randomized lookbook streams delivering fresh creator inspirations on every session.
* **Fair-Exposure Friends Feed**: Intelligent round-robin delivery ensuring proportional creator exposure while preserving strict chronological update streams.
* **Garment Inspection**: Directly inspect and explore individual tagged garments from community lookbooks and moodboard posts.
* **Immersive Dynamic Header**: Auto-tucking navigation system that maximizes visual screen real estate during deep scrolling.

### 5. 🔍 Multi-Category Instant Search
* **In-Place Debounced Search**: Rapid filtering across Top Matches, Creator Accounts, Fashion Hashtags, and Community Posts without disruptive full-page popups.
* **Inline Social Graph**: Instant Follow/Unfollow capabilities directly within creator search results.
* **Archival Search History**: Local search persistence with instant clearance and trending aesthetic chips.

### 6. 📅 Outfit Calendar & Archival Wear Tracker
* **Daily Outfit Dossier**: Schedule upcoming outfits or archive daily wears to build an authentic personal style chronicle.
* **Cost-Per-Wear Analytics**: Track garment frequency and cost efficiency across seasons.
* **Trip Packing Assistant**: Curate multi-day travel wardrobes complete with automated packing checklists.

### 7. 📱 Progressive Web App & Native Mobile Runtime
* **Touch-Optimized Gestures**: Native-feeling mobile gestures, rubber-band overscroll resistance, and bottom drawers.
* **Bilingual Localization**: Instant client-side switching between **English** and **Indonesian (Bahasa Indonesia)**.
* **Cross-Platform Mobile Container**: Seamless native deployment on iOS and Android via Capacitor CLI.

---

## 🛠️ Architecture & Technologies

Fitsy is engineered for uncompromising performance, sub-millisecond perceived latency, and 60–120 FPS rendering:

| Domain | Technology | Implementation Details |
|---|---|---|
| **Core Framework** | [Next.js 16.4](https://nextjs.org/) (App Router) | Full-stack server architecture, Server Actions & optimized bundling |
| **UI Library** | [React 19](https://react.dev/) + [TypeScript 5](https://www.typescriptlang.org/) | Type-safe declarative components and concurrent rendering |
| **Design System** | [Tailwind CSS v4](https://tailwindcss.com/) | Modern atomic CSS, CSS variables, and bespoke design tokens |
| **Motion & Physics** | [Framer Motion](https://www.framer.com/motion/) + [GSAP](https://greensock.com/) | High-performance spring physics, GPU compositing & timeline choreography |
| **Smooth Scrolling** | [@studio-freight/lenis](https://lenis.darkroom.engineering/) | Inertial kinetic smooth scrolling with strict modal isolation |
| **Tactile Audio** | [Tone.js](https://tonejs.github.io/) + Web Audio API | Procedural, zero-network micro-sound synthesis |
| **Expressive Canvas** | [Rough.js](https://roughjs.com/) + [Perfect Freehand](https://github.com/steveruizok/perfect-freehand) | Algorithmic ink strokes, hand-drawn contours & grunge borders |
| **Database & Auth** | [Supabase](https://supabase.com/) (PostgreSQL) | Row Level Security (RLS), real-time indexing & cryptographic sessions |
| **Client-Side AI** | [Transformers.js](https://huggingface.co/docs/transformers.js) + HTML5 Canvas | Local on-device background segmentation & color analysis |
| **Mobile Runtime** | [Capacitor CLI](https://capacitorjs.com/) | Native Android & iOS cross-platform compilation bridges |
| **Hosting & Edge** | [Vercel](https://vercel.com/) | Global Edge network, asset optimization & automated CI/CD pipelines |

---

## 🔒 Proprietary & Closed-Source Notice

**Copyright © 2026 Fitsy. All rights reserved.**

Fitsy is a proprietary commercial product. The full codebase, database schemas, internal algorithms, and brand assets are maintained in a secure private repository.

* For recruitment, technical evaluations, partnerships, or sample access, please contact the author.

---

## 👤 Author & Connect

* **Creator**: [@indofrederika-source](https://github.com/indofrederika-source)
* **Live Product**: [https://fitsy.vercel.app](https://fitsy.vercel.app)
* **Contact**: [indo.frederika@gmail.com](mailto:indo.frederika@gmail.com)

---

<div align="center">
Crafted with passion for street culture, haute-couture fashion, and state-of-the-art web engineering. 🧵✨
</div>

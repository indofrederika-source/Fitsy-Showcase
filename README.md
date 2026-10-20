# Fitsy — Smart Virtual Wardrobe, AI Stylist & Fashion Community

<div align="center">

<img src="icon-192x192.png" alt="Fitsy Logo" width="120" />

### **Your personal digital wardrobe, intelligent AI stylist, and aesthetic fashion community platform.**

[![Next.js](https://img.shields.io/badge/Next.js-16.4-black?logo=next.js)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.0-61dafb?logo=react)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-3178c6?logo=typescript)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-v4-38bdf8?logo=tailwindcss)](https://tailwindcss.com/)
[![Supabase](https://img.shields.io/badge/Supabase-PostgreSQL-3ecf8e?logo=supabase)](https://supabase.com/)
[![Capacitor](https://img.shields.io/badge/Capacitor-Mobile-119eff?logo=capacitor)](https://capacitorjs.com/)

[**🚀 Try Live Web Application (fitsy.vercel.app)**](https://fitsy.vercel.app) • [Product Overview](#-product-overview) • [Key Features](#-key-features) • [Architecture](#-architecture--technologies) • [Author](#-author)

</div>

---

## 🌟 Product Overview

**Fitsy** is a modern fashion-technology platform designed to transform how individuals catalog, style, and share their everyday wardrobes. Inspired by contemporary editorial lookbooks and high-fashion aesthetics, Fitsy bridges personal closet inventory management with generative AI styling and an engaging, community-driven social discovery engine.

Whether organizing garments, assembling visual moodboards, receiving color-theory recommendations, or sharing daily outfit inspiration with friends, Fitsy delivers a seamless experience across desktop, mobile web, and native mobile environments.

Experience the live application: **[fitsy.vercel.app](https://fitsy.vercel.app)**

---

## 🚀 Key Features

### 1. 👗 Smart Wardrobe Digitization & Vision AI
* **Instant Background Removal**: Automatically segments clothing from raw photos into crisp, transparent PNG cutouts directly in the browser using on-device neural vision models.
* **Dominant Color Extraction**: Intelligent pixel analysis extracts exact dominant color palettes and HEX codes for automated categorization.
* **AI Auto-Categorization**: Zero-shot image classification automatically categorizes items into Tops, Bottoms, Outerwear, Footwear, Headwear, and Accessories.
* **Custom Categories & Tags**: Create tailored categories, custom sub-tags, and bespoke icons to match personal closet organization styles.

### 2. 🎨 Hierarchical Outfit Canvas & Moodboard Studio
* **5-Slot Anatomical Hierarchy**: Garments intuitively snap into their natural body positions (`Headwear` → `Tops` → `Bottoms` → `Shoes` → `Accessories`), regardless of the order they are selected.
* **Freeform Moodboard Studio**: Collage canvas featuring layered elements, stickers, background textures, scaling, rotation, and high-resolution export.
* **One-Tap Outfit Loading**: Save favorite combinations to your personal style vault and reload them onto the canvas instantly for fast styling.

### 3. 🤖 Intelligent AI Stylist & Color Harmony Engine
* **Color Theory Algorithms**: Real-time outfit synergy calculations powered by complementary, analogous, monochromatic, and neutral color rules.
* **Aesthetic Filters**: Discover outfit ideas tailored to specific aesthetics like *Minimalist*, *Streetwear*, *Clean Fit*, *Old Money*, and *Casual*.
* **Visual Match Score**: Transparent AI scoring that explains *why* garments complement each other visually.

### 4. 🌐 Aesthetic Fashion Community & Social Feed
* **Dynamic Explore Discovery**: Real-time randomized feed that delivers fresh, inspiring creator lookbooks on every session.
* **Fair-Exposure Friends Feed**: Intelligent round-robin distribution that rotates between friends while preserving 100% chronological order for each friend's updates.
* **Creator Interactions**: Like, comment, share, bookmark, and inspect tagged wardrobe items directly from community outfits.
* **Smart Immersive Header**: Dynamic scroll detection automatically tucks the navigation away on scroll down for maximum viewing immersion, and smoothly reveals when scrolling up.

### 5. 🔍 Multi-Category Search Engine
* **Live Instant Search**: Real-time debounced search bar with active category filtering:
  * **Top**: Curated compilation of the most relevant accounts, hashtags, and posts.
  * **Accounts**: Search creators by username and display name with inline Follow/Unfollow actions.
  * **Hashtags**: Style tags with live post counts (e.g., `#Streetwear` • `1.4k posts`).
  * **Posts**: Keyword and caption search across all community photos and moodboards.
* **Search History & Trending Suggestions**: Local search history with quick-clear options and instant access to trending style chips.

### 6. 📅 Outfit Calendar & Travel Packing Assistant
* **Daily Outfit Logging**: Schedule outfits in advance or log what you wore each day to build a personal wear history and style archive.
* **Closet Utilization Analytics**: Track cost-per-wear and discover which items in your closet get the most love.
* **Trip Packing Assistant**: Plan multi-day itineraries with destination weather forecasts and automated wardrobe packing checklists.

### 7. 🔔 Push Notifications & Activity Alerts
* **Web Push & Service Worker**: Native browser push notifications powered by the Web Notifications API and Service Workers.
* **Granular Alert Preferences**: Toggle notifications for likes, comments, new followers, friend uploads, and daily outfit scheduling reminders.

### 8. 📱 Progressive Web App & Fluid Mobile Experience
* **Touch-First Design**: Engineered for mobile viewports with smooth gesture interactions, bottom sheets, and responsive touch controls.
* **Bilingual UI**: Seamless, instant switching between **English** and **Indonesian (Bahasa Indonesia)**.
* **Adaptive Theming**: Smooth system-level Dark and Light mode support across all screens and canvases.

---

## 🛠️ Architecture & Technologies

Fitsy is built with a modern, high-performance web and mobile stack:

| Layer | Technology | Purpose |
|---|---|---|
| **Core Framework** | [Next.js 16](https://nextjs.org/) (App Router, Server Actions) | Full-stack server-rendered architecture and routing |
| **UI Library** | [React 19](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/) | Declarative component model and type safety |
| **Design System** | [Tailwind CSS v4](https://tailwindcss.com/) + [next-themes](https://github.com/pacocoursey/next-themes) | Custom modern styling and fluid theme switching |
| **Database & Cloud** | [PostgreSQL](https://www.postgresql.org/) via [Supabase](https://supabase.com/) | Relational database, indexing, and Row Level Security |
| **Authentication** | [Supabase Auth](https://supabase.com/auth) & Session Cookies | Secure OAuth (Google) and cryptographic session management |
| **Icons** | [Lucide React](https://lucide.dev/) | Clean, consistent vector iconography |
| **Client-Side AI** | [Transformers.js](https://huggingface.co/docs/transformers.js) + HTML5 Canvas | In-browser background segmentation and color analysis |
| **Cloud AI** | [Google Gemini](https://ai.google.dev/) API | Advanced fashion recommendations and caption analysis |
| **Mobile Runtime** | [Capacitor CLI](https://capacitorjs.com/) | Cross-platform native Android container and bridges |
| **Edge Infrastructure** | [Vercel](https://vercel.com/) | Edge hosting, global CDN, and automated CI/CD |

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

<div align="center">
Designed and crafted with passion for fashion curation, personal style, and modern engineering. 👗✨
</div>

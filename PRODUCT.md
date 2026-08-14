# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Existing static site: HTML5, CSS3 (native variables, Grid, Flexbox), vanilla JavaScript, hosted on GitHub Pages. No framework.

## Users

- Recruiters and technical hiring managers evaluating Juan Calle Rosales as a software developer (web & mobile).
- Potential clients / small businesses (e.g., restaurants) evaluating Calletano POS as a product he builds and ships.
- Developer peers and collaborators.

## Product Purpose

Professional portfolio for Juan Anthony Calle Rosales, "Desarrollador de Software" focused on web and mobile. Purpose: present his profile, technical skills, projects (flagship: Calletano POS), work experience, education, certifications and contact so visitors understand what he builds and how to reach him. Success = quality job opportunities and product/contract inquiries.

## Positioning

A developer who builds complete, synchronized real-time systems end to end: a restaurant POS shipped as a Windows installer (Electron), a waiter mobile app (React Native), a public web menu on Firebase, all sharing one real-time API (Socket.IO). He transforms manual business processes into software (salon management, payments, inventory, reports).

## Operating Context

- Site language: Spanish (es_PE, Piura/Trujillo, Perú).
- Google Analytics tag G-QMWF35M72H present in head.
- GitHub Pages deployment: https://juancall.github.io/Portafolio-Web/
- Users reach it from the CV (printed header) and LinkedIn/GitHub profiles; many visits on mobile.
- Dark theme default, light theme optional via toggle; persisted in localStorage; follows prefers-color-scheme on first visit.

## Capabilities and Constraints

- One-page scroll layout: hero, about, skills, projects, trajectory, contact/footer.
- Sections content reflects the updated CV: profile as web/mobile developer (React, Node.js, Express, Socket.IO, Electron, React Native/Expo, Firebase, SQLite, Bootstrap, Chart.js, Vite, Git/GitHub, Excel); projects Calletano POS and Calletano Web; experience SILSAN (practicante) and I.E.P. Divino Jesús (docente de verano); education UPN 2021–2026; certifications CCNA 2025, Data Science intro 2024, CLA C 2022; languages ES native / EN A2.
- Content in Spanish; project/tool names are proper nouns and should not be translated.
- Contact: email juancallerosales19@gmail.com, WhatsApp +51 979 363 149, LinkedIn, GitHub, Instagram.
- Download CV button linking to a CV file in docs/ (currently docs/CV - Calle Rosales.docx; old docs/CV_Juan_Calle.pdf was deleted from the repo).
- SEO assets present: robots.txt, sitemap.xml, favicon.svg, JSON-LD Person schema, Open Graph/Twitter meta, canonical URL. Keep them working.
- Performance practices in current code: lazy-loaded images, content-visibility, preconnects, fetchpriority on hero image.
- Accessibility in current code: skip link, aria labels, focus-visible, reduced-motion support. Keep them.

## Brand Commitments

- Name: Juan Anthony Calle Rosales.
- Role title: "Desarrollador de Software" (web y móvil) — React · Node.js · React Native · Firebase (per CV header).
- Spanish as the voice of the site.
- User-granted redesign permission: full freedom over typography, colors, layout and visuals ("TODO PUEDES CAMBIAR"), as long as the result matches the CV.

## Evidence on Hand

- CV source of truth: docs/CV - Calle Rosales.docx (extracted text used for content).
- Project screenshots in img/: Sistema-Reservas.jpg, Web-CalletanoRestaurant.jpg, Portafolio-Web.jpg, SistemaPOS_Calletano.jpg, SistemaSmart-Farmacia.jpg, FerretSmart.jpg, perfil.jpg.
- Real project URLs: github.com/JuanCall, calletano-restaurant.web.app, juancall.github.io/Portafolio-Web/.
- No fabricated testimonials, metrics, clients, or claims. User confirmed (2026-08-13) that Sistema-Transaccional-Reservas-Hotel, SistemaSmart and FerretSmart are incomplete projects removed from his GitHub; they are excluded from the portfolio. Portafolio-Web is kept as the only additional project.

## Product Principles

1. The work is the proof: lead with the real-time Calletano POS system and what it does.
2. Truth from the CV: every claim traceable to docs/CV - Calle Rosales.docx; never invent experience or numbers.
3. Spanish first, with proper nouns (product/tool names) kept as-is.
4. Fast and accessible static page: respects reduced motion, keyboard focus, responsive mobile-first, performance budget.
5. Clear path to contact and CV download from the first viewport.

## Accessibility & Inclusion

Existing site already implements skip-link, visible focus, aria attributes, and prefers-reduced-motion support; the redesign must preserve these. Spanish content.

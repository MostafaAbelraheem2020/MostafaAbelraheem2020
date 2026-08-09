# Hi, I'm Mostafa Abdelraheem

**Full-Stack Engineer & AI Automation Specialist**  
Next.js · TypeScript · Node.js · SaaS · AI Agents · n8n Automation

I build production-ready web platforms, SaaS products, and AI-powered automation systems focused on scalable architecture, performance, bilingual experiences, and real business workflows.

**Portfolio:** [mostafa-abdelrahem-portfolio.vercel.app](https://mostafa-abdelrahem-portfolio.vercel.app)

---

## About Me

I'm a Full-Stack Engineer based in Egypt. My work covers:

- Full-stack web development with **Next.js, React, TypeScript, and Node.js**
- SaaS platforms, dashboards, e-commerce flows, and installable **PWAs**
- REST APIs, authentication, and server-side business logic
- **AI agents**, chatbots, generative AI integrations, and secure webhook architectures
- **n8n** workflow automation connected to WordPress, Airtable, Telegram, WhatsApp, and custom APIs
- Multilingual Arabic/English (RTL/LTR), SEO, and performance optimization
- Deployment on **Vercel**, VPS, and Cloudflare-backed environments

Most production and client repositories are kept **private** to protect source code and client IP. This profile documents the systems I build; live demos and production links are provided for review.

---

## Tech Stack

| Area | Technologies |
|---|---|
| Frontend | Next.js, React, TypeScript, JavaScript, Tailwind CSS, Framer Motion |
| Backend | Node.js, Next.js API Routes, REST APIs, authentication, server-side business logic |
| Databases | MongoDB, PostgreSQL, Firebase / Firestore |
| AI & Automation | AI Agents, n8n, OpenAI / Gemini, webhooks, WhatsApp & Telegram integrations |
| Infrastructure | Vercel, VPS, Cloudflare, GitHub, Docker where applicable |
| Product Engineering | SaaS, PWA, SEO, multilingual apps, RTL/LTR, performance optimization |

---

## Services

- **Full-Stack Web Platforms** — Next.js / React / TypeScript products, dashboards, SaaS tools, e-commerce, bilingual websites
- **n8n Workflow Automation** — scheduled workflows, webhooks, publishing pipelines, notifications, operational automations
- **AI Chatbots & Agents** — website assistants, lead capture, memory-enabled agents, multilingual response behavior
- **Generative AI Integrations** — OpenAI/Gemini features, structured JSON output, prompt systems, content automation
- **API & Webhook Automation** — CRM, WordPress, Telegram, WhatsApp, Airtable, and custom backend integrations
- **SEO & Content Automation** — technical SEO, metadata, structured data, safe publishing pipelines

---

## Projects Overview

### AI Platforms & Agents

#### Assistants Pro AI | Multi-Agent Business Platform

Assistants Pro AI is a multi-tenant platform for packaging business AI agents under one Founder/Tenant product surface. It includes a public agent catalog, demo request funnels, scoped authorization, agent registry/subscriptions, and production workflows transferred for Dawrak (clinic) and Marshal (ecommerce) onto a shared n8n infrastructure.

**Goal / positioning**
- Package Agents as products, not one-off chatbots
- Separate Founder/Tenant surfaces and keep production flags default-off until authorized
- Keep Agent cores (Dawrak/Marshal) separate while sharing platform services

**Key features**
- Multi-tenant organization model with subscription-scoped Agents
- Public agent catalog driven by a Registry instead of hard-coded pages
- Demo access lifecycle with hash-only grants, expiry, and scoped usage
- Founder and Tenant dashboards with Agent workspaces and settings
- Dawrak clinic module and Marshal ecommerce module on one platform
- Verified channel-resolver contracts for endpoint/participant isolation

**Technical stack**  
Next.js 16 (platform-web App Router) · React 19 + TypeScript · Tailwind CSS design system · Monorepo packages (@assistant-pro-plus/*) · n8n workflow orchestration on VPS · MongoDB Atlas foundation (synthetic/local contracts) · Vitest + evidence-gated delivery process · Vercel hosting for public preview

**Engineering strategies**
- Transfer workflow authority into the platform tree with rollback backups
- Evidence-first delivery: every APP accepted after independent verification
- UI originates from Stitch, then applied with a locked Tailwind design system

**Performance**
- Next.js App Router with modular route groups
- Local package boundaries to keep Agent logic testable
- Feature flags avoid shipping unfinished operational surfaces
- Vitest coverage across identity, authz, registry, demo, and UI packs

**Security & reliability**
- Hash-only demo grants and expiry windows
- Scoped RBAC with deny-by-default checks
- Cross-tenant isolation fixtures in Registry/Resolver tests
- Secrets stay outside planning/public portfolio artifacts

- **Live / demo:** https://assistants-pro-ai.vercel.app/
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/12

---

#### Dawrak | AI Clinic Front-Desk Agent

Dawrak is a digital clinic receptionist Agent that answers approved FAQs, collects appointment requests, escalates to humans, and supports follow-up through dashboard operations. It is productized with bilingual UX, n8n production workflows, and integrated as a first-class Agent inside Assistants Pro AI.

**Goal / positioning**
- Sell a business outcome (digital receptionist), not a generic medical chatbot
- Keep Sheets operational until a verified Atlas migration window
- Transfer workflow source authority into the platform with backup/rollback

**Key features**
- Clinic reception positioning: FAQ + appointment request + human handoff
- Safety boundaries against diagnosis/prescription claims
- Beta access chat flows for controlled demos
- Landing conversion page with lead webhook contract
- n8n clinic workflow family transferred to platform agents/dawrak
- Synthetic parity module on Assistants Pro AI (FAQ/appointment/handoff/locale)

**Technical stack**  
Next.js 16 + React 19 clinic frontend · n8n clinic workflow orchestration · OpenAI/LLM assisted conversation flows · Google Sheets operational persistence (pre-Atlas cutover) · Assistants Pro AI platform packages · Tailwind CSS + Framer Motion · Vercel hosting for product surfaces

**Engineering strategies**
- Use Assistants Pro AI for packaging, demos, and tenant workspaces
- Enforce honesty chips and safety guardrails in chat UX

**Performance**
- Workflow source centralized for faster iteration and rollback
- Synthetic parity tests before live channel expansion
- Feature-flagged live chat to avoid accidental production exposure
- Reusable Agent packaging instead of rebuilding clinic bots per client

**Security & reliability**
- No unsupported medical claims in agent responses
- Lead form fails closed when webhook destination is unconfigured
- Secrets and channel credentials stay out of public artifacts
- Compat redirects and live flags remain default-off unless authorized

- **Live / demo:** https://assistants-pro-ai.vercel.app/agents/dawrak
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/13

---

### Production Web Platforms

#### Voyajar | Travel Discovery & Affiliate Platform

Voyajar is a production travel discovery and affiliate platform with bilingual Arabic/English experiences, hotel and flights discovery, destination guides, SEO-focused content, and an admin CMS covering media, affiliate links, click logging, users, and performance analytics.

**Goal / positioning**
- Blend SEO content (guides/blog) with transactional search widgets
- Centralize affiliate tracking for measurable conversion loops
- Keep CMS tooling in-product for fast content operations

**Key features**
- English-first global travel discovery with Arabic localization
- Hotel search experience with destination-oriented browsing
- Flights search surfaces for high-intent traffic
- SEO-ready destination guides and blog content hubs
- Affiliate link management with click logging
- Admin dashboard for hotels, destinations, media, and users

**Technical stack**  
Next.js 16.2.9 (App Router) · React 19.2.5 · TypeScript · next-intl for multilingual routing/content · NextAuth.js v5 · MongoDB 7 · TanStack React Query · Framer Motion + Tailwind CSS · OpenAI integrations for content/workflows where used · Vercel production hosting

**Engineering strategies**
- Ship bilingual UX from day one for MENA + global traffic
- Use analytics surfaces to guide destination and campaign priorities

**Performance**
- Next.js App Router with modern React 19 rendering
- React Query for efficient client data states
- Optimized media handling in CMS/media library
- Route-level code splitting for search and content hubs

**Security & reliability**
- NextAuth-protected admin operations
- Audit log for sensitive CMS actions
- Controlled affiliate redirect/click logging
- Environment-separated production credentials

- **Live / demo:** https://www.voyajar.com/
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/14

---

#### Bayoumy Co. | مبرمج ويب - تصميم مواقع شركات

A premium, bilingual (Arabic/English) corporate platform built for Mohamed Abdewahab Bayoumy Company. منصة احترافية لشركة محمد عبد الوهاب بيومي للمقاولات، تم تطويرها بأحدث تقنيات البرمجة لضمان أداء عالٍ وتصدر نتائج البحث.

**Goal / positioning**
- Hybrid Rendering: SSG for content pages with Client-side interactivity
- Edge Middleware: Security headers and route protection
- Dynamic i18n: Client-side language switching with SEO-ready structure

**Key features**
- Advanced Internationalization (i18n) with Native Bilingual Support (AR/EN)
- SEO-First Localization with dynamic hreflang tags
- SSG (Static Site Generation) for 60+ projects and news items
- Automated Visual Optimization (AVIF/WebP) with cache-control
- Hardware-accelerated animations via Framer Motion
- Comprehensive Metadata & Structured Data (JSON-LD) for all routes

**Technical stack**  
Next.js 16.1.6 (App Router, Server Components, Streaming) · React 19.2.4 (Latest React with Hooks and Context API) · TypeScript 5.9.3 (Strict type safety and improved DX) · Tailwind CSS 4.1.18 (Modern utility-first styling with @tailwindcss/postcss) · Framer Motion 12.34.0 (Advanced motion design and hardware-accelerated animations) · Lucide React 0.564.0 (Modern SVG icon library) · Resend API 6.9.3 (Scalable email delivery system) · Sharp 0.34.5 (High-performance image processing) · Swiper 12.1.1 (Interactive and touch-responsive carousels) · ESLint 10 & Prettier (Strict code quality and formatting)

**Engineering strategies**
- Optimized Asset Pipeline: Next/Image with AVIF/WebP support
- Component-based Architecture: Highly modular and reusable React components
- Motion-First UX: Seamless transitions and hardware-accelerated animations
- Anti-Spam Security: Honeypot fields and rate-limiting for all forms

**Performance**
- Static Site Generation (SSG) for sub-second page loads
- Advanced Image Optimization using Next.js Image component
- Code-splitting and Lazy Loading for non-critical assets
- Font optimization via next/font with local storage caching

- **Live / demo:** https://www.mabdelwahabconstructions.com/
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/1

---

#### PharmaFlow | انشاء متجر اليكتروني صيدلي

A cutting-edge, production-ready Pharmacy SaaS solution. حل تقني متطور لإنشاء المتاجر الإلكترونية للصيدليات، يدعم اللغتين العربية والإنجليزية مع نظام إدارة متكامل وبرمجة عالية الأداء.

**Goal / positioning**
- Hybrid Data Enrichment: Scraped data merging with fuzzy-matching for master catalog enrichment
- PWA Lifecycle management: Seamless offline access and background refresh capabilities
- Edge Middleware Routing: Security headers and locale-aware redirection logic

**Key features**
- Advanced Internationalization (i18n) with Native RTL/LTR Support (AR/EN)
- Progressive Web App (PWA) - Fully installable on iOS and Android with offline capabilities
- Master Catalog Scaling with fuzzy-matching algorithms for multi-source data enrichment
- Real-time Push Notifications via Web-push API for order and consultation updates
- Secure Administrative Dashboard for Order Tracking and Automated Stock Control
- Professional Digital Prescription Review Interface for licensed pharmacists

**Technical stack**  
Next.js 15.2.1 (App Router, Server Components, Streaming, Route Handlers) · React 19.2.4 (Latest React with Concurrent Rendering and Action Hooks) · TypeScript 5.8.0 (Strict type safety and improved DX for enterprise applications) · Tailwind CSS 4.0.0 (Modern utility-first styling with native PostCSS support) · MongoDB 7.1.1 (High-performance document-oriented cloud database) · Mongoose 9.3.2 (Elegant MongoDB object modeling and schema validation) · NextAuth.js 5.0.0-beta.30 (Modern authentication and session management) · Next-intl 4.8.3 (Dynamic localization and SEO-ready i18n structure) · Cloudinary 2.9.0 (Advanced media management and global CDN delivery) · Web-push 3.6.7 (Scalable push notifications system for PWA)

**Engineering strategies**
- Decoupled Micro-Scripts: Independent scripting layer for safe data ingestion
- Modular UI Componentry: Highly reusable React 19 components inspired by shadcn/ui
- SEO-First Architecture: Bilingual metadata generation for all dynamic routes
- Resilient Auth Implementation: Combined JWT and Database strategies for session persistence

**Performance**
- Server Components (RSC) for zero-bundle-size rendering logic
- Cloudinary-backed Next/Image for optimized responsive assets
- Aggressive route prefetching for instant navigation
- Optimized MongoDB indexing for sub-second catalog queries

- **Live / demo:** https://pharmacy-website-pwa.vercel.app/en
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/2

---

#### Nuzlaa | مبرمج ويب - منصة حجز فنادق

A high-performance travel affiliate platform. نُزلاء هي منصة سياحية عالمية تعتمد على تقنيات الذكاء الاصطناعي في البحث وتوفير أفضل العروض، تم برمجتها لتكون الأسرع في فئتها.

**Goal / positioning**
- Localized Affiliate Marketing: Arabic-first approach for MENA markets
- Scalable Content Pipeline: Dynamic NoSQL schema for global destinations
- Performance-First Architecture: Hybrid rendering with aggressive caching

**Key features**
- Advanced Hotel Search Engine with global availability
- International Flight Search & Comparison integration
- Dynamic Destination Guides with SEO-optimized content
- Smart Affiliate Link Management System for 28+ programs
- Native Multi-language Support (i18n) focused on Arabic and English
- High-performance SSG & ISR for sub-second page loads

**Technical stack**  
Next.js 16.2.3 (App Router, Server Components, Streaming) · React 19.2.5 (Latest React with Server Actions) · TypeScript 5.9.3 (Strict type safety and robust DX) · Tailwind CSS 4.2.2 (Modern utility-first styling with PostCSS) · MongoDB 7.1.1 (High-performance NoSQL document storage) · Next-Intl 4.9.1 (Comprehensive i18n management) · Lucide React 1.8.0 (Modern SVG icon library) · Sharp 0.34.5 (High-performance image optimization) · Next-PWA 5.6.0 (Zero-config PWA plugin) · Vitest 3.2.4 (Fast unit testing framework)

**Engineering strategies**
- Universal Search Experience: Unified interface for multi-provider bookings
- SEO Domination: Advanced metadata, structured data, and i18n routing
- Mobile App Readiness: PWA integration for cross-platform accessibility

**Performance**
- Incremental Static Regeneration (ISR) for real-time content updates
- Server-side Image Optimization using Sharp and Next/Image
- Reduced Bundle Size with Tailwind 4 and tree-shaken Lucide icons
- Streaming and Suspense for asynchronous data fetching

- **Live / demo:** https://nuzlaa.com/
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/3

---

### AI Automation & Workflow Systems

#### Jobs Publishing Agent | AI WordPress Automation Workflow

A high-volume production n8n automation that discovers job posts, extracts links with custom JavaScript, prevents duplicates through Airtable, uses an AI agent with structured output parsing to rewrite Arabic SEO job content, publishes to WordPress, uploads featured images, sends Telegram notifications, and forwards structured data to an external platform webhook.

**Goal / positioning**
- Used custom parsing instead of fragile manual copy/paste workflows
- Stored unique hashes in Airtable to prevent duplicate WordPress publishing
- Constrained AI output with a manual schema for reliable automation

**Key features**
- Scheduled job discovery workflow running in production
- Custom JavaScript parser for extracting job links and titles
- URL normalization and canonical key generation
- Duplicate detection using Airtable search records
- AI Agent for factual extraction and Arabic SEO rewriting
- Structured Output Parser for predictable job data

**Technical stack**  
n8n 2.6.4 (workflow orchestration) · OpenAI GPT-4.1 Mini (content extraction and rewriting) · n8n LangChain AI Agent (tool-enabled job extraction) · Structured Output Parser (schema-constrained AI result) · HTTP Request Tool (AI-controlled source fetching) · JavaScript Code Nodes (parsing, hashing, categorization) · Airtable (duplicate tracking and record storage) · WordPress REST API (post and media publishing) · Telegram Bot API (channel notification) · External Webhook Bridge (structured data forwarding)

**Engineering strategies**
- Kept factual fields intact while rewriting content into original Arabic copy
- Added SEO-focused rules and JobPosting JSON-LD generation for search visibility
- Split publishing into content creation, media upload, featured image update, and notification steps
- Added external webhook forwarding to reuse the generated structured job data elsewhere

**Performance**
- Runs automatically on a short schedule without manual operation
- Duplicate checks happen before costly AI generation
- Canonical URL hashing keeps lookup data compact
- Single workflow handles discovery, enrichment, publishing, and notifications

**Security & reliability**
- Credentials are managed inside n8n and kept out of public project data
- Duplicate gate prevents accidental content spam
- Structured parser reduces malformed AI data risk
- External webhook forwarding uses server-side authentication

- **Live / demo:** https://jobsgatee.com/
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/4

---

#### AI Tech Blog Harvester | RSS to Next.js Publishing Pipeline

A daily AI content automation pipeline that monitors technology news through RSS, checks existing portfolio blog posts, selects a new article, fetches the source page, extracts the original image, generates bilingual English/Arabic content with AI, validates structured JSON output, and publishes directly to a protected Next.js blog API.

**Goal / positioning**
- Used RSS as the discovery layer and the portfolio API as the source of truth for duplicates
- Generated deterministic slugs from article title and source data
- Validated required AI fields before sending any content to production

**Key features**
- Daily scheduled content automation workflow
- RSS feed monitoring for technology news
- Existing blog check through a custom Next.js API
- Duplicate prevention by generated slug and title comparison
- Source article HTML fetching for richer context
- Open Graph and Twitter image metadata extraction

**Technical stack**  
n8n 2.6.4 (daily workflow automation) · RSS Feed Read Node (source monitoring) · OpenAI GPT-4o Mini (bilingual content generation) · JavaScript Code Nodes (slugging, duplicate checks, validation) · HTTP Request Nodes (source fetch and API publish) · Next.js Blog API (custom publishing endpoint) · HTML Metadata Extraction (original image discovery) · JSON Payload Validation (safe publishing guard) · Docker VPS (self-hosted n8n runtime)

**Engineering strategies**
- Required source image extraction to avoid publishing weak visual content
- Kept AI output constrained to JSON for reliable downstream processing
- Separated article discovery, writing, validation, and publishing into clear workflow stages
- Used a protected API endpoint instead of direct database writes

**Performance**
- Runs on a daily schedule instead of polling continuously
- Stops early when no new article is available
- Checks duplicates before calling the AI model
- Builds compact JSON payloads for API publishing

**Security & reliability**
- Protected blog publishing API
- No public exposure of API keys or webhook secrets
- Validation layer prevents malformed AI output from being published
- Server-side workflow execution on a private n8n instance

- **Live / demo:** https://mostafa-abdelrahem-portfolio.vercel.app/blog
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/5

---

#### AI Portfolio Assistant | n8n Chatbot Agent

A production AI assistant connected to a Next.js portfolio through secure n8n webhooks. The workflow receives visitor questions, validates requests, routes messages to an AI agent with memory, returns JSON responses to the website, and sends WhatsApp notifications for lead awareness. It demonstrates real chatbot engineering across frontend UI, server APIs, n8n automation, AI models, and notification systems.

**Goal / positioning**
- Separated the website chat UI from the automation brain through a secure webhook contract
- Used n8n as the orchestration layer so the bot can be changed without redeploying the frontend
- Added request validation before the AI agent to prevent unauthorized webhook usage

**Key features**
- Production webhook-based AI chatbot backend
- Secure request validation using header/secret checks
- AI Agent powered by OpenAI chat models
- Window Buffer Memory for contextual conversations
- Arabic and English response behavior based on visitor language
- JSON response flow back to the Next.js portfolio frontend

**Technical stack**  
n8n 2.6.4 (workflow orchestration and webhook automation) · Next.js API Route (chat endpoint and fallback layer) · OpenAI Chat Model (AI response generation) · n8n LangChain AI Agent (agent orchestration) · Window Buffer Memory (short-term conversation context) · HTTP Request Node (WhatsApp notification integration) · Respond to Webhook (structured JSON response) · Docker VPS Deployment (self-hosted automation runtime) · Header-based authentication (secure webhook validation)

**Engineering strategies**
- Kept a local fallback inside the Next.js API route for resilience during automation downtime
- Used memory to make visitor conversations more contextual
- Connected notifications to turn chatbot conversations into lead awareness events
- Kept sensitive keys and webhook secrets out of public portfolio content

**Performance**
- Webhook response mode returns directly to the frontend
- Concise assistant prompt reduces model latency
- Fallback route avoids a broken user experience if n8n is unavailable
- JSON response body keeps the frontend integration lightweight

**Security & reliability**
- Header-based secret validation before running the AI agent
- No public exposure of API keys or webhook secrets
- Server-to-server communication between Next.js and n8n
- Safe local fallback for unavailable automation services

- **Live / demo:** https://mostafa-abdelrahem-portfolio.vercel.app/
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/6

---

### Client & Product Websites

#### Mr. Ali Elgabry Portfolio

بورتفوليو احترافي للأستاذ علي الجبري، خبير اللغة العربية، يعتمد على هوية بصرية مستوحاة من طراز 'The Modern Majlis' الذي يمزج بين فخامة التراث العربي والذكاء الرقمي الحديث. يتميز بتصميم متجاوب تماماً باللون الأخضر الملكي والذهبي، مع رسوم متحركة سلسة وتجربة مستخدم تركز على وضوح المحتوى التعليمي.

**Goal / positioning**
- استخدام مكونات العميل (Client Components) حصراً للتفاعلات والرسوم المتحركة
- تصميم مستوحى من طراز الـ Modern Majlis الذي يجمع بين الأصالة والحداثة
- توزيع المحتوى بشكل يضمن تجربة مستخدم مريحة (UX)

**Key features**
- تصميم عصري ومتجاوب مع جميع أنواع الشاشات (Responsive Design)
- رسوم متحركة جذابة وسلسة باستخدام مكتبة Motion
- دعم كامل للغة العربية واتجاه النص من اليمين لليسار (RTL)
- قسم مفصل للمميزات والخدمات التعليمية المقدمة
- عرض لآراء الطلاب وتقييماتهم (Testimonials Section)
- جداول أسعار واضحة ومنظمة للباقات التعليمية

**Technical stack**  
Next.js 15.4.9 (App Router) · React 19.x · Tailwind CSS 4.1.11 · Motion (Framer Motion) 12.23.24 · Lucide React Icons · TypeScript · PostCSS & Autoprefixer

**Engineering strategies**
- تطبيق مبادئ الـ Accessibility لضمان وصول الجميع للمحتوى
- إدارة الحالة باستخدام الـ React Hooks الأساسية

**Performance**
- الاستفادة من Static Site Generation (SSG) لسرعة استثنائية
- تحسين الصور وتصغير حجمها تلقائياً
- تقليل استهلاك الـ JavaScript في الأماكن غير الضرورية
- استخدام Tailwind CSS 4 لتقليل حجم ملف الـ CSS النهائي

**Security & reliability**
- اتباع معايير الأمان في Next.js
- حماية البيانات في روابط التواصل الاجتماعي
- دعم بروتوكول HTTPS عند النشر

- **Live / demo:** https://mr-ali-elgabry-portfolio.vercel.app/
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/7

---

#### Fabrica Store Website

Fabrica Store is a modern, full-featured e-commerce platform built with cutting-edge web technologies. The project delivers a seamless shopping experience with an advanced admin dashboard, secure authentication system, and fully responsive user interface. The project demonstrates expertise in modern web development, performance optimization, and best practices.

**Goal / positioning**
- Server Components for faster data fetching, better SEO, and reduced client bundle size
- Client Components for interactive sections (Search, Cart, Authentication, Theme Toggle)
- Suspense Boundaries with Skeleton Loading for improved perceived performance

**Key features**
- Professional product display with multi-image gallery
- Interactive product cards with hover effects
- Multiple images support per product
- Automatic image optimization via Next.js Image
- Skeleton Loading for improved loading experience
- Real-time product search from header

**Technical stack**  
Next.js 15.5.6 (App Router, Server/Client Components, Suspense, Streaming) · React 19.0.0 (Latest React with Hooks and Context API) · Turbopack (Fast build engine for development) · Firebase 12.0.0 (Authentication, Cloud Firestore, Real-time Database) · Cloudinary 2.7.0 (Image Upload, Optimization, CDN Delivery) · Tailwind CSS 4.1.13 (Utility-First CSS with Dark Mode support) · Material-UI (MUI) 7.3.2 (Component library with Theme Provider) · @emotion/react & @emotion/styled (CSS-in-JS for dynamic styling) · @heroicons/react (SVG icon library) · TanStack React Query 5.85.0 (Server state management, caching, background refetching)

**Engineering strategies**
- Incremental Static Regeneration (ISR) with revalidate for automatic content updates
- Query Parameters for managing search and filtering without Context API overhead
- Automatic Prefetching for pages via next/link for instant navigation
- Data Caching with TanStack React Query (3-5 minute stale time) and localStorage

**Performance**
- Server-Side Rendering (SSR) for initial page load
- Static Site Generation (SSG) where applicable
- Incremental Static Regeneration (ISR) for dynamic content
- Automatic Code Splitting by Next.js

**Security & reliability**
- Firebase Security Rules for database protection
- Environment Variables for API key protection
- Protected Routes with authentication checks
- Role-Based Access Control (Admin/Customer)

- **Live / demo:** https://fabrica-store-website.vercel.app/
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/8

---

#### FoodEx Website

FoodEx is a modern, comprehensive restaurant management and dish display website built with React and Firebase. The project delivers a seamless dining experience with an advanced admin dashboard, secure authentication system, real-time dish management, and fully responsive user interface. The project demonstrates expertise in React development, Firebase integration, state management, and best practices for restaurant web applications.

**Goal / positioning**
- Client Components for all interactive sections (Search, Favorites, Authentication)
- Context API for global state management (Dishes, User, Search)
- LocalStorage for temporary data caching and offline support

**Key features**
- Professional dish display with card-based layout
- Interactive dish cards with hover effects and favorite functionality
- Multiple meal types support (Breakfast, Lunch, Dinner)
- Real-time dish search from header with instant results
- Category-based filtering by meal type
- Rating system with star display

**Technical stack**  
React 18.3.1 (Hooks, Context API, Functional Components) · React Router DOM 7.0.1 (Client-side routing and navigation) · Firebase 11.7.3 (Authentication, Cloud Firestore, Storage) · Material-UI (MUI) 6.1.9 (Component library with theming) · @emotion/react 11.13.5 (CSS-in-JS styling) · @emotion/styled 11.13.5 (Styled components) · @mui/icons-material 6.1.9 (Icon library) · SweetAlert2 11.21.0 (Beautiful alert dialogs) · React Scripts 5.0.1 (Build and development tools) · Web Vitals 2.1.4 (Performance monitoring)

**Engineering strategies**
- Firebase Firestore for real-time database operations
- React Router for client-side routing and navigation
- Dynamic routing for dish details pages
- State Management via React Context API (Dishes, User, Search, Favorites)

**Performance**
- Client-Side Rendering (CSR) for fast initial load
- Component-based code splitting
- LocalStorage caching for dishes data
- Context API for efficient state sharing

**Security & reliability**
- Firebase Security Rules for database protection
- Environment Variables for API key protection
- Protected Routes with authentication checks
- Role-Based Access Control (Admin/User)

- **Live / demo:** https://food-ex-website-by-react-d5uc.vercel.app/
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/9

---

#### First Portfolio (Personal Developer Portfolio)

A modern, responsive developer portfolio built with Next.js 16 featuring animated sections, a projects gallery, SEO optimization, and clean reusable UI components. The site showcases personal projects with dedicated detail pages, an integrated contact form via Web3Forms, and smooth Framer Motion & Lottie animations throughout.

**Goal / positioning**
- App Router architecture for clean routing and server components
- Dynamic project detail pages via [id] route segments
- JSON-driven data layer for projects and skills

**Key features**
- Hero Section with typewriter introduction and CTA buttons
- About Section with animated bio and Lottie circle animation
- Skills Section with auto-scrolling skills list, detail view, and circular progress indicators
- Projects Gallery — JSON-driven grid with dedicated detail pages per project
- Contact Section with integrated contact form via Web3Forms
- Full SEO Optimization — metadata, OpenGraph, Twitter Cards, JSON-LD structured data, canonical URLs

**Technical stack**  
Next.js 16 (App Router, Turbopack) · React 19 (Latest React with Hooks and Context API) · Tailwind CSS 4 (Utility-first CSS with responsive design) · Framer Motion (Advanced motion design and animations) · Lucide React (Modern SVG icon library) · Simple Icons (SVG technology icons) · Lottie React (Interactive Lottie animations) · Web3Forms (Contact form integration) · Google Fonts — Inter, Poppins (Custom typography) · Vercel (Deployment platform)

**Engineering strategies**
- Framer Motion for declarative page and component transitions
- Lottie animations for interactive visual elements
- Web3Forms integration for serverless contact form
- SEO-first approach with comprehensive metadata and structured data

**Performance**
- Dynamic imports and code splitting for reduced bundle size
- Lazy loading of non-critical components
- Next.js Image optimization with next/image
- Turbopack for fast development builds

- **Live / demo:** https://mostafa-abdelraheem-portfolio.vercel.app/
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/10

---

### Learning Foundations

#### Diverse Projects (مشاريع متنوعة)

A collection of several smaller projects completed during training, showcasing a variety of skills including Vanilla JavaScript, React, Material UI, and CSS animations. These projects demonstrate a solid foundation in front-end development through interactive games and utility applications.

**Goal / positioning**
- Consconsolidating small projects to keep the portfolio clean
- Synthesizing various technologies in one highlight entry
- Showcasing fundamental skills alongside complex ones

**Key features**
- Typing Speed Test Game with difficulty levels and timer.
- React-based To-Do List with Material UI and local persistence.
- Responsive Website Templates with custom CSS and theme switching.
- Interactive Quiz App with dynamic question loading from JSON.
- Word Guessing Game with color-coded feedback and image hints.

**Technical stack**  
Vanilla JS · React · Material UI · CSS Animations · Framer Motion · HTML5

**Performance**
- Optimized image collage for fast loading
- Clean and lightweight description synthesis

- **Live / demo:** https://mostafa-abdelraheem-portfolio.vercel.app/
- **Case details:** https://mostafa-abdelrahem-portfolio.vercel.app/projects/11

---

## AI-Assisted Engineering

I use AI-assisted development as part of my engineering workflow for planning, repetitive implementation, debugging, code review, and automation, while keeping architecture, product decisions, validation, and final engineering quality under direct control.

---

## Private Source Code Policy

Most production, commercial, and client repositories remain private to protect source code and client IP.

Selected documentation and live previews are publicly available through this profile and my portfolio. Private production code can be made available for technical review when appropriate.

---

## Links

- **Portfolio:** https://mostafa-abdelrahem-portfolio.vercel.app
- **Blog / content automation demo:** https://mostafa-abdelrahem-portfolio.vercel.app/blog
- **GitHub:** https://github.com/MostafaAbelraheem2020
- **LinkedIn:** https://www.linkedin.com/in/mostafa-mohamed-63b87627a/

---

*For recruiters and technical reviewers: start with Voyajar, Assistants Pro AI / Dawrak, PharmaFlow, and Mohamed Abdelwahab Constructions — then open the live demos above for product-level validation.*

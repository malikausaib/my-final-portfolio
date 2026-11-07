# Malik Mohmmad Ausaib — Personal Portfolio

> **B.Tech Computer Science & Engineering Undergraduate (3rd Semester)**  
> **SRM Institute of Science and Technology (SRMIST), Kattankulathur (KTR) Campus**

A high-end, editorial personal portfolio website designed and engineered with intentional negative space, architectural typography, monochromatic aesthetics, and a custom articulated cartoon character physics system.

---

## 🌟 Key Features

1. **Editorial Display Typography & Composition**:
   - Expressive typography using *Syne*, *Instrument Serif*, *Plus Jakarta Sans*, and *JetBrains Mono*.
   - Strict linguistic integrity: The name **Malik Mohmmad Ausaib** preserves individual words with zero breaking of the word *Mohmmad*.
   - Architectural layout inspired by high-end design studios and minimalist editorial publications.

2. **The Signature Falling & Hanging Person (Left Gutter)**:
   - Handcrafted, strictly black-and-white minimalist SVG character with independently articulated limbs.
   - Three dynamic states:
     - **Falling**: Smoothly glides down the left negative space when scrolling, with arms and legs reacting to velocity.
     - **Grabbing & Hanging**: Latches onto a peg on the guide rail after ~350ms scroll pause, dangling with a subtle natural pendulum swing.
     - **Releasing**: Releases grip and resumes falling when scrolling continues.
   - Playful interactive quotes on click; fully accessible and respects `prefers-reduced-motion`.

3. **Academic Journey (Semester-Wise Coursework)**:
   - **Semester 01**: Chemistry, Computational Biology, Calculus, C Programming, Python Programming.
   - **Semester 02**: Advanced Calculus, Semiconductor Physics, Object-Oriented Programming using C++ (OOPS), Engineering Graphics and Design (EGD — AutoCAD).
   - **Semester 03 (Current)**: Computer Organization and Architecture (COA), Operating Systems (OS), Data Structures and Algorithms (DSA), Java Programming, Transforms and Boundary Value Problems (TBVP).
   - Interactive semester index with expandable focus areas and syllabus units.

4. **Things I Work With (Core Languages)**:
   - Focused exclusively on **C**, **Python**, **Java**, and **C++**.
   - Zero subjective skill bars or percentage ratings; showcases real paradigms, standards, and code examples.

5. **Full Backend Contact Architecture**:
   - Integrated with **Supabase Database** + **Supabase Edge Functions** + **Resend API**.
   - Table: `contact_messages` with strict Row Level Security (RLS) preventing public access to submitted messages.
   - Notification email automatically routed to `malikausaib07@gmail.com` with `reply_to` configured to the sender's email.
   - Automated confirmation receipt sent to the visitor.
   - Honeypot anti-spam field, client and server-side rate-limiting, and input sanitization.
   - Graceful sandbox demo mode when credentials are not yet added.

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v18+)
- npm or pnpm

### Development
```bash
# Install dependencies
npm install

# Start local development server
npm run dev
```

### Production Build
```bash
# Compile TypeScript and bundle with Vite
npm run build

# Preview production build locally
npm run preview
```

---

## 🛠️ Supabase & Resend Backend Setup

Refer to [`supabase/README.md`](./supabase/README.md) for detailed deployment steps:
1. Execute `supabase/schema.sql` in your Supabase SQL editor.
2. Deploy the Edge Function:
   ```bash
   supabase functions deploy contact --no-verify-jwt
   supabase secrets set RESEND_API_KEY=re_... RESEND_FROM_EMAIL=...
   ```
3. Set your `VITE_SUPABASE_URL` and `VITE_SUPABASE_ANON_KEY` in `.env`.

---

## 📬 Contact & Profiles

- **Personal Email**: [malikausaib07@gmail.com](mailto:malikausaib07@gmail.com)
- **Student Email**: [ma1533@srmist.edu.in](mailto:ma1533@srmist.edu.in)
- **LinkedIn**: [linkedin.com/in/malik-mohammad-ausaib-23ab72248](https://www.linkedin.com/in/malik-mohammad-ausaib-23ab72248/)
- **GitHub**: [github.com/malikausaib](https://github.com/malikausaib)
- **Instagram**: [instagram.com/ausaib.malik](https://www.instagram.com/ausaib.malik/)


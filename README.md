<div align="center">
  <img src="assets/varun-profile-banner.svg" alt="Varun Gupta — Full-Stack Developer" width="100%" />
  <h2>Full-Stack Developer · Mumbai, India</h2>
  <p>Building useful digital products — from polished interfaces to secure, dependable application workflows.</p>
  <p>
    <a href="https://blue-crab-314523.hostingersite.com"><img src="https://img.shields.io/badge/PORTFOLIO-Visit%20website-172b4d?style=for-the-badge" alt="Portfolio"/></a>
    <a href="https://strydegosox.com"><img src="https://img.shields.io/badge/FEATURED%20PROJECT-Live%20store-126b67?style=for-the-badge" alt="Live client project"/></a>
    <a href="https://github.com/varung4067-hash?tab=repositories"><img src="https://img.shields.io/badge/GITHUB-Explore%20code-24292f?style=for-the-badge&logo=github" alt="GitHub repositories"/></a>
  </p>
</div>

<p align="center">
  <a href="#about-me">About</a> &nbsp;·&nbsp;
  <a href="#featured-projects">Projects</a> &nbsp;·&nbsp;
  <a href="#technical-toolkit">Technical toolkit</a> &nbsp;·&nbsp;
  <a href="#education--professional-background">Education & background</a> &nbsp;·&nbsp;
  <a href="#learning--certifications">Learning</a>
</p>

---

## About me

I’m **Varun Gupta**, a full-stack developer and BSc IT graduate based in Mumbai, India. I enjoy taking a business problem or an unfinished user journey and turning it into a working digital product — one that feels intuitive on the front end and behaves predictably behind the scenes.

My work spans responsive interfaces, frontend state and interactions, REST APIs, database models, authentication, payment integrations and the operational tools that teams use after launch. I’m especially interested in the engineering details that become important when a product is used by real people: how an application handles duplicate requests, delayed payment callbacks, changing stock, invalid input, failed API calls and privileged admin actions.

I’m most interested in **full-stack and frontend engineering**, with a growing focus on backend reliability and security-minded application design. I like understanding how the complete system fits together rather than treating the UI, API and database as separate pieces.

### What you can expect from my work

- **End-to-end product thinking:** I look at the complete customer and operator journey, not only the screen being requested.
- **Practical engineering:** I connect frontend components, APIs, persistence and third-party services into a coherent workflow.
- **Care for edge cases:** I pay attention to validation, retries, payment states, inventory changes, authentication and failure handling.
- **Interface detail:** I enjoy responsive layouts, clean visual hierarchy, motion and interactive experiences when they improve usability.
- **Ownership and learning:** I use AI-assisted tools where they help me move faster, but I focus on understanding the implementation, integrating it correctly, debugging it and validating the result.

## Featured projects

These projects show the range of work I enjoy: a live client commerce platform, a security-monitoring lab, interactive business websites and a hardware-commerce application.

---

### 01 · StrydeGoSox — Live client e-commerce platform

<p><strong>Full-stack development · Payments · Inventory · Admin operations</strong></p>
<a href="https://strydegosox.com"><img src="https://raw.githubusercontent.com/varung4067-hash/strydegosox-ecommerce/main/docs/screenshots/01-home-hero.jpg" alt="StrydeGoSox live storefront" width="100%"/></a>

StrydeGoSox is a customer-facing online store built for a consumer product brand. The application brings together product discovery, product options, cart and checkout, online payments, Cash on Delivery, order fulfilment and the admin workflows required to run the store.

**My contribution**
- Built and integrated the responsive storefront, product selection, cart and checkout experience.
- Developed Node.js and Express API workflows backed by MongoDB and Mongoose.
- Implemented server-side cart repricing so the backend calculates order totals from trusted product records.
- Integrated Razorpay order creation, checkout-signature verification and signed webhook processing.
- Added checkout idempotency and webhook event tracking to reduce duplicate order and payment side effects.
- Worked on inventory reservation, commit, release and restoration across payment, fulfilment and refund states.
- Built admin workflows for catalogue and stock management, orders, fulfilment, COD collection/remittance and refunds.
- Integrated transactional order and status emails through Resend.

**Architecture — see how the complete product works**

<a href="https://github.com/varung4067-hash/strydegosox-ecommerce/blob/main/docs/ARCHITECTURE.md"><img src="https://raw.githubusercontent.com/varung4067-hash/strydegosox-ecommerce/main/docs/architecture-diagram.svg" alt="StrydeGoSox architecture: storefront and admin, Express API, MongoDB, Razorpay and Resend" width="100%"/></a>

<p align="center">
  <a href="https://strydegosox.com"><img src="https://img.shields.io/badge/1-Live%20store-126b67?style=flat-square" alt="Live store"/></a>
  <a href="https://github.com/varung4067-hash/strydegosox-ecommerce"><img src="https://img.shields.io/badge/2-Source%20code-24292f?style=flat-square&logo=github" alt="Source code"/></a>
  <a href="https://github.com/varung4067-hash/strydegosox-ecommerce/tree/main/src"><img src="https://img.shields.io/badge/3-Backend%20modules-263f5b?style=flat-square" alt="Backend modules"/></a>
  <a href="https://github.com/varung4067-hash/strydegosox-ecommerce/blob/main/docs/ARCHITECTURE.md"><img src="https://img.shields.io/badge/4-Architecture%20notes-51458c?style=flat-square" alt="Architecture notes"/></a>
</p>

**Engineering areas worth exploring in the code**

| Area | Where to look |
|:--|:--|
| API entry point and middleware | [`src/server.js`](https://github.com/varung4067-hash/strydegosox-ecommerce/blob/main/src/server.js) · [`src/middleware`](https://github.com/varung4067-hash/strydegosox-ecommerce/tree/main/src/middleware) |
| Checkout and pricing | [`src/routes/checkout.js`](https://github.com/varung4067-hash/strydegosox-ecommerce/blob/main/src/routes/checkout.js) · [`src/utils/orders.js`](https://github.com/varung4067-hash/strydegosox-ecommerce/blob/main/src/utils/orders.js) |
| Payment verification and webhooks | [`src/routes/payments.js`](https://github.com/varung4067-hash/strydegosox-ecommerce/blob/main/src/routes/payments.js) |
| Admin and order operations | [`src/routes/admin.js`](https://github.com/varung4067-hash/strydegosox-ecommerce/blob/main/src/routes/admin.js) · [`admin/`](https://github.com/varung4067-hash/strydegosox-ecommerce/tree/main/admin) |
| Data models | [`src/models`](https://github.com/varung4067-hash/strydegosox-ecommerce/tree/main/src/models) |

**Client-reported activity:** 70 orders in the first week and 500+ orders in the first month after launch. These are order counts shared by the client, not independently audited revenue or conversion figures.

**Technology:** `HTML` `CSS` `JavaScript` `Node.js` `Express` `MongoDB` `Mongoose` `Razorpay` `Resend` `JWT` `bcryptjs` `Helmet`

---

### 02 · Sysmon SIEM Homelab — Security monitoring and detection engineering

**Python · Windows event telemetry · PowerShell detection · Flask dashboard**

A hands-on Windows endpoint-monitoring lab exploring how process-creation telemetry can be turned into structured security alerts. It reads Sysmon Event ID 1 from the Windows Operational event channel, inspects PowerShell command lines for suspicious indicators and presents the resulting alert context in a Flask investigation dashboard.

<a href="https://github.com/varung4067-hash/soc-homelab-siem-project"><img src="https://raw.githubusercontent.com/varung4067-hash/soc-homelab-siem-project/main/docs/architecture.svg" alt="Sysmon SIEM detection pipeline from Windows event telemetry to Flask dashboard" width="100%"/></a>

**What I explored and implemented**
- Event collection and parsing from `Microsoft-Windows-Sysmon/Operational`.
- Rule-based checks for encoded PowerShell, `FromBase64String`, `Invoke-Expression` / `IEX` and `DownloadString`.
- Alert enrichment with severity, confidence, detection rationale and MITRE ATT&CK technique `T1059.001`.
- Command-line deduplication and basic correlation of alerts sharing a host and user within a ten-minute window.
- A Flask dashboard for reviewing alert details, severity summaries and visualisations.

**Be transparent about the scope:** this is a learning and experimentation project, not a production SIEM. The repository documents follow-up work around packaging, dependency setup and separating demo data from live telemetry. The detection rules are keyword-based triage signals and require contextual investigation; they are not definitive proof of compromise.

**Technology:** `Python` `Sysmon` `Windows Event Logs` `pywin32` `XML` `Flask` `Chart.js` `MITRE ATT&CK`

[Explore source code and dashboard](https://github.com/varung4067-hash/soc-homelab-siem-project) · [Read project documentation](https://github.com/varung4067-hash/soc-homelab-siem-project#readme)

---

### 03 · Sai Shradha Construction — Corporate website and interactive 3D experience

**React website · Service presentation · Project portfolio · Scroll-linked 3D interaction**

A multi-section website concept for a construction business, designed to make the company’s capabilities and project work easier to understand and explore. The experience is organised around six key sections: Home, About, Services, Projects, Safety and Contact.

**What I worked on**
- Structured the content and navigation to help visitors move from company introduction to services and project examples.
- Built reusable React components and responsive layouts for desktop and mobile.
- Added project showcases, service information, safety content and clear enquiry paths.
- Created a scroll-linked 3D construction sequence using GSAP / ScrollTrigger and Three.js with React Three Fiber.
- Considered reduced-motion behaviour and responsive fallbacks for the interactive experience.

**Technology:** `React 18` `Vite` `Tailwind CSS` `React Router` `Framer Motion` `GSAP` `Three.js` `React Three Fiber`

[View the construction website walkthrough in my portfolio](https://blue-crab-314523.hostingersite.com/#work)

<sub>The linked page is a portfolio preview rather than a separately hosted construction-company domain.</sub>

---

### 04 · Varun & Co. — Digital studio website

**Studio positioning · Services · Selected work · Enquiry journey**

Varun & Co. is my digital studio website, built to communicate the studio’s services, show work and guide prospective clients towards starting a project. Its positioning is simple: helping businesses turn into brands through useful digital experiences.

**What the website includes**
- Clear service categories: Website Development, Business Software, Branding & Digital Presence, and Hosting & Support.
- A five-stage delivery story: Discovery → Strategy → Design → Development → Launch.
- Service information, selected work, FAQs and project-enquiry calls to action.
- Responsive navigation and motion-led interactions, while keeping the content easy to scan.

**Technology:** `React` `TypeScript` `Tailwind CSS` `Motion for React` `Lucide React` `Custom CSS`

[Visit the Varun & Co. website](https://blue-crab-314523.hostingersite.com) · [Explore selected work](https://blue-crab-314523.hostingersite.com/#work)

---

### 05 · Hardware E-commerce Platform — Product catalogue and store administration

**Full-stack commerce application · Product management · Cart and checkout**

A hardware-store application concept for browsing computer components and managing a product catalogue. The customer experience covers product discovery, cart, checkout and order history; the admin side is designed to let the store owner manage products, prices and stock without editing source files.

**Core functionality**
- Product catalogue for components such as graphics cards, processors, RAM, cases and motherboards.
- Product browsing, add-to-cart, quantity management and checkout flow.
- Order history and backend order persistence.
- Admin dashboard to add, edit and remove products and maintain pricing and inventory.
- MongoDB Atlas for data persistence, Razorpay for payment integration and Resend for transactional email.

**Technology:** `HTML` `CSS` `JavaScript` `Node.js` `Express` `MongoDB Atlas` `Razorpay` `Resend`

[View the hardware-store project preview in my portfolio](https://blue-crab-314523.hostingersite.com/#work)

<sub>This project is currently showcased through the portfolio preview; I have not linked a separate public source repository for it.</sub>

## Technical toolkit

| Area | Technologies and tools |
|:--|:--|
| **Frontend** | React, JavaScript, TypeScript, HTML5, CSS3, Tailwind CSS, responsive UI development |
| **Backend** | Node.js, Express.js, REST APIs, Python, Flask |
| **Databases** | MongoDB, MongoDB Atlas, Mongoose |
| **Payments and integrations** | Razorpay, Resend, payment callbacks and webhooks |
| **Application security** | JWT, bcrypt / bcryptjs, HTTP-only cookies, Helmet, CSP, CORS, rate limiting, server-side validation |
| **Security operations** | Sysmon, Windows Event Logs, PowerShell, MITRE ATT&CK, detection rules, alert triage |
| **Motion and 3D** | Framer Motion, GSAP, ScrollTrigger, Three.js, React Three Fiber |
| **Development workflow** | Git, GitHub, debugging, source-level checks, project documentation and deployment workflows |

## Education & professional background

**Bachelor of Science in Information Technology (BSc IT)**  
Guru Nanak Khalsa College · University of Mumbai · Completed 2025

**Customer Support Executive — Teleperformance**  
Worked on an international Airbnb support process for six months, handling 1,000+ customer interactions. That experience strengthened my ability to understand user problems, communicate clearly, troubleshoot under pressure and follow an issue through to resolution — skills I bring into product development.

## Learning & certifications

- **Google Cybersecurity Professional Certificate** — completed.
- **TryHackMe SOC Level 1 learning path** — completed.
- **CompTIA Security+** — currently preparing.

These security studies complement my full-stack work and help me think more carefully about authentication, secure application behaviour, event visibility and operational risk.

## How I approach a project

1. **Understand:** clarify the user, business goal and problem to solve.
2. **Map:** work out the user journey, data flow, application boundaries and integrations.
3. **Build:** connect the interface, backend, persistence and external services.
4. **Validate:** check the main flow, error states, repeated requests and edge cases.
5. **Improve:** document the decisions, fix rough edges and keep strengthening the implementation.

## What I’m looking for

I’m interested in **Junior Full-Stack Developer, Frontend Developer and Node.js Developer** opportunities where I can work on real products, contribute across the stack, learn from experienced engineers and grow my ability to design and deliver maintainable software.

<div align="center">
  <h3>Interested in working together?</h3>
  <p>Explore the live work, inspect the implementation and follow the architecture links above.</p>
  <a href="https://blue-crab-314523.hostingersite.com"><img src="https://img.shields.io/badge/Visit-Portfolio-172b4d?style=for-the-badge" alt="Visit portfolio"/></a>
  <a href="https://github.com/varung4067-hash?tab=repositories"><img src="https://img.shields.io/badge/Browse-GitHub-24292f?style=for-the-badge&logo=github" alt="Browse repositories"/></a>
</div>

---

<div align="center"><sub>Thoughtful interfaces. Reliable workflows. Continuous improvement.</sub></div>
<div align="center">
  <img src="assets/varun-profile-banner.svg" alt="Varun Gupta — Full-Stack Developer" width="100%" />
  <h1>Varun Gupta</h1>
  <h3>Junior Full-Stack Developer · React · Node.js · MongoDB</h3>
  <p>Mumbai, India · Open to junior full-stack, React and Node.js opportunities</p>
  <p>Building useful web products with thoughtful interfaces, dependable APIs and clear data flows.</p>
  <p>
    <a href="https://blue-crab-314523.hostingersite.com"><img src="https://img.shields.io/badge/PORTFOLIO-Explore%20my%20work-172b4d?style=for-the-badge" alt="Portfolio"/></a>
    <a href="https://strydegosox.com"><img src="https://img.shields.io/badge/LIVE%20CLIENT%20PROJECT-StrydeGoSox-126b67?style=for-the-badge" alt="StrydeGoSox live store"/></a>
    <a href="https://github.com/varung4067-hash?tab=repositories"><img src="https://img.shields.io/badge/GITHUB-Explore%20repositories-24292f?style=for-the-badge&logo=github" alt="Repositories"/></a>
  </p>
</div>

---

## About

I'm a Mumbai-based full-stack developer and BSc IT graduate who enjoys turning business requirements into working web applications. I work across responsive frontend experiences, REST APIs, database-backed workflows, authentication, payment integrations and admin tools.

My strongest practical example is **StrydeGoSox**, a live client e-commerce platform. I worked across the storefront, Node.js/Express backend, MongoDB data layer, Razorpay payment flow and store-administration workflows. I also build security-focused projects to understand endpoint telemetry, detection logic and investigation workflows.

I care about the parts of software that matter after the first demo: trusted server-side calculations, input validation, authentication boundaries, retries, consistent order state, useful error handling and interfaces that remain usable across screen sizes. I use AI-assisted tools as part of my workflow, while focusing on understanding the code, integrating components, debugging issues and validating the behaviour.

**Currently looking for:** Junior Full-Stack Developer, React Developer or Node.js Developer roles where I can contribute to real products, learn from experienced engineers and grow through code reviews and collaboration.

### How I think about full-stack architecture

A useful product is more than a collection of screens. The interface, application rules, persistent data and external services need clear boundaries. The diagram below uses the StrydeGoSox implementation as a concrete example of how those layers connect.

<p align="center">
  <a href="https://github.com/varung4067-hash/strydegosox-ecommerce/blob/main/docs/ARCHITECTURE.md">
    <img src="https://raw.githubusercontent.com/varung4067-hash/strydegosox-ecommerce/main/docs/architecture-diagram.svg" alt="StrydeGoSox application architecture: customer storefront and admin console, Express API and middleware, MongoDB persistence, Razorpay payments and Resend email" width="100%" />
  </a>
</p>
<p align="center"><sub>Project-specific architecture diagram · Select the diagram to read the detailed architecture and workflow notes.</sub></p>

| Layer | Responsibility | Technologies / components |
|:--|:--|:--|
| Experience | Customer storefront and authenticated admin console | HTML, CSS, JavaScript |
| Application | Routing, business rules, auth, checkout, payments and operations | Node.js, Express.js, middleware |
| Persistence | Users, products, orders, settings and webhook-event records | MongoDB, Mongoose |
| Integrations | Payment processing and transactional email | Razorpay, Resend |
| Transaction controls | Server-side repricing, signature checks, idempotency and inventory state transitions | Backend validation and workflow logic |

**Engineering decisions I pay attention to:** the browser is treated as an input surface rather than the source of truth for price or payment status; payment callbacks are verified on the server; webhook events and checkout retries are handled with duplicate processing in mind; and inventory moves through explicit reservation, commit and release steps.

---

## Featured projects

### 01 · StrydeGoSox — Live client e-commerce platform

<p><strong>Full-stack development · Checkout and payments · Inventory · Admin operations</strong></p>

<img src="assets/strydegosox-project-visual.webp" alt="Concept artwork showing an e-commerce storefront on a laptop and mobile phone with sock products; presentation artwork, not a screenshot of the live application" width="100%" />

<p align="center"><sub>Project concept artwork created for this portfolio. It is not a captured screen from the live site; actual application screenshots are shown below.</sub></p>

**The product:** a live online store for a consumer product brand, connecting product discovery, product options, cart, checkout, online payments, Cash on Delivery, order fulfilment and the tools used to operate the store.

**My contribution**
- Built and integrated responsive storefront, product-selection, cart and checkout experiences.
- Developed backend API workflows with Node.js, Express.js, MongoDB and Mongoose.
- Implemented server-side cart repricing so order totals are calculated from trusted catalogue records.
- Integrated Razorpay order creation, payment-signature verification and signed webhook processing.
- Added checkout idempotency and webhook-event tracking to reduce duplicate order and payment side effects.
- Worked on inventory reservation, commit, release and restoration across order and payment states.
- Built admin workflows for catalogue, stock, orders, fulfilment, COD collection/remittance and refunds.
- Integrated transactional order and status emails through Resend.

**Real application screenshots**

<p align="center">
  <img src="https://raw.githubusercontent.com/varung4067-hash/strydegosox-ecommerce/main/docs/screenshots/01-home-hero.jpg" alt="Actual StrydeGoSox storefront screenshot" width="100%" />
</p>
<p align="center">
  <a href="https://raw.githubusercontent.com/varung4067-hash/strydegosox-ecommerce/main/docs/screenshots/02-product-specifications.jpg">Product details screenshot</a>
  &nbsp;·&nbsp;
  <a href="https://raw.githubusercontent.com/varung4067-hash/strydegosox-ecommerce/main/docs/screenshots/03-bundle-options.jpg">Bundle selection screenshot</a>
</p>

**Explore the implementation:** [Live store](https://strydegosox.com) · [Source code](https://github.com/varung4067-hash/strydegosox-ecommerce) · [Architecture and checkout flow](https://github.com/varung4067-hash/strydegosox-ecommerce/blob/main/docs/ARCHITECTURE.md) · [Security notes](https://github.com/varung4067-hash/strydegosox-ecommerce/blob/main/SECURITY.md)

**Technology:** HTML · CSS · JavaScript · Node.js · Express.js · MongoDB · Mongoose · Razorpay · Resend · JWT

**Client-reported activity:** the client reported 70 orders in the first week and 500+ orders in the first month after launch. These are client-reported order counts, not independently audited revenue or conversion figures.

### 02 · Sysmon SIEM Homelab — Endpoint telemetry and detection engineering

<p><strong>Python · Windows Sysmon · PowerShell detections · Flask dashboard · MITRE ATT&CK</strong></p>

A hands-on Windows endpoint-monitoring lab that explores how process-creation telemetry can be turned into structured alerts for analyst review.

<p align="center">
  <img src="https://raw.githubusercontent.com/varung4067-hash/soc-homelab-siem-project/main/DASHBOARD.png" alt="Actual dashboard screenshot from the Sysmon SIEM homelab project" width="100%" />
</p>
<p align="center"><sub>Detection pipeline: Sysmon Event ID 1 → Python event parsing → PowerShell indicators → alert enrichment → Flask investigation view.</sub></p>

**What I implemented and explored**
- Read process-creation events from the Microsoft-Windows-Sysmon/Operational channel.
- Added keyword-based triage rules for encoded PowerShell, FromBase64String, Invoke-Expression/IEX and DownloadString.
- Enriched alerts with severity, confidence, detection rationale and MITRE ATT&CK technique T1059.001.
- Added command-line deduplication and basic grouping of alerts that share a host and user within a ten-minute window.
- Built a Flask dashboard for reviewing alert details, severity summaries and visualisations.

**Be clear about the scope:** this is a learning and experimentation project, not a production SIEM. The current rules are heuristic triage signals, not proof of compromise. The repository documents remaining work around packaging, dependency setup, test fixtures and separating demo data from live telemetry.

[Source code and documentation](https://github.com/varung4067-hash/soc-homelab-siem-project) · [Detection architecture](https://github.com/varung4067-hash/soc-homelab-siem-project/blob/main/docs/architecture.svg)

**Technology:** Python · Sysmon · Windows Event Logs · pywin32 · XML · Flask · Chart.js · MITRE ATT&CK

### 03 · Additional web and product work

**Sai Shradha Construction — interactive business website**  
A React website experience organised around company information, services, project showcases, safety content and enquiries. The portfolio walkthrough includes a scroll-linked 3D construction sequence.  
[View portfolio work](https://blue-crab-314523.hostingersite.com/#work)

**Varun & Co. — digital studio website**  
A studio website presenting website development, business software, branding and digital-presence services, with a structured discovery-to-launch journey.  
[Visit the website](https://blue-crab-314523.hostingersite.com)

**Hardware e-commerce application — product catalogue and store administration**  
A portfolio project covering computer-component discovery, cart and checkout, order history, and an admin dashboard for product and inventory management. It is presented through the portfolio; a separate public source repository is not currently linked.  
[View portfolio work](https://blue-crab-314523.hostingersite.com/#work)

---

## Technical toolkit

| Area | Tools and technologies |
|:--|:--|
| Frontend | JavaScript, React, HTML5, CSS3, responsive UI development |
| Backend | Node.js, Express.js, REST APIs, Python, Flask |
| Databases | MongoDB, MongoDB Atlas, Mongoose |
| Payments and integrations | Razorpay, Resend, payment callbacks and webhooks |
| Application security | JWT, bcryptjs, HTTP-only cookies, Helmet, CSP, CORS, rate limiting, server-side validation |
| Security operations | Sysmon, Windows Event Logs, PowerShell, MITRE ATT&CK, alert triage |
| Development workflow | Git, GitHub, debugging, documentation and deployment workflows |
| Motion and 3D | Framer Motion, GSAP, ScrollTrigger, Three.js, React Three Fiber |

## Education and professional background

**Bachelor of Science in Information Technology (BSc IT)**  
Guru Nanak Khalsa College · University of Mumbai · 2025

**Customer Support Executive — Teleperformance**  
Worked on an international Airbnb support process for six months, handling 1,000+ customer interactions. This experience strengthened my communication, troubleshooting, customer empathy and issue-resolution skills.

## Learning and certifications

- Google Cybersecurity Professional Certificate — completed.
- TryHackMe SOC Level 1 learning path — completed.
- CompTIA Security+ — currently preparing.

## What I bring to a team

- A practical end-to-end view of user journeys, APIs, data and third-party integrations.
- Experience building and launching a client-facing web application.
- Curiosity about secure application design and system behaviour.
- Clear communication, ownership of debugging and willingness to learn through feedback.

<div align="center">
  <h3>Let's build something useful.</h3>
  <p>
    <a href="https://blue-crab-314523.hostingersite.com">Portfolio</a>
    &nbsp;·&nbsp;
    <a href="https://github.com/varung4067-hash?tab=repositories">GitHub repositories</a>
    &nbsp;·&nbsp;
    <a href="https://strydegosox.com">Live client project</a>
  </p>
  <sub>Thoughtful interfaces · Reliable workflows · Continuous improvement</sub>
</div>

# Salone HealthConnect
### A Digital Healthcare Directory & Advisory Solution for Sierra Leone

> **Connecting every citizen to the care they need — from Freetown to Kono.**

---

## Table of Contents

- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Solution](#solution)
- [Key Features](#key-features)
- [Technical Architecture](#technical-architecture)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Impact & Vision](#impact--vision)
- [Contributing](#contributing)
- [License](#license)

---

## Project Overview

**Salone HealthConnect** is a fully functional, mobile-responsive web platform purpose-built to address critical healthcare accessibility challenges in Sierra Leone. It serves as a centralized digital hub where patients, caregivers, and community health workers can:

- Find verified medical facilities across all districts
- Book doctor appointments online
- Coordinate blood and medical supply donations
- Access emergency health information instantly

The platform is optimized for low-data environments, ensuring it remains accessible to the majority of Sierra Leoneans connecting on 2G or 3G mobile networks.

---

## Problem Statement

Sierra Leone has made significant progress expanding its healthcare infrastructure — yet millions of citizens still struggle to access basic health information when they need it most. The core challenges include:

| Challenge | Description |
|---|---|
| **Fragmented Information** | Hospital contacts, opening hours, and available services are scattered across paper directories, word of mouth, and outdated resources, with no single reliable digital source. |
| **Emergency Delays** | In life-threatening situations, locating the nearest open facility or reaching a blood donor can take hours — directly costing lives. |
| **Rural-Urban Divide** | Patients in districts such as Bo, Kenema, Kono, Makeni, and Tonkolili have little visibility into what specialist care is available and where. |
| **Blood Shortage Coordination** | Blood banks regularly run critically low with no public-facing system to alert donors or match urgent requests in real time. |
| **High Data Costs** | Most existing digital health tools are built for high-bandwidth environments, making them inaccessible to users on limited mobile data. |

---

## Solution

Salone HealthConnect bridges these gaps by providing a single, low-data-capable platform that brings together the four most critical healthcare needs:

### 🏥 Healthcare Facility Directory
A searchable, filterable directory of verified hospitals, clinics, and health centres across all Sierra Leone districts. Each listing includes contact details, operating hours, available services, and location via Google Maps integration.

### 📅 Doctor Appointment Booking
An intuitive appointment scheduling interface allowing users to browse available doctors by specialty and district, select time slots, and confirm bookings — without requiring a phone call.

### 🩸 Blood & Medical Donation Network
A tabbed donation platform covering:
- **Blood Donation** — Live stock levels by blood type at major facilities, with a blood type selector linking users directly to donor registration.
- **Medicine Contributions** — Connecting medication donors with facilities in greatest need.
- **Medical Equipment** — Facilitating the redistribution of equipment to under-resourced clinics.
- **Financial Support** — Directing monetary contributions to verified healthcare partners.

### 🚨 Emergency Information Access
Emergency contact numbers — including the **national emergency line (999)** and **ambulance line (117)** — are prominently displayed on every page via a persistent banner and a floating emergency button, ensuring critical contacts are never more than one tap away.

---

## Key Features

- **Nationwide Coverage** — Facilities and services across all Sierra Leone districts
- **Low-Data Optimized** — No heavy frameworks, no large media files, no unnecessary external dependencies
- **Mobile-First Design** — Fully responsive from 320px screen width upward
- **Real-Time Blood Stock Indicators** — Visual blood type availability levels at major facilities
- **Google Maps Integration** — Location-based facility discovery on the hospital search page
- **Single Stylesheet Architecture** — Consistent theming via CSS custom properties across all pages
- **Offline-Resilient** — Core content accessible even on poor connections
- **Always-Visible Emergency Access** — Persistent emergency contacts on every page

---

## Technical Architecture

### Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 (semantic, accessible) |
| Styling | CSS3 with custom properties (single `style.css`) |
| Interactivity | Vanilla JavaScript (ES6+) |
| Maps | Google Maps Embed API |
| Hosting | Static — deployable to any web host or CDN |

### Design Principles

- **Pure HTML/CSS core** for maximum compatibility and speed across all devices and browsers
- **Progressive enhancement** — fully usable without JavaScript; JS adds interactivity on top
- **No external dependencies** at runtime — no frameworks, no CDN-loaded libraries
- **Mobile-first CSS** with breakpoints scaling up to desktop
- **CSS custom properties** for unified theming and easy future rebranding

### JavaScript Functionality

- Search and filter for facility directory
- Time slot selection for appointment booking
- Tab switching in the donation portal
- Modal dialogs
- Mobile navigation menu

---

## Getting Started

### Prerequisites

No build tools or package manager required. The project runs as a standard static website.

### Running Locally

```bash
# Clone the repository
git clone https://github.com/your-org/salone-healthconnect.git
cd salone-healthconnect

# Open in browser (any method works)
open index.html

# Or serve with a simple local server (optional)
npx serve .
# or
python3 -m http.server 8000
```

Then visit `http://localhost:8000` in your browser.

### Deployment

The project is a fully static site and can be deployed to any static hosting provider:

- **Netlify** — drag and drop the project folder
- **Vercel** — connect your GitHub repository
- **GitHub Pages** — push to a `gh-pages` branch
- **Any web server** — upload files via FTP/SFTP

---

## Project Structure

```
salone-healthconnect/
├── index.html              # Homepage
├── hospitals.html          # Facility directory & map search
├── appointments.html       # Doctor appointment booking
├── donations.html          # Blood & medical donation portal
├── emergency.html          # Emergency contacts & resources
├── css/
│   └── style.css           # Single unified stylesheet (CSS custom properties)
├── js/
│   └── main.js             # Core JavaScript (search, tabs, modals, navigation)
├── assets/
│   └── icons/              # UI icons and graphics
└── README.md
```

---

## Impact & Vision

Salone HealthConnect exists to ensure that **no life in Sierra Leone is lost** simply because someone could not find the nearest hospital, did not know which doctor to see, or could not reach a blood donor in time.

By centralizing verified healthcare information in a low-cost, mobile-friendly platform, the project directly supports Sierra Leone's national health goals and lays the foundation for a fully connected healthcare ecosystem — one that serves every citizen, from Freetown to the most remote community in Kono or Tonkolili.

### Roadmap

- [ ] SMS-based appointment confirmations and reminders
- [ ] Offline-first PWA (Progressive Web App) mode
- [ ] Community health worker portal with field data entry
- [ ] Real-time blood stock API integration with participating facilities
- [ ] Multilingual support (Krio, Temne, Mende)
- [ ] USSD fallback channel for feature phones

---

## Contributing

Contributions are welcome. If you work in healthcare, technology, or community outreach in Sierra Leone — or simply want to help — please open an issue or submit a pull request.

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m "Add: brief description"`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a pull request

Please review our [Contributing Guidelines](CONTRIBUTING.md) and [Code of Conduct](CODE_OF_CONDUCT.md) before submitting.

---

## License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute this software with attribution.

---

<div align="center">

**Built with purpose for Sierra Leone 🇸🇱**

*Emergency Line: 999 · Ambulance: 117*

</div>

# Sentinel — Threat Intelligence Dashboard

**Sentinel** is a modern, interactive security operations center (SOC) dashboard designed for real-time threat monitoring, incident response, and network visualization. Built as a single-page HTML/CSS/JS application, it provides security analysts with a comprehensive, dark-themed interface to track alerts, analyze attack vectors, and manage security posture.

## ✨ Features

### Core Modules
- **Overview Dashboard** – Live security posture gauge, key metrics counters, threat activity timeline, and distribution charts.
- **Threat Feed** – Sortable and filterable table of active threats with severity indicators, search, and export to CSV.
- **Network Map** – Animated, interactive topology visualization with real-time attack path animations and node inspection.
- **Analytics Hub** – MTTR trend analysis, hourly alert volume chart, and geographic threat origin mapping.
- **Incident Management** – Track and resolve security incidents with status updates and drill-down details.
- **Asset Inventory** – Risk-scored asset list with filtering and visual risk indicators.
- **Detection Rules** – Manage and toggle detection rules on/off with a clean switch interface.

### Interactive Elements
- **Drill-down Panels** – Click any threat, incident, or notification to view detailed context and recommended actions.
- **Modals** – Add new threats, incidents, or rules inline without leaving the dashboard.
- **Live Clock & Auto-refresh** – Real-time UTC clock and periodic data updates simulate live event ingestion.
- **Heatmap** – Visualize event distribution across days and hours with color-coded density.
- **Chart.js Visualizations** – Bar charts, line graphs, donut charts, and radar charts for deep insights.

### Technical Highlights
- **Responsive Design** – Works on desktop, tablet, and mobile with collapsible sidebar.
- **Dark/Light Theme Toggle** – Switch between light and dark modes with preserved data.
- **GSAP Animations** – Smooth page transitions and fade-in effects.
- **Canvas Network Topology** – Custom-drawn network map with moving attack indicators.
- **Local Data Simulation** – Fully functional with realistic mock data, ready to connect to a backend API.

## 🖼️ Screenshots

> *Add your screenshots here to showcase the interface.*

| Overview Dashboard | Threat Feed |
|-------------------|-------------|
| *[Insert screenshot of main dashboard]* | *[Insert screenshot of threat table]* |

| Network Map | Analytics |
|------------|----------|
| *[Insert screenshot of network canvas]* | *[Insert screenshot of MTTR charts]* |

## 🚀 Getting Started

### Prerequisites
No build tools or server required. Any modern web browser (Chrome, Firefox, Safari, Edge) is sufficient.

### Installation & Usage
1. Clone or download the repository.
2. Open `index.html` directly in your browser.
   ```bash
   # If you have a local server (optional)
   npx serve

   🔧 Customization
Data Integration
All data is currently served from static JavaScript arrays (e.g., THREATS, ASSETS, RULES). To connect to a live backend:

Replace the THREATS array with API fetch calls inside renderThreatTable().

Modify liveRefresh() to pull real-time events from a WebSocket or REST endpoint.

Theming
CSS custom properties (variables) are used extensively. Edit the :root block to adjust colors, spacing, and border radii.

The toggleTheme() function toggles between light and dark variable sets.

Charts
Charts are initialized with Chart.js. Data for charts can be updated by modifying the buildTimelineData() function and other chart initialization functions.

👨‍💻 Developer
Afaq Ahmad
Security Dashboard Architect & Developer

This project was designed and built as a comprehensive demonstration of a modern security monitoring interface, combining real-time data visualization with practical SOC workflows.

📄 License
This project is released under the MIT License. Feel free to use, modify, and distribute with appropriate attribution.


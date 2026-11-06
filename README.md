🛸 Space Hazard Tracker

A real-time space and Earth hazard monitoring dashboard powered by NASA's Open APIs.

Space Hazard Tracker brings together information about Near-Earth Objects (NEOs), space weather events, and active environmental hazards in one interactive dashboard.

The project combines hands-on web development with AI-assisted coding to explore how real-world APIs, backend services, and modern frontend technologies can work together.

🌌 Features

☄️ Near-Earth Object Tracking
- Tracks asteroids approaching Earth using NASA's NeoWs API.
- Displays physical characteristics and proximity information.
- Provides hazard-level assessments based on asteroid data.

 ☀️ Space Weather Monitoring
- Monitors solar activity through NASA's DONKI API.
- Covers solar flares, coronal mass ejections (CMEs), and geomagnetic storms.
- Includes simulated fallback data when the DONKI API is unavailable.

🌍 Earth Hazards Map
- Interactive global map powered by Leaflet.
- Displays active environmental events such as wildfires, volcanoes, and storms.
- Uses NASA's Earth Observatory Natural Event Tracker (EONET).

 📊 Hazard Overview
- Provides an overview of cosmic and terrestrial hazard information.
- Displays summary statistics for the upcoming week.
- Brings different NASA data sources together in one dashboard.

 🎨 User Interface
- Dark space-inspired design.
- Responsive dashboard layout.
- Interactive data visualizations and map-based exploration.

 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| Frontend | React 18, TypeScript, Vite |
| Mapping | Leaflet |
| Styling | CSS3, Custom Design System |
| Backend | Node.js, Express.js |
| HTTP Requests | Axios |
| Caching | NodeCache |
| Validation | Zod |
| Security | Helmet, Express Rate Limit |
| APIs | NASA NeoWs, DONKI, EONET |
| AI-assisted Development | Google Antigravity, Google AI Studio |

## 🏗️ Application Architecture

The application follows a frontend-backend architecture.


              USER
                |
                v
        REACT FRONTEND
       (React + TypeScript)
                |
                v
        EXPRESS BACKEND
                |
       +--------+--------+
       |        |        |
       v        v        v
     NeoWs    DONKI    EONET
       |        |        |
       +--------+--------+
                |
                v
        NASA API RESPONSES
                |
                v
       PROCESSING & CACHING
                |
                v
        FRONTEND DASHBOARD

 🔌 NASA API Integration

This project uses three NASA data services:

**1. NASA NeoWs – Near-Earth Object Web Service**

Retrieves asteroid information, including estimated size, velocity, and distance from Earth.

https://api.nasa.gov/

**2. NASA DONKI – Space Weather Database**

Provides information about solar flares, coronal mass ejections, and geomagnetic storms.

https://ccmc.gsfc.nasa.gov/tools/DONKI/

**3. NASA EONET – Earth Observatory Natural Event Tracker**

Provides information about active natural events across the globe.

https://eonet.gsfc.nasa.gov/

🚀 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm
- NASA API key

Get your free NASA API key from:

https://api.nasa.gov/

Installation

**1. Clone the repository**

```bash
git clone https://github.com/YOUR_USERNAME/space-hazard-tracker.git
cd space-hazard-tracker
```

**2. Install dependencies**

```bash
npm install
```

**3. Configure environment variables**

Create a `.env` file in the root directory:

```env
NASA_API_KEY=your_nasa_api_key
PORT=3002
CACHE_TTL_SECONDS=300
```

**4. Start the application**

```bash
npm run dev
```

The application will be available at:

- Frontend: http://localhost:5173
- Backend: http://localhost:3002

*Note: These commands and environment settings assume the root-level package configuration used by this project.*

🛡️ Architecture & Security

**API Proxying**

NASA API requests are handled through the Express backend, keeping the API key away from the frontend.

**Caching**

NodeCache reduces repeated requests to external NASA services and helps improve response efficiency.

**Input Validation**

Zod validates incoming request parameters to help prevent invalid requests.

**Security Headers & Rate Limiting**

Helmet and Express Rate Limit provide additional protection for the backend.

**Fallback Handling**

The DONKI integration includes simulated fallback data when the external service is unavailable. Simulated results should not be interpreted as live NASA observations.

🤖 AI-Assisted Development

This project was developed through a combination of hands-on programming and AI-assisted development.

Google Antigravity and Google AI Studio were explored as development tools during the workshop.

The development process involved working with:
- Frontend and backend integration.
- API communication and response handling.
- Debugging and code refinement.
- Understanding how different application components interact.
- Using AI tools to support coding and problem-solving.

The focus was not just on generating code, but also on understanding the implementation and how the different technologies work together.

📚 Key Learning Outcomes

- Integrating multiple external APIs into one application.
- Building frontend interfaces using React and TypeScript.
- Developing backend services with Node.js and Express.
- Understanding API security and server-side key management.
- Implementing caching and input validation.
- Working with interactive geographical maps.
- Exploring AI-assisted software development workflows.

🔮 Future Improvements

- Introduce customizable asteroid proximity alerts.
- Add historical space weather comparisons.
- Improve hazard prediction and visualization.
- Add user-configurable monitoring preferences.
- Expand the range of NASA data sources.

🙌 Acknowledgements

Developed during the workshop:

**Build a Live NASA Space Hazard Tracker from Scratch**

Organized by White Coding, with hands-on exposure to Google Antigravity, Google AI Studio, and NASA's open data APIs.

---

⭐ Thanks for exploring Space Hazard Tracker!

**Built with curiosity, coding, and AI-assisted development. 🚀**

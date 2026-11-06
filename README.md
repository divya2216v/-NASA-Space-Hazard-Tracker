# 🛸 Space Hazard Tracker

A real-time dashboard for monitoring cosmic and terrestrial hazards using NASA's Open APIs. This application tracks Near-Earth Objects (NEOs), Space Weather events (Solar Flares, CMEs, Geomagnetic Storms), and active Earth hazard events like wildfires and storms.

<img width="1906" height="918" alt="image" src="https://github.com/user-attachments/assets/d2f8eea3-edc7-4f91-b21e-c5f53e4ab3f2" />
<img width="1786" height="855" alt="image" src="https://github.com/user-attachments/assets/c00aa66e-3d11-45da-8989-746923e8ec60" />
<img width="1825" height="817" alt="image" src="https://github.com/user-attachments/assets/b7bd9277-dc7d-488b-abb8-973f32956e0a" />


## � Features

- **Near-Earth Object Watch**: Real-time tracking of asteroids approaching Earth, with hazard level assessments and physical characteristics.
- **Space Weather Monitoring**: Monitoring of solar activity including flares, coronal mass ejections, and geomagnetic storms with automated failover to simulated data during API outages.
- **Earth Hazards Map**: Interactive global map displaying active events (wildfires, volcanoes, storms) via NASA's EONET service.
- **Hazard Overview**: Quick-glance statistics of cosmic and global threats for the upcoming week.
- **Dark Space Aesthetic**: A premium, responsive UI designed for optimal viewing in low-light environments.

## 🛠️ Tech Stack

- **Frontend**: React 18, TypeScript, Vite, Leaflet (Map), CSS3 (Custom Design System)
- **Backend**: Node.js, Express, Axios, Node-Cache, Zod (Validation)
- **APIs**: NASA NeoWs, NASA DONKI, NASA EONET
- **Security**: Express Helmet, Rate Limiting, Server-side API key proxying

## 🚀 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- A NASA API Key (Get one for free at [api.nasa.gov](https://api.nasa.gov/))

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/space-hazard-tracker.git
   cd space-hazard-tracker
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Configure Environment**:
   Create a `.env` file in the root directory:
   ```env
   NASA_API_KEY=your_api_key_here
   PORT=3002
   CACHE_TTL_SECONDS=300
   ```

4. **Run the application**:
   ```bash
   npm run dev
   ```
   The frontend will be available at `http://localhost:5173` and the backend proxy at `http://localhost:3002`.

## 🛡️ Architecture & Security

- **API Proxying**: The client never sees the NASA API key. All requests are proxied through the Express server.
- **Caching**: Implemented `node-cache` to reduce API overhead and improve performance.
- **Resilience**: Integrated automated simulated data failover for NASA's DONKI service to ensure the dashboard remains functional during external service outages.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
Built with 🚀 for Space Enthusiasts.

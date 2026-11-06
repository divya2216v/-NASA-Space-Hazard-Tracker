# Space Hazard Tracker — Build Plan

## Stack
- Frontend: Vite + React + TypeScript
- Backend: Express proxy (server/) with caching, validation, friendly errors
- Map: Leaflet (lazy-loaded)

## Steps
A. Scaffold: Vite+React+TS project, Express server in server/, .gitignore, .env.example
B. Proxy routes: /api/health, /api/asteroids, /api/space-weather, /api/events, /api/overview
   - node-cache for caching, zod for input validation, never expose API key
C. Frontend foundation: dark theme CSS, layout shell, Skeleton, ErrorState, typed fetch helpers
D. Hazard Overview strip (summary counts from /api/overview)
E. Asteroid Watch section (table/cards from /api/asteroids)
F. Space Weather section (/api/space-weather)
G. Earth Hazards Map — lazy-loaded Leaflet, /api/events, category filters
H. Footer with NASA credit
I. verify-app skill → fix issues
J. security-audit skill → fix issues, never print key
K. Final report (≤10 lines)

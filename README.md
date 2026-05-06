[🌤️ SkyNarrata 🌙]

The sky narrated... your daily story of weather and wonder.

SkyNarrata is a beautiful, responsive weather application that blends real-time meteorological data with astronomical insights, including moon phase calendars and NASA’s Astronomy Picture of the Day.

✨ Features
🌍 Smart Weather Search
Coordinate-based accuracy – get precise weather for any location

Disambiguate city names – e.g., Nassau, Bahamas vs. Nassau, Minnesota

Country codes & state info – for clear identification

Real-time autocomplete – search as you type

Smart filtering – dropdown with 15+ accurate city variations

🌙 Astronomical Moon Phase Calendar
8-day lunar calendar with phase calculations

Moonrise/set times based on your coordinates

Educational phase descriptions and percentages

Timezone-aware calculations

Emoji visuals for each moon phase

🚀 NASA Astronomy Picture of the Day
Archive dating back to 1995

High-res images and videos with expert explanations

Custom date picker

Direct NASA links for further learning

🎨 Beautiful User Experience
Cosmic themes with glassmorphism

Adaptive weather backgrounds

Fully responsive and WCAG accessible

Smooth animations and a dark theme for evening viewing

🔐 Production-Ready Security
API keys handled server-side

Environment variables for local and production use

Secure proxy routes

HTTPS ready

🛠️ Technology Stack
Core Framework
Next.js 14 – App Router architecture

TypeScript – strict typing for safer code

Tailwind CSS – utility-first styling

UI Components
Custom glassmorphism components (Card, Button, Input, Select)

Responsive design from mobile to desktop

Accessible components (WCAG-compliant)

Subtle transitions and animations

APIs & Data Sources
OpenWeatherMap – weather + geolocation

NASA APOD – public astronomy education API

Custom astronomical engine – moon phase calculations done locally

Hosting & Tools
Replit – lightweight cloud deployment

Ohara – agent-based automation and UI/UX builder

Environment-based routing – secure .env setup for keys

🧱 Project Structure
lua
Copy code
skynarrata/
├── public/
│   ├── icon-192.png
│   ├── icon-512.png
│   └── favicon.ico
├── src/
│   ├── app/
│   │   ├── api/
│   │   │   ├── nasa-apod/route.ts
│   │   │   └── proxy/route.ts
│   │   ├── moon-phases/page.tsx
│   │   ├── apod/page.tsx
│   │   ├── globals.css
│   │   ├── layout.tsx
│   │   └── page.tsx
│   ├── components/ui/
│   │   ├── button.tsx
│   │   ├── card.tsx
│   │   ├── input.tsx
│   │   └── select.tsx
│   └── lib/
│       ├── weatherApi.ts
│       ├── nasaApi.ts
│       └── utils.ts
├── .env.example
├── .env.local
├── .gitignore
├── package.json
├── tailwind.config.js
├── tsconfig.json
├── next.config.js
└── README.md
🚀 Quick Start
Prerequisites
Node.js 18 or higher

npm / yarn / pnpm

NASA API key

OpenWeatherMap API key (provided for dev)

🌟 Unique Features
Location Accuracy
No more weather mismatches: Get local data based on exact coordinates

Supports ambiguous cities like Paris, Texas or St. Petersburg, Florida

Enhanced Search
Fuzzy matching: handles "St Petersburg" and "Saint Petersburg"

Smart deduplication, shows unique results only

Clean dropdown UI with up to 8 results

Astronomical Education
Phase explanations & moonrise/set

NASA media with scientific descriptions

Archive with 29+ years of photos

Emoji moon phases for every day

📱 Mobile Optimization
Mobile-optimized interactions, buttons, and pickers

Lazy loading and debounced API calls

Swipe gesture support

Fast initial load for slower connections

🔧 Configuration
Environment Variables
ini
Copy code
# Required
WEATHER_API_KEY=your-openweathermap-api-key
NASA_API_KEY=your-nasa-api-key

# Optional
NODE_ENV=development
Customization Options
Change background logic in getWeatherBackground()

Replace emojis in MOON_PHASE_EMOJIS

Adjust search limits and theme colors via config files

✅ Testing Checklist
 Test weather accuracy (e.g., Saint Petersburg, FL vs. RU)

 Check moon phase calculations across timezones

 Verify NASA APOD images on different dates

 Test responsiveness on mobile devices

 Confirm dropdown filtering and search behavior

📄 License
Licensed under the MIT License. See LICENSE for full details.

🙏 Acknowledgments
NASA

OpenWeatherMap

Next.js

Tailwind CSS

Ohara – AI-assisted front-end builder

The astronomy and open source communities 🌌

🌤️ SkyNarrata 🌙

Built with Ohara

The sky narrated... your daily story of weather and wonder.

A beautiful, responsive weather application that combines real-time meteorological data with astronomical information. Built with Next.js, featuring coordinate-based weather accuracy, moon phase calculations, and NASA's Astronomy Picture of the Day.

Next.js TypeScript Tailwind
✨ Features
🌍 Smart Weather Search

    Coordinate-based accuracy - Get weather for the exact location you select

    Global city disambiguation - Choose between Nassau, Bahamas vs Nassau, Minnesota

    Country codes and state information - Clear location identification

    Real-time autocomplete - Search results as you type

    Enhanced dropdown - Up to 15 city variations with smart filtering

🌙 Astronomical Moon Phase Calendar

    8-day lunar calendar with precise phase calculations

    Moonrise and moonset times for any location

    Phase percentage and descriptions

    Educational content about lunar cycles

    Timezone-aware calculations based on coordinates

    Beautiful lunar emoji representations for each phase

🚀 NASA Astronomy Picture of the Day

    Historical archive dating back to June 16, 1995

    High-resolution images and videos

    Professional astronomical explanations

    Custom date picker with year, month, and day selection

    Educational space content from NASA astronomers

    HD image viewing with direct NASA links

🎨 Beautiful User Experience

    Cosmic gradient themes with glassmorphism effects

    Weather-adaptive backgrounds that change based on conditions

    Fully responsive design for all screen sizes

    Accessible UI meeting WCAG standards

    Smooth animations and loading states

    Dark theme optimized for nighttime and cloudy skies

🔐 Production-Ready Security

    Server-side API key management - No exposed credentials

    Environment variable configuration

    Secure API proxy endpoints

    HTTPS deployment ready

🏗️ Project Structure
skynarrata/
├── public/
│   ├── icon-192.png          # App icon (192x192)
│   ├── icon-512.png          # App icon (512x512)
│   └── favicon.ico           # Browser favicon
│
├── src/
│   ├── app/
│   │   ├── api/
│   │   │   ├── nasa-apod/
│   │   │   │   └── route.ts   # Secure NASA API endpoint
│   │   │   └── proxy/
│   │   │       └── route.ts   # API proxy for external calls
│   │   │
│   │   ├── moon-phases/
│   │   │   └── page.tsx       # Moon phase calendar page
│   │   │
│   │   ├── apod/
│   │   │   └── page.tsx       # NASA APOD page
│   │   │
│   │   ├── globals.css        # Global styles and Tailwind
│   │   ├── layout.tsx         # Root layout with metadata
│   │   └── page.tsx           # Main weather page
│   │
│   ├── components/
│   │   └── ui/
│   │       ├── button.tsx     # Reusable button component
│   │       ├── card.tsx       # Glassmorphism card component
│   │       ├── input.tsx      # Search input component
│   │       └── select.tsx     # Dropdown select component
│   │
│   └── lib/
│       ├── weatherApi.ts      # Weather data fetching and geocoding
│       ├── nasaApi.ts         # NASA APOD API integration
│       └── utils.ts           # Utility functions
│
├── .env.example               # Environment variable template
├── .env.local                 # Local development environment (not committed)
├── .gitignore                 # Git ignore rules
├── package.json               # Dependencies and scripts
├── tailwind.config.js         # Tailwind CSS configuration
├── tsconfig.json              # TypeScript configuration
├── next.config.js             # Next.js configuration
└── README.md                  # This file
🚀 Quick Start
Prerequisites

    Node.js 18.0 or higher

    npm, yarn, or pnpm package manager

    Weather API key (included for development)

    NASA API key (get free at api.nasa.gov)

🛠️ Technology Stack
Core Framework

    Next.js 14 - React framework with App Router

    TypeScript - Type-safe JavaScript

    Tailwind CSS - Utility-first CSS framework

UI Components

    Custom components with glassmorphism effects

    Responsive design for all screen sizes

    WCAG accessibility compliance

    Smooth animations and transitions

APIs & Data

    OpenWeatherMap - Weather data and geocoding

    NASA APOD - Astronomy pictures and educational content

    Custom astronomical calculations - Moon phases and lunar data

Key Features

    Coordinate-based weather lookup - Eliminates location ambiguity

    Multi-variation city search - Enhanced geocoding with 15+ results

    Local moon phase calculations - No external API dependencies

    Secure server-side routes - Protected API key management

🎨 Design Philosophy
Cosmic Theme

    Gradient backgrounds inspired by space and sky

    Glassmorphism effects for modern, translucent UI

    Weather-adaptive colors that change based on conditions

    Astronomical imagery integration

    Dark theme optimization for better contrast

User Experience

    Coordinate-based accuracy eliminates location confusion

    Educational content makes learning engaging

    Mobile-first design optimized for touch interfaces

    Fast loading with optimized performance

    Progressive enhancement for all device capabilities

🌟 Unique Features
Location Accuracy Problem Solved

    Nassau, Minnesota shows Minnesota weather (45.38°, -95.83°)

    Saint Petersburg, Florida shows Florida weather, not Russia

    Paris, Texas shows Texas weather, not France

    Coordinate-based API calls prevent wrong location data

Enhanced Search Experience

    Multiple search variations - tries "saint petersburg", "st petersburg"

    Smart result deduplication - no duplicate cities in dropdown

    Country and state codes - clear location identification

    Up to 8 visible results - optimal UI balance

Astronomical Education

    Moon phase descriptions - learn about lunar cycles

    NASA educational content - professional astronomical explanations

    Historical space imagery - 29+ years of APOD archive

    Location-aware calculations - accurate for any timezone

Code Guidelines

    TypeScript required - No implicit any types

    Responsive design - Test on mobile and desktop

    Accessibility - Follow WCAG guidelines

    Performance - Optimize images and API calls

    Security - Never expose API keys client-side

Testing Checklist

    Test weather search with various city names (Nassau MN, Saint Petersburg FL)

    Verify moon phase calculations for different timezones

    Check NASA APOD functionality with different dates

    Ensure mobile responsiveness across devices

    Test dropdown behavior and coordinate accuracy

📱 Mobile Optimization
Responsive Features

    Touch-optimized dropdown interactions

    Mobile-friendly date picker for NASA APOD

    Glassmorphism effects that work on all screen sizes

    Optimized loading states for slower connections

    Swipe gestures for navigation between features

Performance

    Optimized images from NASA with proper loading

    Debounced search to prevent excessive API calls

    Lazy loading for non-critical components

    Efficient caching of weather and astronomical data

🔧 Configuration
Environment Variables
# Required for production
WEATHER_API_KEY=your-openweathermap-api-key
NASA_API_KEY=your-nasa-api-key

# Optional for development
NODE_ENV=development
Customization Options

    Weather backgrounds - Modify getWeatherBackground() function

    Moon phase emojis - Update MOON_PHASE_EMOJIS constant

    City search limits - Adjust geocoding result limits

    Theme colors - Modify Tailwind config for cosmic gradients

📄 License

This project is licensed under the MIT License - see the LICENSE file for details.
🙏 Acknowledgments

    NASA for providing the Astronomy Picture of the Day API

    OpenWeatherMap for weather data and geocoding services

    Next.js team for the excellent React framework

    Tailwind CSS for the utility-first styling approach

    The astronomy community for inspiring beautiful space-themed design


# Healthcare Portal - Frontend

Modern healthcare portal application built with React, Vite, and TailwindCSS-inspired styling.

## Features

- 🏥 **Doctor Search & Booking**: Browse and book appointments with healthcare providers
- 📅 **Appointment Management**: View, track, and manage your appointments
- 👤 **User Profile**: Manage personal information and health records
- 📊 **Health Dashboard**: Track vitals and health metrics with interactive charts
- 🔐 **Authentication**: Secure login and user management
- 📱 **Responsive Design**: Works seamlessly on desktop and mobile devices

## Tech Stack

- **React 19** - UI framework
- **Vite** - Build tool and dev server
- **React Router** - Client-side routing
- **TanStack Query** - Data fetching and caching
- **Recharts** - Data visualization
- **CSS Modules** - Scoped styling

## Getting Started

### Prerequisites

- Node.js >= 18.0.0
- npm or yarn

### Installation

```bash
# Install dependencies
npm install

# Create environment file (optional)
# Update the API URL if needed
```

### Development

```bash
# Start development server (port 5173)
npm run dev
```

Visit [http://localhost:5173](http://localhost:5173)

### Build

```bash
# Build for production
npm run build

# Preview production build
npm run preview
```

## Environment Variables

For local development with local backend:
```env
VITE_API_URL=http://localhost:3001/api
```

For production (using deployed backend):
```env
VITE_API_URL=https://your-backend-url.vercel.app/api
```

## Deployment to Vercel

1. Push code to GitHub
2. Import repository in Vercel
3. Configure:
   - Framework: Vite
   - Build Command: `npm run build`
   - Output Directory: `dist`
4. Add environment variable (if needed):
   - `VITE_API_URL`: Your backend API URL
5. Deploy!

## Features Overview

### Doctor Search
- Filter by specialty and location
- Search by doctor name
- View detailed doctor profiles

### Appointments
- Book new appointments
- View upcoming appointments
- Cancel appointments

### Dashboard
- Health vitals tracking
- Appointment overview
- Quick access features

## License

MIT

# 🌍 Raintor Technical Assessment — Real-Time Location Sharing & User Feed

A comprehensive **Next.js 14** application demonstrating:

- 🔴 Real-time GPS location sharing using **SignalR**
- 👥 Infinite scroll user feed using **React Query** and **IntersectionObserver**
- 🗺️ Live map integration via **Leaflet**
- 💅 Fully responsive UI using **Tailwind CSS** and **shadcn/ui**

---

## 🚀 Features

### ✅ Task 1: Real-Time Location Sharing (SignalR)

- Real-time WebSocket communication via **SignalR**
- Dual interface: **User A** (sender) and **User B** (receiver)
- Interactive **Leaflet** map with real-time updates
- Browser **Geolocation API** integration (manual & live GPS)
- Custom `useSignalR()` hook with:
  - Auto-reconnection
  - Connection status monitoring
  - Graceful error handling

### ✅ Task 2: Infinite Scroll User Feed

- Paginated user feed with infinite scroll
- **React Query** for data fetching and caching
- Virtualized rendering using **react-window**
- Skeleton loaders, error boundaries, and retry UI
- Responsive grid layout
- Accessible: Keyboard navigation, ARIA labels

---

## 🛠️ Tech Stack

| Tool              | Purpose                                |
|-------------------|----------------------------------------|
| **Next.js 14**    | Full-stack React framework (App Router)|
| **TypeScript**    | Static typing and type safety          |
| **Tailwind CSS**  | Utility-first CSS styling              |
| **shadcn/ui**     | Styled, accessible React UI components |
| **SignalR**       | Real-time WebSocket communication      |
| **Leaflet**       | Interactive map rendering              |
| **React Query**   | API handling, caching, pagination      |
| **react-window**  | Performance-friendly virtual list      |
| **Lucide Icons**  | Clean, modern SVG icons                |

---

## 📦 Installation & Setup

### ✅ Prerequisites

- Node.js `v18+`
- npm `v8+` (or yarn)

### 🔧 Local Development

```bash
# 1. Clone the repository
git clone https://github.com/Sohag00879/location-sharing-project.git
cd location-sharing

# 2. Install dependencies
npm install

# 3. Start the development server
npm run dev

# 4. Open in browser
http://localhost:3000 
````

🔌 API Integration

📡 SignalR Hub
Hub URL: https://tech-test.raintor.com/Hub

Features:

Real-time GPS broadcasting

Auto-reconnection with state tracking

Integrated into a reusable useSignalR() hook

📂 User Feed API
Endpoint: https://tech-test.raintor.com/api/users/GetUsersList

Features:

Infinite scrolling support

Error retry mechanism with exponential backoff

Virtualized rendering for performance

# SIMS - Sports Information Management System

A responsive frontend for a Sports Information Management System (SIMS) featuring role-based access, real-time leaderboards, event management, and player profiles. Built with React, TypeScript, and Tailwind CSS.

## ✨ Features

- **Role-Based Access Control**: Different views and permissions for Users, Team Leads, Officers, and Admins.
- **Real-Time Leaderboard**: Live updates on team rankings, scores, and placement statistics.
- **Dynamic Dashboard**: At-a-glance view of top teams and overall standings with data visualizations.
- **Comprehensive Event Management**: Create, update, delete, and view detailed event information including mechanics and criteria.
- **Team Hub**: Detailed team pages with member rosters, leadership structure, and score history.
- **User Profiles**: View and edit personal information and event interests.
- **Admin Panel**: Centralized control over user roles and content visibility.
- **Dark Mode**: A sleek, modern UI with a fluid animated background and a toggle for dark/light themes.
- **Real-Time Sync**: Changes made on one device are instantly broadcast to all connected clients.

## 🛠️ Tech Stack

- **Frontend**: [React](https://react.dev/) 19 (via CDN), [TypeScript](https://www.typescriptlang.org/)
- **Routing**: [React Router](https://reactrouter.com/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) (via CDN)
- **Animation**: [Framer Motion](https://www.framer.com/motion/)
- **Data Visualization**: [Recharts](https://recharts.org/)
- **AI Integration**: [Google Gemini API](https://ai.google.dev/) for content generation.

## 🚀 Getting Started

This project is set up to run without a local build process, using modern browser features like import maps.

### Prerequisites

- A modern web browser that supports import maps (e.g., Chrome, Firefox, Edge).
- A simple local HTTP server.

### Setup

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/your-username/sims-frontend.git
    cd sims-frontend
    ```

2.  **API Key Configuration:**
    This project uses the Google Gemini API for certain features. The API key is expected to be available in the execution environment as `process.env.API_KEY`. For local development, you will need to find a way to make this variable available to the browser.
    
    > **Note:** Do not hardcode your API key directly in the source code.

3.  **Serve the files:**
    Since the app uses ES modules, you need to serve the `index.html` file through a local web server. You cannot open it directly from the file system (`file:///...`).

    A simple way to do this is using the `serve` package:
    ```sh
    # If you have Node.js installed
    npx serve
    ```
    Alternatively, if you have Python installed:
    ```sh
    # Python 3
    python -m http.server
    ```
    Then, open your browser and navigate to the local address provided (e.g., `http://localhost:3000` or `http://localhost:8000`).

## 📁 Project Structure

```
.
├── index.html          # Main HTML entry point with import map
├── index.tsx           # React application root
├── metadata.json       # Project metadata
├── src/
│   ├── App.tsx             # Main app component with routing
│   ├── components/       # Reusable UI components
│   ├── constants.ts      # App-wide constants
│   ├── contexts/         # React context providers
│   ├── hooks/            # Custom React hooks
│   ├── pages/            # Page components for each route
│   ├── services/         # API service modules (mock and Gemini)
│   └── types.ts          # TypeScript type definitions
└── ...
```

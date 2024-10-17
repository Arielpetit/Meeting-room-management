# Meeting Room Manager 

## Table of Contents
 - [Project Overview](#project-overview)
  - [Features](#features)
  - [Technologies Used](#technologies-used)
  - [Prerequisites](#prerequisites)
  - [Installation Instructions](#installation-instructions)
  - [Usage](#usage)
  - [Project Structure](#project-structure)
  - [Development and Contribution](#development-and-contribution)
  - [License](#license)
  - [Contact Information](#contact-information)
  - [Acknowledgements](#acknowledgements)

## Project Overview

The **Meeting Room Manager** is a web-based application designed to help users and administrators efficiently manage the booking of meeting rooms. It offers a user-friendly interface to view available rooms, book time slots, and manage room schedules via a calendar interface. As a Progressive Web App, it provides offline functionality, notifications, and can be installed on mobile and desktop devices.

---

## Features

### User Features
- **View Available Rooms**: Browse a list of rooms with descriptions, capacities, and availability.
- **Book a Meeting Room**: Easily select an available time slot for a room and confirm a booking.
- **Calendar View**: Visualize the availability of each room via a calendar interface.
- **Modify/Cancel Bookings**: Users can update or cancel their bookings from a personal dashboard.
- **Offline Mode**: Browse room availability and make bookings even while offline, syncing when back online.
- **Push Notifications**: Receive reminders for upcoming meetings or booking updates.

### Admin Features
- **Add/Edit/Delete Rooms**: Admin users can manage the rooms available for booking.
- **Manage Bookings**: Admins can view and manage all user bookings, with full control to modify or cancel reservations.

### PWA Features
- **Offline Support**: Leverage service workers to cache content for offline use.
- **Installable App**: Users can install the app on their devices for a native-like experience.
- **Push Notifications**: Notify users of upcoming meetings or booking reminders.
- **Fast Load Times**: Optimized caching strategies provide fast loading even in low network conditions.

---

## Technologies Used

- **Frontend**:
  - React.js (with hooks and context)
  - React Router for SPA navigation
  - react-big-calendar for interactive calendar view
  - Tailwind CSS or Material-UI for styling
- **Backend** (Optional, for a full-stack implementation):
  - Node.js with Express.js
  - MongoDB or any database for persistence
- **Mock API**:
  - json-server for mock data during development
- **PWA Tools**:
  - Service workers for offline caching
  - Push API for notifications
- **Database** (optional):
  - MongoDB or any database solution

---

## Prerequisites

Ensure that the following are installed on your system:

- [Node.js](https://nodejs.org/) (v14 or higher)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)
- Git

---

## Installation Instructions

Follow the steps below to set up the project on your local machine:

### Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/meeting-room-manager.git
cd meeting-room-manager
```

### Step 2: Install Dependencies

Using npm:

```bash
npm install
```

Or using yarn:

```bash
yarn install
```

### Step 3: Start the Development Server

Using npm:

```bash
npm run dev
```

Or with yarn:

```bash
yarn dev
```

This will start the app at [http://localhost:3000].

### Step 4: Set up a Mock API (Optional)

To mock the backend API, use json-server:

#### Install json-server:

```bash
npm install -g json-server
```

#### Create a `db.json` file with the following structure:

```json
{
  "rooms": [],
  "bookings": []
}
```

#### Start the mock server:

```bash
json-server --watch db.json --port 5000
```

## Usage

### Booking a Room

1. View the list of available rooms on the homepage.
2. Select a room to view its available time slots in a calendar view.
3. Choose an available time slot and complete the booking form to reserve the room.

### Managing Bookings

Users can view their existing bookings on the "My Bookings" page and make updates or cancel bookings as needed.

### Admin Panel

Admin users can add, edit, or remove meeting rooms from the "Admin Panel".  
Admins can also view and manage all user bookings.

### PWA Functionality

- Install the app from your browser using the "Add to Home Screen" option for mobile or desktop.
- Offline support ensures you can access previously loaded data and make bookings that sync when back online.
- Receive push notifications for reminders and updates on your bookings.

## Project Structure

```plaintext
├── CHANGELOG.md                  // Log of changes made to the project
├── e2e                           // End-to-end tests
│   ├── hotkeys                   // Hotkeys test suite
│   └── theme                     // Theme-related test suite
├── env                           // Environment configurations
├── index.html                    // Main HTML file for the app
├── LICENSE                       // License information
├── manifest.json                 // Web app manifest for PWA
├── package.json                  // Node.js project metadata
├── package-lock.json             // Dependency lock file
├── playwright.config.ts          // Playwright configuration for E2E testing
├── public                        // Public assets folder
│   ├── apple-touch-icon.png      // Apple touch icon for PWA
│   ├── audit.png                 // Performance audit result image
│   ├── bundle.png                // Bundle size visualization
│   ├── cover.png                 // App cover image
│   ├── demo-dark.png             // Demo image for dark theme
│   ├── demo-light.png            // Demo image for light theme
│   ├── favicon.ico               // Favicon in .ico format
│   ├── favicon.svg               // Favicon in .svg format
│   ├── file-folder-structure.png // Visual representation of folder structure
│   ├── pwa-192x192.png           // PWA icon for 192x192 resolution
│   ├── pwa-512x512.png           // PWA icon for 512x512 resolution
│   ├── pwa-reload.png            // Reload image for PWA
│   ├── robots.txt                // Guide for search engine indexing
│   └── use-template.png          // Template usage image
├── README.md                     // Project documentation
├── src                           // Source files for the app
│   ├── App.tsx                   // Main application component
│   ├── components                // Reusable components
│   │   ├── Meta                  // Component for managing page metadata
│   │   └── styled.ts             // Styled components for reuse
│   ├── config                    // Application configuration
│   ├── error-handling            // Error handling mechanisms
│   ├── hooks                     // Custom React hooks
│   ├── main.tsx                  // Application entry point
│   ├── pages                     // Page components
│   ├── Root.tsx                  // Root application component
│   ├── routes                    // Routing configuration
│   ├── sections                  // Application sections (header, sidebar, etc.)
│   ├── store                     // Redux store for application state
│   ├── theme                     // Theme management
│   ├── utils                     // Utility functions
│   └── vite-env.d.ts             // TypeScript environment definitions for Vite
├── tsconfig.json                 // TypeScript configuration
├── tsconfig.node.json            // TypeScript config for Node.js
└── vite.config.ts                // Vite configuration file
```

## Development and Contribution

### Contribution Guidelines

We welcome contributions!
Please adhere to the project's coding standards [Contibution.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426)
## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Contact Information

For any questions, feedback, or contributions, feel free to reach out:

- **Name:** Tchikaya Ariel
- **Email:** Tchikayaline@gmail.com
- **GitHub:** [Arielpetit](https://github.com/arielpetit)

## Acknowledgements

A special thanks to the following resources and communities for providing invaluable tools and guidance:

- React.js - for building dynamic UIs.
- My team mates .
- Tailwind CSS - for modern, utility-first styling.
- react-big-calendar - for the amazing calendar component.
- MDN Web Docs - for comprehensive documentation.
- All open-source contributors who helped shape the web development ecosystem.

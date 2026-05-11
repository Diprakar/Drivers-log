# 🚛 Driver's Log Generator

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Leaflet](https://img.shields.io/badge/Leaflet-199900?style=for-the-badge&logo=Leaflet&logoColor=white)
![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)

A React-based frontend prototype designed to digitize daily driver logs. This project demonstrates complex UI/UX challenges, including an interactive 24-hour duty status grid and dynamic map visualization.

> **Note:** This is a frontend-only build. The application currently uses mock data to simulate trip generation for demonstration purposes.

**🔗 Live Demo:** [https://drivers-log-chi.vercel.app/](https://drivers-log-chi.vercel.app/)

## 🚀 Features

* **Interactive Log Grid:** Visualizes 24-hour duty cycles (Off Duty, Sleeper Berth, Driving, On Duty) using a custom CSS-based grid system.
* **Route Mapping:** Integrates **Leaflet Maps** to render route polylines and markers.
* **Trip Input Simulation:** Validated form that accepts trip details (Current Location, Pickup/Dropoff).
    * *Note: Submitting the form triggers a pre-defined demo scenario (Dhaka → Comilla → Chittagong).*
* **Automated Calculations:** Displays aggregated driving and on-duty hours based on the simulated dataset.
* **Responsive Design:** Fully responsive layout optimized for desktop and mobile viewing.

## 🛠 Tech Stack

* **Frontend Library:** [React.js](https://reactjs.org/) (v19)
* **Mapping Engine:** [React Leaflet](https://react-leaflet.js.org/) & [OpenStreetMap](https://www.openstreetmap.org/)
* **Styling:** CSS3, Flexbox
* **Deployment:** Vercel

## 📂 Project Structure

```bash
src/
├── components/
│   ├── TripInputForm.js  # Captures user input for locations & cycle
│   ├── LogSheet.js       # Renders the 24-hour duty status grid
│   ├── MapDisplay.js     # Renders the map with route polyline & markers
│   └── ...css            # Component-scoped styling
├── App.js                # Main state container & layout
└── index.js              # Entry point & Leaflet style imports

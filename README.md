# 🌦️ Real-Time Weather Monitoring System

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-1.0.0-brightgreen.svg)](https://github.com/yourusername/weather-monitoring-system)
[![Build Status](https://img.shields.io/badge/build-passing-success.svg)](https://github.com/yourusername/weather-monitoring-system/actions)
[![Coverage](https://img.shields.io/badge/coverage-85%25-success.svg)](https://github.com/yourusername/weather-monitoring-system/coverage)
[![Code Style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](https://standardjs.com)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![Node.js Version](https://img.shields.io/badge/node-%3E%3D%2012.0.0-brightgreen.svg)](https://nodejs.org/)
[![OpenWeatherMap](https://img.shields.io/badge/Powered%20by-OpenWeatherMap-orange.svg)](https://openweathermap.org/)

## 🌐 Hosted Link
[Access the application here](https://yourapplication.com)

## 📋 Overview
This project provides real-time weather data retrieval and analysis using the OpenWeatherMap API. It periodically fetches weather updates for specified locations, processes the data, and generates daily summaries, including weather statistics like average, maximum, and minimum temperatures, and dominant weather conditions. Additional parameters such as humidity and wind speed are also supported.
<p align="center">
  <img src="/api/placeholder/800/400" alt="Weather Dashboard Preview">
</p>

## ✨ Features

* **Real-Time Weather Data Retrieval**: Continuously fetches data from OpenWeatherMap API for cities such as Delhi, Mumbai, Chennai, Bangalore, Kolkata, and Hyderabad.
* **Daily Weather Summary**: Calculates daily aggregates like average, maximum, and minimum temperatures, along with determining the dominant weather condition.
* **Temperature Conversion**: Automatically converts temperatures from Kelvin to Celsius or Fahrenheit based on user preferences.
* **5-day Forecast**: Displays weather forecasts, including temperature, humidity, and wind speed for the next five days.
* **Alerting System**: Sends alerts (console or notification) when defined thresholds (like temperature) are breached.
* **Visualizations**: Historical weather trends, daily summaries, and triggered alerts can be visualized for better insights.
  
## 🛠️ Technical Stack

### Core Technologies
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

### Development Tools
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![NPM](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)

## 🏗 System Design
The application is designed with modularity and scalability in mind, making it easy to extend and maintain. Key modules include:

* **API Connection Module**: Handles connection to the OpenWeatherMap API and fetches data periodically.
* **Data Processing Module**: Processes weather data, including temperature conversion and summary calculation.
* **Alerting Module**: Monitors weather conditions and triggers alerts when thresholds are breached.
* **Visualization Module**: Displays weather summaries, trends, and alerts in a user-friendly way.
  
## 🚀 Getting Started

### Prerequisites
To run this system locally, you'll need:

* Node.js and npm installed on your machine
* An API key from OpenWeatherMap. Sign up at [OpenWeatherMap API](https://openweathermap.org/api) to get a free API key

### Installation

Follow these steps to set up the project:

1. **Clone the Repository**

   Open a terminal and run the following command to clone the repository:
   ```bash
   git clone [https://github.com/Karthickeien/Weather-Monitoring-System.git]
   cd Weather-Monitoring-System
   ```
2. **Install Dependencies**

   Install all required dependencies using npm:
   ```bash
   npm install
   ```

3. **Start the Live Server**

   If you're not using a live server tool, you can set up one by running:
   ```bash
   npm run dev
   ```

4. **Open the Application**

   Once the server is running, open your browser and go to `http://localhost:5173` to view the weather app.

## 🎯 Core Features

### 🌡️ Temperature Unit Conversion
```javascript
// Smart temperature conversion utility
const convertTemp = (temp, unit) => {
    switch(unit) {
        case "F": return ((temp * 9/5) + 32).toFixed(2);  // 🌡️ Fahrenheit
        case "K": return (temp + 273.15).toFixed(2);      // 🌡️ Kelvin
        default:  return temp.toFixed(2);                 // 🌡️ Celsius
    }
};
```

### 📊 Data Visualization
```javascript
// Example of weather data structure
const weatherData = {
    city: "Bangalore",
    temperature: 25,
    condition: "Clear",
    humidity: 65,
    windSpeed: 12
};
```

## 🧪 Test Cases

### 1. System Setup
* Verify that the system initializes correctly and connects to the OpenWeatherMap API with a valid API key

### 2. Data Retrieval
* Simulate API calls at configurable intervals to ensure the system retrieves data for specified locations and parses the data correctly

### 3. Temperature Conversion
* Test the temperature conversion functionality to ensure that temperature values are converted from Kelvin to Celsius or Fahrenheit accurately

### 4. Daily Weather Summary
* Simulate multiple weather updates over a period of time and verify that the system correctly calculates daily summaries, including average, maximum, and minimum temperatures

### 5. Alerting Thresholds
* Configure a user-defined threshold for a weather parameter (e.g., temperature) and simulate weather conditions exceeding that threshold
* Check that alerts are triggered as expected

## 🔮 Future Enhancements

* **Additional Weather Parameters**: Add support for additional weather data such as air pressure, cloud cover, and UV index
* **Forecast Summary**: Generate summaries and visualizations based on weather forecasts
* **Custom Alert Channels**: Implement alert notifications through different channels like email or SMS

## 📜 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## 🙏 Acknowledgments

- 🌤️ OpenWeatherMap for reliable weather data
- 🎨 Weather icons from OpenWeatherMap
- 👥 Amazing contributors and maintainers

## 📧 Contact
For any queries or support, please contact:
* Email: karthicke243@gmail.com
* LinkedIn: [Karthickeien Elangovan](https://www.linkedin.com/in/karthickeien-elangovan/)
* GitHub: [Karthickeien](https://github.com/Karthickeien)

<p align="center">
  <a href="https://github.com/Karthickeien/weather-monitoring-system/issues">
    <img src="https://img.shields.io/badge/Ask%20for-Help-blue?style=for-the-badge&logo=github" alt="Get Help">
  </a>
</p>

---

<p align="center">
  Made with ❤️ by Karthickeien
</p>

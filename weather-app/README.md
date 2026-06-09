# Weather App

A simple React weather app that shows current temperature, humidity, wind speed, and weather icon for a searched city.

## Features

- Search weather by city name
- Displays temperature in Celsius
- Shows humidity and wind speed
- Uses OpenWeatherMap API for live weather data
- Includes animated weather icons for clear, cloud, rain, drizzle, and snow

## Setup

1. Install dependencies:

   ```bash
   npm install
   ```

2. Create a `.env` file in the project root and add your OpenWeatherMap API key:

   ```bash
   REACT_APP_ID=your_openweather_api_key
   ```

3. Start the app:

   ```bash
   npm start
   ```

4. Open the app in your browser:

   ```
   http://localhost:3000
   ```

## Notes

- The app loads weather for `London` by default.
- Enter a city name and click the search icon to fetch new weather data.
- Make sure your OpenWeatherMap API key is valid.

## Available Scripts

In the `weather-app` directory, you can run:

- `npm start` - start development server
- `npm run build` - build for production
- `npm test` - run tests

## Project Structure

- `src/App.js` - main app component
- `src/components/Weather.jsx` - weather search and display UI
- `src/assets/` - weather icon images
- `src/index.js` - app entry point

# Weather Dashboard 🌤️

A beautiful, feature-rich weather dashboard that fetches real-time weather data from the OpenWeatherMap API.

## 🌟 Features

### Current Weather Display
- 🌡️ Real-time temperature and "feels like" temperature
- 📍 Location name with country code
- ☁️ Weather description and conditions
- 📅 Current date and time

### Detailed Weather Metrics
- 💧 Humidity percentage
- 🌬️ Wind speed (km/h)
- 🅿️ Atmospheric pressure (hPa)
- 👁️ Visibility (km)
- ☁️ Cloud coverage percentage
- 🌅 UV Index

### Extended Forecasts
- 📊 5-Day weather forecast
- ⏰ 24-hour hourly forecast with detailed metrics
- 📈 Temperature trends

### Additional Information
- 🌅 Sunrise and sunset times
- 🌡️ Daily max/min temperatures
- 🌧️ Precipitation data (rain & snow)

### User Experience
- 🔍 Search by city name
- 📍 Auto-detect current location
- 📱 Fully responsive design
- ✨ Smooth animations
- 🎨 Modern UI with gradient background

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection

### Installation

1. **Clone or download the files:**
   ```bash
   git clone https://github.com/dashm-sol/traditional-chaddar.git
   cd traditional-chaddar
   ```

2. **Open the weather dashboard:**
   - Open `weather-dashboard.html` in your web browser
   - Or access it from your deployed GitHub Pages site

### API Setup

The dashboard uses the **OpenWeatherMap API** (free tier):

1. **Sign up for free API key:**
   - Visit: https://openweathermap.org/api
   - Create a free account
   - Get your API key from the dashboard

2. **Update API Key:**
   - Open `weather-app.js`
   - Replace the API key on line 5:
   ```javascript
   const API_KEY = 'YOUR_API_KEY_HERE';
   ```

**Note:** A demo API key is included for testing purposes.

## 📁 File Structure

```
weather-dashboard/
├── weather-dashboard.html      # Main HTML file
├── weather-styles.css          # CSS styling
├── weather-app.js              # JavaScript functionality
└── README.md                   # Documentation
```

## 🎨 Features Breakdown

### Search Functionality
- **City Search:** Enter any city name to get weather
- **Location Services:** Click "Use My Location" to auto-detect your coordinates
- **Keyboard Support:** Press Enter to search

### Weather Data
- **Current Weather:** Comprehensive real-time data
- **Forecast:** 5-day and 24-hour hourly forecasts
- **Metrics:** All standard weather measurements

### Responsive Design
- ✅ Desktop (1200px+)
- ✅ Tablet (768px - 1199px)
- ✅ Mobile (Below 768px)

## 🔌 API Endpoints Used

The dashboard uses three OpenWeatherMap endpoints:

1. **Current Weather:**
   ```
   /weather?q={city}&appid={API_KEY}&units=metric
   /weather?lat={lat}&lon={lon}&appid={API_KEY}&units=metric
   ```

2. **Forecast (5-day, 3-hour intervals):**
   ```
   /forecast?lat={lat}&lon={lon}&appid={API_KEY}&units=metric
   ```

3. **UV Index:**
   ```
   /uvi?lat={lat}&lon={lon}&appid={API_KEY}
   ```

## 🎯 How to Use

1. **Search by City:**
   - Type a city name in the search box
   - Click "Search" or press Enter

2. **Use Current Location:**
   - Click the "📍 Use My Location" button
   - Allow browser location access when prompted

3. **View Weather Data:**
   - Current weather conditions
   - Detailed metrics in the grid
   - 5-day forecast cards
   - 24-hour hourly forecast
   - Sunrise/sunset times

## 🛠️ Customization

### Change Temperature Units
To switch from Celsius to Fahrenheit:
- Open `weather-app.js`
- Change `&units=metric` to `&units=imperial`
- Update temperature display in HTML

### Modify Colors
Edit `weather-styles.css`:
```css
--primary-color: #667eea;
--secondary-color: #764ba2;
--accent-color: #ff6b6b;
```

### Add More Features
Possible extensions:
- Multiple city comparison
- Weather alerts and warnings
- Air quality data
- Pollen forecasts
- Save favorite locations

## 🌐 Deployment

### GitHub Pages
1. Push files to your GitHub repository
2. Go to Settings → Pages
3. Select the branch and save
4. Access at: `https://yourusername.github.io/repository-name/weather-dashboard.html`

### Other Platforms
- Netlify
- Vercel
- Firebase Hosting
- Any static hosting service

## 📊 Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- Mobile browsers (iOS Safari, Chrome Mobile)

## ⚠️ Limitations

- Free API tier has rate limits (60 calls/minute)
- Some advanced features require paid API tier
- Accuracy depends on OpenWeatherMap's data

## 🔐 API Key Security

**Important:** The included API key is for demonstration. For production:
1. Create your own API key at openweathermap.org
2. Consider using a backend server to hide the API key
3. Implement rate limiting on your server
4. Never expose API keys in client-side code in production

## 🐛 Troubleshooting

### "City not found" error
- Check spelling
- Try without country code first
- Use city name instead of abbreviation

### "Unable to access location"
- Ensure location services are enabled
- Grant browser permission to access location
- Some browsers require HTTPS for geolocation

### No data displaying
- Check API key is valid
- Verify internet connection
- Check browser console for errors
- Ensure API quota not exceeded

## 📚 Resources

- [OpenWeatherMap API Documentation](https://openweathermap.org/api)
- [Weather Icons](https://openweathermap.org/weather-conditions)
- [Geolocation API](https://developer.mozilla.org/en-US/docs/Web/API/Geolocation_API)

## 📄 License

Free to use and modify.

## 🤝 Contributing

Feel free to fork, modify, and improve!

---

**Created with ❤️ for weather enthusiasts**

Made with HTML5, CSS3, and Vanilla JavaScript

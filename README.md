# ChargeHunt

ChargeHunt is a modern Android app to help electric vehicle (EV) drivers find charging stations near them, powered by OpenChargeMap and OpenStreetMap (osmdroid). Built with Jetpack Compose and Material 3 for a fast, beautiful, and intuitive experience.

## Features

- 🌍 Interactive map (OpenStreetMap/osmdroid) with multi-touch gestures
- 📍 Find charging stations near your current location (with permission)
- 🔍 Manual location search with autocomplete (OpenStreetMap Nominatim)
- ⚡ Filter by fast or slow charging
- 🏷️ Tap markers for station details: name, address, power rating, connection types
- 🧭 One-tap navigation to stations via Google Maps
- 🎨 Modern Material 3 UI, responsive and optimized for performance
- 🛡️ Robust error handling and onboarding guidance
- 📦 Production-ready APK builds

## Getting Started

### Prerequisites

- Android Studio (Giraffe or newer recommended)
- Android SDK 24+
- Java 17+ (set `JAVA_HOME` accordingly)
- Internet connection and location services enabled on device/emulator

### Setup

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/chargehunt.git
   cd chargehunt
   ```

2. **Open in Android Studio.**

3. **Configure API keys:**
   - The app uses OpenChargeMap and OpenStreetMap APIs. For production, add your OpenChargeMap API key to `local.properties`:
     ```
     OPENCHARGEMAP_API_KEY=your_api_key_here
     ```
   - For testing, a fallback key is used.

4. **Build and run:**
   - Use the "Run" button in Android Studio, or build a release APK with:
     ```sh
     ./gradlew assembleRelease
     ```

### Permissions

- Location: To show nearby charging stations
- Internet: For map and API access

## Usage

1. Launch the app.
2. Tap **Show My Location** to load the map and find stations near you.
3. Use the search bar to find stations in other locations (autocomplete supported).
4. Filter results by fast/slow charging.
5. Tap a station marker for details and navigation.

## Tech Stack

- Kotlin, Jetpack Compose, Material 3
- osmdroid (OpenStreetMap)
- Retrofit (networking)
- OpenChargeMap API
- Nominatim (OpenStreetMap geocoding)
- Google Play Services (location)
- AdMob (optional, for ads)

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to change.

## License

[MIT](LICENSE)

## Credits

- [OpenChargeMap](https://openchargemap.org/)
- [OpenStreetMap](https://www.openstreetmap.org/)
- [osmdroid](https://github.com/osmdroid/osmdroid)

# FitBasic - Complete React Native Fitness App

A production-ready React Native fitness application built with Expo, featuring workout routines, diet plans, exercise library, and multi-language support with RTL capabilities.

## Features

### Core Fitness Features
- **Workouts** - Browse, search, and track workout routines with detailed instructions
- **Exercises** - Comprehensive exercise library with equipment and muscle group filtering
- **Diets** - Customizable nutrition plans with calorie and serving information
- **Workout Timer** - Built-in exercise timer with keep-awake functionality
- **Custom Workouts & Diets** - Create personalized routines and meal plans
- **Progress Tracking** - Track completed workouts and favorites

### Additional Features
- **Blog/Posts** - Fitness articles and educational content
- **Products/Store** - Fitness product recommendations
- **Equipment Library** - Browse exercises by equipment type

### User Features
- **Firebase Authentication** - Email/password login with email verification
- **User Profiles** - Profile management with profile pictures
- **Settings** - Theme and language preferences
- **Dark/Light Mode** - Full theme support

### Internationalization
- **English** (Default)
- **Spanish**
- **Arabic** (with full RTL support)

## Tech Stack

| Category | Technologies |
|----------|-------------|
| Framework | React Native 0.73.4, Expo 50.0.0 |
| Navigation | React Navigation 6 (Stack, Drawer, Tabs) |
| UI Components | React Native Paper 5.12.3 |
| State Management | React Context API, AsyncStorage |
| Authentication | Firebase 9.15.0 |
| Animations | React Native Reanimated, Animatable |
| Push Notifications | OneSignal |
| Ads | Google AdMob |

## Project Structure

```
app/
├── src/
│   ├── screens/          # 43 screen components
│   ├── components/       # 35 reusable UI components
│   ├── navigation/       # Navigation configuration
│   ├── context/          # Theme context provider
│   ├── languages/        # i18n translations (en, es, ar)
│   ├── hooks/            # Custom React hooks
│   ├── config/           # App configuration
│   └── assets/           # Images and icons
├── assets/               # App icons and splash screens
├── App.js                # Root component
├── app.json              # Expo configuration
└── package.json          # Dependencies
```

## Prerequisites

- Node.js (v16 or higher recommended)
- npm or yarn
- Expo CLI (`npm install -g expo-cli`)
- iOS Simulator (Mac only) or Android Emulator
- Physical device with Expo Go app (optional)

## Installation

1. **Clone the repository**
   ```bash
   git clone git@github.com:say2alihassan/fintessBasicapp.git
   cd fintessBasicapp
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure Firebase** (Optional - for authentication)

   Update the Firebase configuration in `src/config/ConfigFirebase.js` with your credentials:
   ```javascript
   const firebaseConfig = {
     apiKey: "YOUR_API_KEY",
     authDomain: "YOUR_AUTH_DOMAIN",
     projectId: "YOUR_PROJECT_ID",
     storageBucket: "YOUR_STORAGE_BUCKET",
     messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
     appId: "YOUR_APP_ID"
   };
   ```

4. **Configure App Settings** (Optional)

   Update `src/config/ConfigApp.js` for:
   - Backend API URL
   - AdMob IDs
   - OneSignal App ID
   - Default language and theme

## Running the App

```bash
# Start Expo development server
npm start

# Run on Android
npm run android

# Run on iOS
npm run ios

# Run on web
npm run web
```

## Configuration

### ConfigApp.js Options

| Setting | Description |
|---------|-------------|
| `URL` | Backend API endpoint |
| `DEFAULTLANG` | Default language (en, es, ar) |
| `THEMEMODE` | Default theme (light, dark) |
| `SHOWADS` | Enable/disable advertisements |
| `ANDROID_BANNER_ID` | AdMob Android banner unit ID |
| `IOS_BANNER_ID` | AdMob iOS banner unit ID |
| `ONESIGNAL_APP_ID` | OneSignal push notification app ID |

## Building for Production

This project uses Expo Application Services (EAS) for builds:

```bash
# Install EAS CLI
npm install -g eas-cli

# Login to Expo
eas login

# Build for Android
eas build --platform android

# Build for iOS
eas build --platform ios
```

## Key Dependencies

```json
{
  "expo": "^50.0.0",
  "react": "18.2.0",
  "react-native": "0.73.4",
  "react-native-paper": "^5.12.3",
  "@react-navigation/native": "^6.1.1",
  "firebase": "^9.15.0",
  "react-native-reanimated": "~3.6.2",
  "react-native-google-mobile-ads": "^12.10.0",
  "react-native-onesignal": "4.5.0"
}
```

## Screenshots

The app includes:
- Home dashboard with latest workouts and diets
- Workout browsing with goal and level filtering
- Exercise library with equipment categories
- Diet plans with nutritional information
- User profile and settings
- Dark and light theme modes

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the terms included with the CodeCanyon purchase.

## Support

For support and questions, please open an issue in this repository.

---

**Version:** 1.0.0
**Package:** com.wicombit.fitbasic

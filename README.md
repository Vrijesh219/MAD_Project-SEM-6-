#  Event Management App

A Flutter mobile application for managing events like Birthday Parties, Wedding Ceremonies, and Night Parties. The app features Google/Facebook authentication, cloud storage with Firebase, local storage with Hive, and a beautiful Material Design UI.

## Features

- 🔐 Authentication
  - Google Sign-In
  - Secure user data management

- 📅 Event Management
  - Create, Read, Update, Delete events
  - Categorize events (Birthday, Wedding, Night Party, etc.)
  - Set event date, time, and location
  - View event details and history

- 💾 Data Storage
  - Cloud storage with Firebase Firestore
  - Local storage with Hive for offline access
  - Real-time data synchronization

- 🎨 UI/UX
  - Material Design
  - Responsive layout
  - Smooth animations
  - User-friendly interface

## Getting Started

### Prerequisites

- Flutter SDK (3.0.0 or higher)
- Dart SDK (3.0.0 or higher)
- Android Studio / VS Code
- Firebase account
- Google Cloud Platform account
- Facebook Developer account

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/event_app.git
   cd event_app
   ```

2. Install dependencies:
   ```bash
   flutter pub get
   ```

3. Configure Firebase:
   - Create a new Firebase project
   - Add Android and iOS apps to your Firebase project
   - Download and add the configuration files:
     - Android: `google-services.json` to `android/app`
     - iOS: `GoogleService-Info.plist` to `ios/Runner`

4. Configure Google Sign-In:
   - Enable Google Sign-In in Firebase Authentication
   - Configure OAuth consent screen
   - Add SHA-1 and SHA-256 fingerprints

5. Configure Facebook Sign-In:
   - Create a Facebook app in Facebook Developers Console
   - Enable Facebook Login
   - Add your app's OAuth redirect URL
   - Configure Facebook app ID in Firebase

6. Run the app:
   ```bash
   flutter run
   ```

## Project Structure

```
lib/
  ├── core/
  │   ├── app_constants.dart
  │   └── firebase_options.dart
  ├── features/
  │   ├── auth/
  │   │   ├── login_screen.dart
  │   │   └── auth_service.dart
  │   ├── events/
  │   │   ├── event_model.dart
  │   │   ├── event_provider.dart
  │   │   ├── event_list_screen.dart
  │   │   ├── add_event_screen.dart
  │   │   └── event_detail_screen.dart
  │   └── profile/
  │       └── profile_screen.dart
  ├── services/
  │   ├── api_service.dart
  │   ├── local_storage_service.dart
  │   └── cloud_firestore_service.dart
  ├── widgets/
  │   ├── custom_button.dart
  │   └── event_card.dart
  └── main.dart
```

## Testing

Run tests using:
```bash
flutter test
```

The project includes:
- Unit tests for models and services
- Widget tests for UI components
- Integration tests for main flows

## State Management

The app uses Provider for state management:
- AuthService for authentication state
- EventProvider for event data management
- Local and cloud data synchronization

## Dependencies

Main packages used:
- `firebase_core`: ^2.24.2
- `firebase_auth`: ^4.15.3
- `cloud_firestore`: ^4.13.6
- `google_sign_in`: ^6.1.6
- `flutter_facebook_auth`: ^5.0.10
- `provider`: ^6.1.1
- `hive`: ^2.2.3
- `hive_flutter`: ^1.1.0
- `go_router`: ^13.0.0
- `google_fonts`: ^6.1.0
- `cached_network_image`: ^3.3.0



## Acknowledgments

- Flutter team for the amazing framework
- Firebase team for the backend services
- All contributors and package maintainers






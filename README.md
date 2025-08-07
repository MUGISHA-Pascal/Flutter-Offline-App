# Flutter Offline Task App

A modern Flutter application for task management with offline-first capabilities. Built with BLoC pattern for state management and SQLite for local data persistence.

## Features

- **Offline-First Design**: Works seamlessly without internet connection
- **Task Management**: Create, edit, delete, and organize tasks
- **User Authentication**: Secure signup and login system
- **Local Data Storage**: SQLite database for persistent data
- **Modern UI**: Clean, responsive design with Material 3
- **State Management**: BLoC pattern for predictable state management
- **Connectivity Monitoring**: Real-time network status detection

## Technology Stack

- **Framework**: Flutter 3.8+
- **State Management**: flutter_bloc
- **Database**: SQLite (sqflite)
- **HTTP Client**: http package
- **Local Storage**: shared_preferences
- **Connectivity**: connectivity_plus
- **UI Components**: Material Design 3
- **Custom Fonts**: Cera Pro

## Getting Started

### Prerequisites

- Flutter SDK (3.8.1 or higher)
- Dart SDK
- Android Studio / VS Code
- Android SDK (for Android development)
- Xcode (for iOS development, macOS only)

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd flutter_offline_app
   ```

2. Install dependencies:
   ```bash
   flutter pub get
   ```

3. Run the app:
   ```bash
   flutter run
   ```

### Building for Production

**Android:**
```bash
flutter build apk --release
```

**iOS:**
```bash
flutter build ios --release
```

**Web:**
```bash
flutter build web --release
```

## Project Structure

```
lib/
├── core/           # Core utilities and constants
├── features/       # Feature-based modules
│   ├── auth/       # Authentication feature
│   └── home/       # Task management feature
├── models/         # Data models
└── main.dart       # App entry point
```

## Architecture

This app follows a feature-based architecture with BLoC pattern:

- **Features**: Each feature is self-contained with its own pages, cubits, and models
- **BLoC Pattern**: Uses Cubit for state management within each feature
- **Repository Pattern**: Data access layer for local and remote operations
- **Offline-First**: Prioritizes local data with sync capabilities when online

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support and questions, please open an issue in the repository.

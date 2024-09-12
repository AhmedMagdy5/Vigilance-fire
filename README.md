# Vigilance-fire
Vigilance Fire - Flutter App

This repository contains the Flutter mobile app for the Vigilance Fire System. The app enables real-time monitoring and control of fire-related incidents using **AI detection and a user management system. It also provides alert notifications, emergency AR navigation, and admin functionalities for managing users and controlling gas flow in case of emergencies.

---

 Features Implemented
- Sign-In Screen: 
  - Login for both admin and employees using Firebase authentication.
  
 Dashboard:
  - Admin dashboard shows key information like gas quantity and temperature.
  - Users see a simplified version with alerts.
  
 Alert Notifications:
  - Users and admins receive notifications when fire incidents are detected.

 User Management (Admin only):
  - Admins can add and manage employees through unique ID assignments.
  
 AR Navigation:
  - Allows users to view emergency exits using the camera via AR functionality.


 Code Details

 Key Screens and Widgets
- alertnotify_screen.dart: Handles notifications for fire alerts. It uses a simple Scaffold layout to display the alert.
  
  dart
  import 'package:flutter/material.dart';
  
  class AlertNotifyScreen extends StatelessWidget {
    const AlertNotifyScreen({super.key});
  
    @override
    Widget build(BuildContext context) {
      return Scaffold(
        // Alert notification UI will go here
      );
    }
  }
  

- dashboard_screen.dart: This screen displays gas quantity, temperature, and fire status. It uses a real-time data feed to keep the admin updated on critical values.

user_provider.dart and admin_provider.dart: These files manage the business logic for user and admin functionality, respectively. They handle tasks like adding new users, updating user data, and managing permissions.

---

 File Structure

plaintext
lib/
├── providers/
│   ├── admin_provider.dart
│   ├── user_provider.dart
├── screens/
│   ├── alertnotify_screen.dart  // Notifications for fire alerts
│   ├── dashboard_screen.dart    // Dashboard for displaying sensor data
│   ├── sign_screen.dart         // Sign-in for both admin and users
│   ├── ar_screen.dart           // AR-based emergency exit routes
│   └── profile_screen.dart      // User and admin profile management
└── widgets/
    └── main.dart                // Main entry point for the app



 Getting Started

 Prerequisites
 Flutter SDK
 Dart
 Firebase for authentication and real-time database

 Installation

1. Clone the repository:
   bash
   git clone https://github.com/youssefzamzam/Vigilance-fire.git
   
2. Navigate into the project directory:
   bash
   cd Vigilance-fire
   
3. Install dependencies:
   bash
   flutter pub get
   
4. Run the app on an emulator or real device:
   bash
   flutter run
   

 Future Features
 Integration of AI Detection Model: In future updates, the app will integrate the AI model for real-time fire detection.
 Enhanced AR Navigation: Improving the AR capabilities for better emergency navigation.
 Admin Dashboard Enhancements: Adding more detailed control options for gas shutdown and system status.
 Contributing
1. Fork this repository.
2. Create your feature branch: git checkout -b feature-branch.
3. Commit your changes: git commit -m 'Add feature'.
4. Push to the branch: git push origin feature-branch.
5. Open a pull request.
 Contact
- *Flutter developer *: Youssef zamzam & Ahmed magdy 
  GitHub: [youssefzamzam](https://github.com/youssefzamzam)

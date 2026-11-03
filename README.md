# Spendwise-
Calculate daily expenses 
SpendWise – Expense Tracker

Project Name

SpendWise – Expense Tracker

Project Description

SpendWise is a Flutter mobile application that helps users manage their daily expenses. Users can add, view, edit, and delete expenses, organize them by category, and view a category-wise spending summary.

The application stores expense data locally on the device so that records remain available after restarting the app.

Main Features

- Add expenses with name, amount, category, date, and optional note
- Validate user input before saving
- View all expenses
- View detailed information about an expense
- Edit and delete expenses
- View total expenses
- View category-wise spending summary
- Save data locally using SharedPreferences
- Use Provider for shared application state

Technologies Used

- Flutter
- Dart
- Provider
- SharedPreferences
- Intl
- Android

Data Source

User-created expense records stored locally on the device using SharedPreferences. No internet connection is required for core expense tracking.

Screenshots

Add three screenshots of the application here:

1. Home / Expense List Screen
2. Add Expense Screen
3. Category Summary Screen

How to Run the Project

1. Install Flutter and Android Studio.

2. Clone this repository.

3. Open the project folder in your IDE.

4. Run:
   
   flutter pub get

5. Connect an Android device or start an emulator.

6. Run:
   
   flutter run

Testing

Run the widget tests:

flutter test

Team Members and Responsibilities

Team Member| Responsibility
Member 1| Add/Edit Expense Form
Member 2| Expense List and Details
Member 3| Category Summary, Testing, and Documentation

Update this table with the actual team members and contributions.

Release APK

The release APK can be generated using:

flutter build apk --release

APK location:

build/app/outputs/flutter-apk/app-release.apk
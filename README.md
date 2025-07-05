# Smart Plant Management App

This Android application is designed to work with a custom-built device that automatically plants and waters plants. It connects via Bluetooth to an Arduino microcontroller, which controls two stepper motors (each using a different driver). The system provides an intuitive interface for managing plants and interacting with the physical device. To activate the Arduino code, the app sends the command START Smart Plant Management App via Bluetooth once the connection is established

## Features

- Bluetooth Communication  
  Connects to an Arduino via Bluetooth (e.g., HC-05 module) for real-time control of planting and watering mechanisms.

- Plant Management  
  Add new plants with custom images using the `dodanie_rosliny` activity.

- Shelf View  
  Organizes plants visually in a shelf-like layout (`ShelfActivity`).

- Progress Tracking  
  Monitor actions like planting and watering via `ProgressActivity`.

- Custom Adapter  
  Dynamically displays plant data in the app using `PlantAdapter`.

## Technologies Used

- Platform: Android (Java)  
- Build Tool: Gradle (Kotlin DSL)  
- Bluetooth: Serial communication with Arduino  
- Hardware: Arduino + 2 stepper motors + different drivers (e.g., A4988, DRV8825)

Modules:
- `MainActivity.java` – main menu/navigation
- `dodanie_rosliny.java` – add new plants
- `ShelfActivity.java` – display plants
- `ProgressActivity.java` – show progress
- `Rosliny.java` – plant model
- `PlantAdapter.java` – data binding for plant lists

## How It Works

1. Pair your phone with the Bluetooth module (e.g., HC-05) connected to Arduino.  
2. Open the app, add plants and assign images.  
3. Send commands via Bluetooth to the Arduino to start planting or watering.  
4. Track progress visually in the app.

## Hardware Requirements

- Arduino Uno/Nano  
- 2x Stepper motors (with different drivers)  
- Bluetooth module (e.g., HC-05)  
- Watering and planting mechanical system (custom-built)

## Future Improvements

- Creating same app but for IOS
- Wi-Fi/cloud support for remote access

![Main Menu](https://github.com/user-attachments/assets/015ceb11-860c-4ab5-872f-6e09d5dd3987)


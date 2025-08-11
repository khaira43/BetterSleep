# BetterRest

BetterRest is a SwiftUI iOS app that helps users determine their optimal bedtime based on desired wake-up time, amount of sleep, and daily coffee intake.  
It uses Core ML's `SleepCalculator` model to provide a personalized sleep schedule.

---

## Features

- **Wake-Up Time Selection** — Pick the time you want to wake up using a `DatePicker`.
- **Desired Sleep Duration** — Select desired sleep time in quarter-hour increments using a `Stepper`.
- **Daily Coffee Intake** — Enter your daily coffee consumption with a `Stepper`.
- **Machine Learning Prediction** — Uses Core ML to predict optimal bedtime.
- **Simple UI** — Built entirely with SwiftUI for a clean and minimal design.

---

## Technologies Used

- **SwiftUI** — Declarative UI framework for iOS.
- **Core ML** — Machine learning framework for sleep prediction.
- **SleepCalculator.mlmodel** — Pre-trained model for estimating ideal bedtime.

---

## How It Works

1. User selects:
   - Wake-up time
   - Desired amount of sleep
   - Daily coffee intake
2. The app sends this data to the `SleepCalculator` model.
3. The model predicts the amount of sleep needed.
4. The app subtracts that from the wake-up time to determine the ideal bedtime.
5. The result is displayed in an alert.

---

## Example

If you:
- Wake up at **7:00 AM**
- Want **8 hours** of sleep
- Drink **2 cups** of coffee a day

The app might tell you to go to bed at **10:45 PM** for optimal rest.

---

## Requirements

- iOS 17.0+
- Xcode 15+
- Swift 5.9+
- Core ML enabled in the project

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/BetterRest.git
   ```
2. Open `BetterRest.xcodeproj` in Xcode.
3. Ensure `SleepCalculator.mlmodel` is included in the project.
4. Run the app on a simulator or physical device.

---

## License

This project is open source and available under the [MIT License](LICENSE).

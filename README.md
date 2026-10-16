# Android Activity & Intent Demo

A simple, clean Android application built in Java to demonstrate core Android fundamentals, including Activity lifecycle navigation, layout design, button click listeners, and Explicit Intents.

---

## 📌 Features
- **Main Activity Screen**: Features a clean UI with a heading and a button to launch the secondary screen.
- **Second Activity Screen**: Opens seamlessly upon button click, showing a confirmation/welcome screen.
- **Explicit Intent Implementation**: Demonstrates how to pass context and trigger navigation between Android activities.

---

## 🛠️ Tech Stack & Requirements
- **Language**: Java
- **IDE**: Android Studio (Jellyfish / Koala or newer)
- **Min SDK**: API 24 (Android 7.0)
- **Target SDK**: API 34 (Android 14)
- **UI Design**: XML (`ConstraintLayout`)

---

## 🚀 How to Run the App

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/dulanachathurma/Android-Activity-Intent-Demo.git
   ```

2. **Open in Android Studio**:
   - Open Android Studio.
   - Click **File > Open...** and select the cloned project folder.

3. **Build & Sync**:
   - Wait for Gradle sync to complete successfully.

4. **Run on Emulator / Device**:
   - Select an emulator (e.g., Pixel 6 API 34) or connect a physical device via USB Debugging.
   - Click the green **Run (▶)** button or press `Shift + F10`.

---

## 💡 Code Explanation

### 1. Handling Button Clicks
The `OnClickListener` interface listens for user interactions on the button control:

```java
Button btnSecond = findViewById(R.id.btnSecondActivity);
btnSecond.setOnClickListener(new View.OnClickListener() {
    @Override
    public void onClick(View v) {
        // Navigation logic triggered here
    }
});
```

### 2. Navigating with Explicit Intent
An **Explicit Intent** specifies the exact target activity class to be started:

```java
Intent intent = new Intent(MainActivity.this, SecondActivity.class);
startActivity(intent);
```

- **`MainActivity.this`**: Provides the current activity context.
- **`SecondActivity.class`**: Specifies the target Activity component to launch.

---

## 👨‍💻 Author
- **Developer**: Dulana Chathurma
- **GitHub**: [@dulanachathurma](https://github.com/dulanachathurma)
- **Repository**: [Android-Activity-Intent-Demo](https://github.com/dulanachathurma/Android-Activity-Intent-Demo)
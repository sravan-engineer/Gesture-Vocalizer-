# Gesture Vocalizer for Deaf and Mute People 🤟🔊

An Arduino-based embedded system that converts hand gestures into text and voice messages, helping deaf and mute individuals communicate more easily with people unfamiliar with sign language.

## 📽️ Demo

> Add your video link here after uploading (see "Adding the Demo Video" section below).

```
[Demo Video](https://github.com/sravan-engineer/Gesture-Vocalizer-/blob/main/prototype%20of%20gesture%20vocalizer.mp)
```

## 📌 Problem Statement

Many deaf and mute individuals rely on sign language for communication. Since most people do not understand sign language, communication becomes difficult in hospitals, schools, and public places. This project helps bridge that communication gap by converting hand gestures into understandable text and voice output.

## ⚙️ Working Principle

1. Flex sensors mounted on a glove detect finger bending.
2. The resistance change from bending is converted into voltage signals.
3. An Arduino Uno reads and processes these sensor values.
4. The system compares the values against predefined gesture patterns.
5. The corresponding message is displayed on an LCD and/or spoken aloud.

## 🧩 Components Used

| Component | Purpose |
|---|---|
| Arduino Uno | Main controller for processing sensor data |
| Flex Sensors | Detect finger bending and gestures |
| 16x2 LCD Display (I2C) | Displays output messages |
| HC-05 Bluetooth Module | Wireless communication |
| Resistors | Used in voltage divider circuit |
| Battery | Power supply |
| Glove | Mounting platform for sensors |

**Estimated Budget:** ₹2500 – ₹3000

## ✅ Advantages

- Helps deaf and mute people communicate easily
- Low cost and easy to implement
- Portable and user-friendly
- Can be extended using AI-based gesture recognition

## 💻 Source Code

The Arduino sketch is available in [`gesture_vocalizer.ino`](./gesture_vocalizer.ino). It initializes a 16x2 I2C LCD and defines the set of predefined gesture messages:

```
WASHROOM, DRINK WATER, FOOD, FRUIT, THANK YOU, HELP, SORRY, YES, NO, PLEASE, WAIT, GOOD MORNING
```

Flex sensor reading and gesture-matching logic can be added inside the `loop()` function to map live sensor values to these messages.

## 📁 Repository Structure

```
gesture-vocalizer-arduino/
├── README.md
├── gesture_vocalizer.ino
├── Embedded_Systems_Report.pdf
└── demo/
    └── prototype_demo.mp4   (or a link to hosted video, see below)
```

## 🚀 Future Scope

- AI/ML-based gesture recognition for higher accuracy
- Larger gesture vocabulary
- Mobile app integration via Bluetooth
- Text-to-speech improvements for natural voice output

## 📄 Full Report

See [`Embedded_Systems_Report.pdf`](./Embedded_Systems_Report.pdf) for the complete project report, including the introduction to embedded systems and detailed methodology.

## 👤 Author

Add your name, college/institution, and contact/social links here.

## 📜 License

Add a license of your choice (e.g., MIT) — see [choosealicense.com](https://choosealicense.com/) if unsure.


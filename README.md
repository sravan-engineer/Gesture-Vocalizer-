# Gesture-Vocalizer-
Gesture Vocalizer for Deaf and Mute People using Arduino:
#include <Wire.h>
#include <LiquidCrystal_I2C.h>

// Set the I2C address of your LCD (0x27 or 0x3F)
LiquidCrystal_I2C lcd(0x27, 16, 2);

// List of messages to display (add or remove as you like)
const char* messages[] = {
  "WASHROOM",
  "DRINK WATER",
  "FOOD",
  "FRUIT",
  "THANK YOU",
  "HELP",
  "SORRY",
  "YES",
  "NO",
  "PLEASE",
  "WAIT",
  "GOOD MORNING"
};
const int numMessages = sizeof(messages) / sizeof(messages[0]);

String lastMsg = "";

void setup() {
  Serial.begin(9600);
  lcd.init();
  lcd.backlight();
  lcd.print("SIGN LANGUAGE");
  delay(2000);
  lcd.clear();
  randomSeed(analogRead(A0));  // Randomize based on an unused analog pin
}

void loop() {
  // Pick a random message
  int index = random(numMessages);
  String currentMsg = messages[index];
  
  // Update LCD only if the message changed
  if (currentMsg != lastMsg) {
    lcd.clear();
    lcd.setCursor(0, 0);
    lcd.print("SIGN LANGUAGE");
    lcd.setCursor(0, 1);
    lcd.print(currentMsg);
    Serial.println("Display: " + currentMsg);
    lastMsg = currentMsg;
  }
  
  // Random delay between 150ms and 2000ms
  int delayTime = random(150, 2000);
  delay(delayTime);
}

/*
  Arduino Lm35 LCD Termometre
  Tarih:28.08.2017
  Can KILIÇ
*/

#include <LiquidCrystal.h>
LiquidCrystal lcd(12, 11, 5, 4, 3, 2);
int sicaklik = 0;
const int sicaklik_pin = A0;

void setup() {
  lcd.begin(16, 2);
}

void loop() {
  lcd.clear();
  sicaklik = analogRead(sicaklik_pin);
  sicaklik = sicaklik * 0.48828125;
  lcd.print("Sicaklik: ");
  lcd.print(sicaklik);
  lcd.print("\337C");
  lcd.setCursor(2, 1);
  lcd.print("-Can KILIC-");
  delay(1000);
}

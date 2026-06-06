int ledPins[] = {2, 4, 5, 18, 19}; 
int total = 5;

void setup() {
  for (int i = 0; i < total; i++) {
    pinMode(ledPins[i], OUTPUT);
    digitalWrite(ledPins[i], LOW); 
  }
}

void loop() {
  for (int i = 0; i < total; i++) {
    digitalWrite(ledPins[i], HIGH);
    delay(1000);
    digitalWrite(ledPins[i], LOW);
  }
}

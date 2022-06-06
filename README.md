# Practica1: BLINK

En aquesta pràctica utilitzarem l'assignació i utilització de pins, les sortides pel terminal, el setup i el loop.

# codi
```
#include <Arduino.h>
//pin del LED
#define PIN 14
//set up
void setup() {
  Serial.begin(115200);
  pinMode(PIN, OUTPUT);
}
//loop
void loop() {

  digitalWrite(PIN, HIGH);
  Serial.println("ON");
  delay(500);
  digitalWrite(PIN, LOW);
  Serial.println("OFF");
  delay(500);
}
```
# Explicació del codi

Primer assignem la llibreria Arduino (necessaria per a poder operar amb arduino) i definirem el pin que utilitzarem pel led:

```
#include <Arduino.h>
//pin del LED
#define PIN 14
```
**Set up:**

```
void setup() {
  Serial.begin(115200);
  pinMode(PIN, OUTPUT);
}
```

**Loop:**

```
void loop() {
  digitalWrite(PIN, HIGH);
  Serial.println("ON");
  delay(500);
  digitalWrite(PIN, LOW);
  Serial.println("OFF");
  delay(500);
}
```


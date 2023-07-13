int switchState = 0;

void setup() {
  //assign pins to their desired mode of input or output
  pinMode(3, OUTPUT);
  pinMode(4, OUTPUT);
  pinMode(5, OUTPUT);
  pinMode(2, INPUT);
}

void loop() {
  //assign switchState variable to voltage reading is coming from pin 2
  //result will be 0 (low/off/no voltage) or 1 (high/on/voltage)
  switchState = digitalRead(2);

  //if the switch is not pressed
  if (switchState == LOW) {
    //turn the green LED on
    digitalWrite(3, HIGH);
    //turn the red LEDs off
    digitalWrite(4, LOW);
    digitalWrite(5, LOW);
  } else {
    //otherwise
    //turn the green LED off
    digitalWrite(3, LOW);
    //turn the red 4 LED off
    digitalWrite(4, LOW);
    //turn the red 5 LED on
    digitalWrite(5, HIGH);

    //pause for quarter second
    delay(100);

    //toggle red LEDs
    digitalWrite(4, HIGH);
    digitalWrite(5, LOW);

    //pause for quarter second
    delay(100);
  }
}


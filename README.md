Byte IOT Submission Task
this is a simple Arduino-based project that demonstrates how to control an RGB LED with a push button. The project follows a specific sequence for the LED colors as the button is pressed.
The circuit consists of:

  RGB LED: Three colors (Red, Green, and Blue) are controlled via code.
  Push Button: A button is used to change the state of the LED.

LED Sequence

  Initial State (Circuit On):
        Red light: ON
        Green light: OFF
        Blue light: OFF

   First Button Press:
        Red light: OFF
        Green light: ON
        Blue light: OFF

   Second Button Press:
        Red light: OFF
        Green light: OFF
        Blue light: ON


CODE SNIPPET USED:
const int ledPin = 9; // Define the pin for the LED

void setup() {
    pinMode(ledPin, OUTPUT); // Set the LED pin as an output
}

void loop() {
    digitalWrite(ledPin, HIGH); // Turn on the LED
    delay(1000); // Wait for 1 second
    digitalWrite(ledPin, LOW); // Turn off the LED
    delay(1000); // Wait for 1 second
}

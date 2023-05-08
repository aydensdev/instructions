# Servo Pointing at LED Tutorial #

1) Make sure you are using Arduino IDE 2.1.0 https://www.arduino.cc/en/software

2) Open the IDE which should automatically create a new sketch. `File > Save As` to a folder of your choice.

3) Go back to the IDE and open the library manager on your left. Find and install the Servo Library.

![figure1](https://user-images.githubusercontent.com/68286181/236929744-24fbd8a1-f2dd-4a80-8c70-69455d4d679a.png)

4) Import the servo library with the following code:

```cpp
#include <Servo.h> 

#define SERVO_PIN 4 // <= REPLACE WITH THE PIN # YOU CONNECTED THE YELLOW WIRE TO
Servo myServo;

void setup() {
  myServo.attach(SERVO_PIN)
}

int targetAngle = 0; 

// change the target angle until it points to the led
// then set this to that angle
int angleToLED = -1; 

void loop() {
  targetAngle = 90; // CHANGE THIS ANGLE TO MAKE THE SERVO TURN
  
  if ( targetAngle = angleToLED ) {
    /* turn on the LED here im not giving you a tutorial on that */
  }

  s1.write(targetAngle); 
}
```

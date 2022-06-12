# FIRST-CLASS

## TOPIC
- LED blink
### CONTENTS
- VCC, VDD, and 5V mean the same thing. So the red line is used for 5V, vcc, vdd
- the black line is used for GND.
- LED's longer led: ANODE(positive), LED's shorter leg: CATHODE(negative)
![image](https://user-images.githubusercontent.com/102523600/173241461-b521b81c-461b-446f-a09d-ccd35dd4d0b4.png)
- blue line: CATHODE(negative)
- red line: ANODE(positive)
- green line: Depends on the line where the pin is held
![image](https://user-images.githubusercontent.com/102523600/173241719-9aad257a-0d9b-4c8d-aa08-a6cc272b2d37.png)
- LED's longer led: Resistance 330 ohms to one side
- Resistance 330 ohms: connect to digital pin number 13
- LED's shorter leg: connect to GND
### CODE
1. int LED=13; // the setup function runs once when you press reset or power the board
2. void setup() {
3. pinMode(LED_BUILTIN, OUTPUT); // initialize digital pin LED_BUILTIN as an output.
4. }
5. // void loop means that function runs over and over again forever
6. void loop() {
7. digitalWrite(LED_BUILTIN, HIGH);  // turn the LED on (HIGH is the voltage level)
8. delay(1000);                       // wait for a second(1000 mMillisecond)
9. digitalWrite(LED_BUILTIN, LOW);   // turn the LED off by making the voltage LOW
10. delay(1000);                       // wait for a second
11. }

# Robotics_Notes

Analog Input Homework Assignment

For this project I had difficulties with just about everything. I am unable to complete the homework due to the LDR not working and I am not sure why. From this project I have learned that when connected to the 5V on the arduino it goes on the positive side of the breadboard and the GND goes on the negative. I also learned that the A0 chord, LDR, and resistor all have to be on the same row. 
When I first started this I had difficulties putting everything together because I didn't understand where anything went. Because I cannot get this part of the homework to work I do not believe I am able to continue and will have to ask for help tomorrow.

for the sensor value I cannot put the code in to test it out but I think in the void loop section I would add:

analogValue = analogRead(0);

  // print it out in many formats:
  Serial.println(analogValue);       // print as an ASCII-encoded decimal
  Serial.println(analogValue, DEC);  // print as an ASCII-encoded decimal
  Serial.println(analogValue, HEX);  // print as an ASCII-encoded hexadecimal
  Serial.println(analogValue, OCT);  // print as an ASCII-encoded octal
  Serial.println(analogValue, BIN);  // print as an ASCII-encoded binary

  // delay 10 milliseconds before the next reading:
  delay(10);
  
  For creating the light I would use:
  
   if (brightness <= 499) {
    brightness = 0 ;
  }
  
  For the second part:
  
   if (brightness >= 700) {
    brightness = 300
} else if (brightness <= 300 || brightness >= 700) {
  fadeAmount = -fadeAmount;
}
  
  http://s1136.photobucket.com/user/audreen890/media/IMG_3993.jpg.html
  

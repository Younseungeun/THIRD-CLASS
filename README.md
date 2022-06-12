# THIRD-CLASS

## TOPIC
- LCD monitor
- CDS sensor
### LCD monitor

### CODE
1. 1#include <Wire.h> 
2. #include <LiquidCrystal_I2C.h>     // header file, we can use header files by downloading it 
3. LiquidCrystal_I2C lcd(0x27,16,2);  // set the LCD address to 0x27 for a 16 chars and 2 line display
4.                                   // "0x27" means the address of LCD
5.void setup(){
6.lcd.init();                      // initialize the lcd
7.                                   // Print a message to the LCD.
8. lcd.backlight();
9. lcd.setCursor(0,0);                // first line of the LCD
10. lcd.print("Hello,Every one!");    // print "Hello,Every one!" in LCD display
11. lcd.setCursor(0,1);               // second line of the LCD
12. lcd.print("Welcome Reader!");     // print "Welcome Reader!" in LCD display
13. }
14. void loop(){}

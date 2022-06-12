# THIRD-CLASS

## TOPIC
- LCD monitor
- CDS sensor
### LCD monitor
![image](https://user-images.githubusercontent.com/102523600/173245391-e4419cd9-b084-4c01-a4da-8770d9f2fbe3.png)
### CODE
1. 1#include <Wire.h> 
2. #include <LiquidCrystal_I2C.h>     // header file, we can use header files by downloading it 
3. LiquidCrystal_I2C lcd(0x27,16,2);  // set the LCD address to 0x27 for a 16 chars and 2 line display, "0x27" means the address of LCD
4. void setup(){
5. lcd.init();                      // initialize the lcd, Print a message to the LCD.
6. lcd.backlight();
7. lcd.setCursor(0,0);                // first line of the LCD
8. lcd.print("Hello,Every one!");    // print "Hello,Every one!" in LCD display
9. lcd.setCursor(0,1);               // second line of the LCD
10. lcd.print("Welcome Reader!");     // print "Welcome Reader!" in LCD display
11. }
12. void loop(){}
### CDS sensor
### CODE

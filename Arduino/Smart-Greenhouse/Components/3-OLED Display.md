### SSD1306 0.96 inch I2C OLED display for the Arduino
### You can find the example codes in full article source in detail here.
### https://randomnerdtutorials.com/guide-for-oled-display-with-arduino/



![image](https://github.com/selldream2/My-Project/assets/27531428/0716ef7c-8e4f-45f6-91e6-d7a2e4712a49)

- SSD1306 model a monocolor
- 0.96-inch display with 128×64 pixels
- Four pins and communicates with the Arduino using I2C communication protocol.\
- Pin wiring
  - I2C pin
  - Vin	: 5V
  - GND : GND
  - SCL	: A5
  - SDA	: A4

- Libraries
  - To control the OLED display you need the adafruit_SSD1306.h and the adafruit_GFX.h libraries. Follow the next instructions to install those libraries.
  - Open your Arduino IDE and go to Sketch > Include Library > Manage Libraries. The Library Manager should open.
  - Type “SSD1306” in the search box and install the SSD1306 library from Adafruit.
  - After installing the SSD1306 library from Adafruit, type “GFX” in the search box and install the library

- Funtions
  - `display.clearDisplay()` – all pixels are off
  - `display.drawPixel(x,y, color)` – plot a pixel in the x,y coordinates
  - `display.setTextSize(n)` – set the font size, supports sizes from 1 to 8
  - `display.setCursor(x,y)` – set the coordinates to start writing text
  - `display.print(“message”)` – print the characters at location x,y
  - `display.display()` – call this method for the changes to make effect

# LCD_I2C
Arduino example for PCF8574/PCF8574A based character LCD (SPLC780/HD44780) I/O controllers.

When I originally received the expander, it took me quite a while to make it work,
and problem was the address, because it was PCF8574A chip and address space on -A
chips is different from non-A version. This Arduino sketch initializes all known
addresses and prints the corresponding address on the LCD, so if one attaches multiple
LCDs, they will all show their own address.

The LCD keeps continuously refreshing, so this can also be used as I2C LCD tester.

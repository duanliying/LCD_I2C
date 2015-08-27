# LCD_I2C
Arduino example for PCF8574/PCF8574A based character LCD (SPLC780/HD44780) I/O controllers.

When I originally received the expander, it took me quite a while to make it work.
There is quite a few libraries out there and all of them claim this one is the ultimate
that 100% works and yet my LCD did not respond. The problem was the address, mine came
with PCF8574A chip (notice the A suffix) and address space on -A expanders is different
from non-A version.

This Arduino sketch initializes all known addresses and prints the corresponding address
on the LCD, so if one attaches multiple LCDs, they will all show their own address.

The LCD keeps continuously refreshing, so this sketch supports hot-swap and can  be used
as I2C LCD tester.

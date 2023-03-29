# esphome-toslink-switch

ESP32 control of simple button+rgb-led style toslink switch (https://www.amazon.se/dp/B089ZVWF66?psc=1&ref=ppx_yo2ov_dt_b_product_details).
Recommended to get one with separate led instead for easier soldering...

1. Connect pin 32 to the first and pin 33 to the last input led indicators.
2. Connect pin 26 to the base of a transistor. Connect the emitter and collector to the button. Pin 26 then effectively pushes the button on the toslink switch.

The ESP32 reads the status on the leds to determine the state of the switch. Note that you only need two input leds to determine all three states.

Change board, names etc. as necessary.

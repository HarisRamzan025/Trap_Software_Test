# Trap_Software_Test
Trap software test on esp32 wroom
Please install the libraries on arduino found in the library folder, also please download the fast led library as well, found in the link below
https://github.com/FastLED/FastLED


To start off, we’ll need a component test program. The technical project details/components lists have been provided (Dropbox).

The test should contain the following features:

1. Neo Pixel Test: The LED ring should light up in a rotating manner for a couple of seconds in order to be able to test if all LEDs are functioning.

2. The battery status (V) should be shown on the serial monitor (2 decimals) and via the Neo Pixel LED ring, based on the following table:

Translations:
Grün -> green
Gelb -> yellow
Ganzer Ring -> Complete Ring
Je, halber Ring -> Half ring each
LED anzeige -> Show LED?

For now, the voltage numbers in column 1 are relevant. We’ll move to another battery later which will make column 2 relevant.

The colors are from-to, i.e. 8.4V-7.71V green, 7.7V-7.41V green/yellow, 7.4V-6.61V yellow etc.

3. The Gyro position should be initialized upon start. On the serial monitor, a notice should be displayed if the angle has changed. It is not necessary to show the exact offset, displaying a change is sufficient.

4. The SIM module should be tested. As part of the test, a message containing the battery status (V) should be sent to a phone number.

To be noted:
All variables (e.g. phone number, PINs, etc) should be named accordingly and placed at the top of the program to make them easily identifiable and changeable.

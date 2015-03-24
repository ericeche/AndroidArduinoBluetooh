CoffeeController
================

Coffeepot Microcontroller


#Design Choices

## Micro Controller Choice

| | Atmega328 (Aurdiuno) | LPC800 Series|
| -------------------------- | ------------------------------------ | ------------------------------------ |
|Cost per unit (quantity 10)|$3.12|$1.60|
|Cost per unit (quantity 100)|$2.84|$0.99|
|Cost per unit (quantity 1,000)|$1.69|$0.69|
|Pro|	Super easy to program|	Super cheap|
|Con|	Slightly more expensive|	Harder to Program 
|||Requires special device to load code onto it|

## Wireless Design choice

| |	CC3000 (Wifi) | CC2541 (Bluetooth)|
| ------------------------------- | ------------------------------- | ------------------------- |
| (quantity 10)|	$20.58|	$12.94|
| (quantity 100)|	$17.49|	$11.09|
| (quantity 1,000)|	$13.29|	$8.93|
|Pro|	Be able to always be connected to the network. This allows for an app that doesn’t require the phone to be near by to use. Coming home from a long day at work, you could go on the app to turn on your coffee maker so it is hot and ready when you get home.	| Cheaper and slightly simpler to configure and set up. |
|Con|	More expensive than the Bluetooth option. Requires a little bit more software to configure. Though this is done with smartconfig, a package that can be loaded into an iphone or android app	| Requires a phone with Bluetooth to be nearby. |

## Real Time Clock

This is used to keep track of time, so alarms can be set. 

[Reference Design] (https://www.sparkfun.com/products/99)

## Power Relay

Use a digitial signal to open and close a VAC power line

[Reference Design] (https://www.sparkfun.com/products/11042)

## AC - DC converter

Used to power the board. 

Instead of trying to develop a custom solution for prototype board, the plan is to instead gut a cheap USB wall wart. This will enable the design to be safer and cheeper as the USB wall warts are produced at a much larger scale. 

[Product Choice] (http://www.monoprice.com/Product?c_id=112&cp_id=11213&cs_id=1082603&p_id=8857&seq=1&format=2)

## Other components

* Oscillator for the clock
* Oscillator for the microcontroller
* Diagnostic LEDs
* Programming port
* various SMD components


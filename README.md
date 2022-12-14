# Solar Tracker

This is a dual axis solar tracker which can orient a small solar panel in horizontal plane (pan) and in vertical plane (tilt).

The solar tracker is based on the leg of the Sam robot.

<img src=https://github.com/magape/SolarTracker/blob/1935c11b0477f71cbbabe97ca98d21a85bd9af2f/3D/img/solar_tracker_3D.png title="Solar tracker" width=24%>     <img src= https://github.com/magape/SolarTracker/blob/4e9680a6272867e0081966e3852bacfaa4263a70/3D/img/sam.png title="Sam" width=30%>

## Mechanical assembly
The parts of the solar tracker can be seen in the next figure.

<img src=https://github.com/magape/SolarTracker/blob/bdeee48374c2c4c5d911661432b44216edad3a6e/3D/img/solar_tracker_annotated_en.png title="Solar tracker parts" width=50%>

The mechanical parts (solar tracker base, servos’ support, solar panel holding foot, solar panel support and shading cross) are 3D printed using [stl files](https://github.com/magape/SolarTracker/tree/main/3D/stl).

The parts are assembled with M2 nuts, bolts, and washers, according to the [pictures](https://github.com/magape/SolarTracker/tree/main/img) showing the step-by-step process.

## Electrical part

The direction of the light source is detected by an optical sensor which has four LDRs. Four analog signals are sent from the sensor to the microcontroller. The sensor is built from scratch.

<img src=https://github.com/magape/SolarTracker/blob/55dfdb1341e153b078db1fd08278cfa78a1f6e69/etc/ldrs_3D_top.png title="Sensor - top" width=25%>   <img src=https://github.com/magape/SolarTracker/blob/55dfdb1341e153b078db1fd08278cfa78a1f6e69/etc/ldrs_3D_bot.png title="Sensor - bottom" width=25%>


The change of the solar panel orientation is made by the two MG90 servos: the pan servo and the tilt servo.

An Arduino Nano board is used as controller. The four analog signals from the LDR’s are transmitted to the Arduino Nano controller. The controller controls each servo through a PWM signal with a frequency of 50 Hz.

<img src=https://github.com/magape/SolarTracker/blob/55dfdb1341e153b078db1fd08278cfa78a1f6e69/img/20220618_160423.jpg title="Solar tracker" width=50%>   

To facilitate the assembly of the electrical circuit (and eliminate the need to use a breadboard) we use an extension board for Arduino Nano.

[<img src=https://github.com/magape/SolarTracker/blob/9dd4d127923d71d00038682b8efd73d441c11e0a/img/20220618_170026.jpg title="Solar tracker" width=50%>](https://youtu.be/WkN0v6vKtUE)

## Credits

The solar tracker was designed by [Mihai Agape](https://github.com/magape).

## Licence

[Licensed under the Creative Commons — Attribution-ShareAlike 4.0 International — CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

## Note

This project has been initiated as part of the Erasmus+ project ["New Generation Schools in the Light of Education 4.0"](https://eduplus.ro).

This is a work in progress.

## Disclaimer
The European Commission's support for the project "New Generation Schools in the Light of Education 4.0" does not constitute an endorsement of the contents of this publication, which reflect the views only of the authors, and the Commission cannot be held responsible for any use which may be made of the information contained therein.

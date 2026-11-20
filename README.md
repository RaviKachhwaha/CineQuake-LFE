<h1 align="center">
  <br>
  <img src="https://github.com/RaviKachhwaha/CineQuake-LFE/blob/main/docs/images/CineQuake-LFE.png" alt="docs/images/CineQuake-LFE.png">

  <br>
  CineQuake-LFE
  <br>
</h1>
<h3 align="center">
A hand-wired Zero PCB device for real-time tactile rumbles-turning any theater seat into 4DX.
</h3>

Note :- At top cover image I will replace it with the completed Zero PCB after build.

| Front Render | Back Render | 
| --- | --- |
| ![](https://github.com/RaviKachhwaha/CineQuake-LFE/blob/main/docs/images/CineQuake-LFE_front_image.png) | ![](https://github.com/RaviKachhwaha/CineQuake-LFE/blob/main/docs/images/CineQuake-LFE_back_image.png) | 

Note:- The Image will come after build due to this will built on Zero PCB, So when I solder all components on PCB then the image is taken and uploaded to here!!

## Schematics  

Here are the schematic design,

![](https://github.com/RaviKachhwaha/CineQuake-LFE/blob/main/docs/images/CineQuake-LFE.png)

## Features
* **Acoustic LFE Wavefront Sensor**: It have a electret condenser mic to capture deep cinema subwoofer waves.
* **48.8 Hz Sallen-Key Sub-Bass Filter**: I added a LM358N op-amp with 22kOhm resistors and 220nF/100nF capacitors to block dialogue and pass only bass.
* **4.5V Virtual Ground Rail**: It have a symmetric 100kOhm voltage divider bypassed by a 10uF capacitor for ripple-free single-supply op-amp biasing.
* **Precision Auditorium Calibration**: I added a 10kOhm potentiometer with an 82kOhm dropper resistor sweeps trigger sensitivity from 0V to 0.98V.
* **Envelope Pulse-Stretching Engine**: I use a 1N4148 diode and 47uF capacitor shape rapid bass hits into punchy ~140 ms tactile rumbles.
* **Saturated Haptic Driver & Snubber**: I also use a PN2222A transistor which drives a silent 3V coin vibration motor with a 1N4007 flyback protection diode.
* **Thermal-Rated 9V Motor Dropper**: I added An 82Ohm 1W resistor which is to safely steps down 9V battery power to 3.0V at 70mA without overheating.
* **Surge Decoupling & Master Switch**: There is a 100uF bulk reservoir, 100nF bypass capacitor, and SPDT slide switch to ensure clean battery operation.
* **Invisible Operation**: It have zero LEDs for silent, invisible operation inside dark theaters.

### The PCB is Zero PCB with 2 layers (bottom and Top) with dimensions 75.00 x 100.00 mm, made to be easily useable for anyone. 

### PCB Schematic Design files are [here](https://github.com/RaviKachhwaha/CineQuake-LFE/blob/main/hardware) 

## Pinout  

This is a general pinout 

| ![](https://github.com/RaviKachhwaha/CineQuake-LFE/blob/main/docs/images/Pin_Outs.png) | 
| --- | 

Note :- This image will come after building the board over Zero PCB.

## 3D image of case 

This is a 3D view screenshot of case for board.

| ![](https://github.com/RaviKachhwaha/CineQuake-LFE/blob/main/docs/images/3D_case_view.png) | 
| --- | 

3D design files are on Onshape [here](https://cad.onshape.com/documents/4bba22cec4122c4bcc3083e4/w/36bf6bd5371a5c47f1820a45/e/f9805e91552ef832d796fe02?renderMode=0&uiState=6b002dea16bcd8ce7b74e065)

(Credits to KiCad EDA for KiCad 10, Texas Instruments for the LM358N dual op-amp, onsemi for the PN2222A NPN transistor, and Hack Club for funding to make this possible.)

## Why was it made?  

While watching movies in normal theaters many time, I realised it doesn't have 4DX, and felling quality and I couldn't got 4DX felling, unfortunately I had to think to go to a 4DX theater but I seen there is no 4DX theater near me or in my city, but now I designed one device with many simplicity's and have power to give me 4DX felling and also give me the top most need of near by 4DX felling.
It will also build my soldering skills more best and perfect.

## How you can get one for yourself? 

That is pretty easy, you have all the files you will need in the hardware folder, order the compoents and BOM list items and solder them by your self on Zero PCB and BINGO! You will have it to use for any movie  in any theaters you want!  

## How do you use it?  
You can use it as any normal device in you pocket but first you want to connect the board input power to 9V Rechargeable battery and then turn on via the switch and set the potentiometer according to your need and you are good to go!
It doedn't require any firmware.

## BOM  
|Name|Purpose          |Quantity|Total Cost (USD)|Link               |Distributor|
|----|-----------------|--------|----------------|-------------------|-----------|
|General Purpose Printed Mini Zero PCB Board |To place every component over it and hand solder them using soldering Iron|1       |1.85           |[Zero PCB](https://www.amazon.in/dp/B0CJJJLB2P)|Amazon India     |
|Components|Needed components to place over Zero PCB and build the working board|1       |47.33           |[Amazon India](https://www.amazon.in)|Amazon India     |
|3D printing |3D printing service for 3D printed case|2       |10.00           |[3D printing](https://3ding.in/)| 3Ding     |
|Rosin Core Soldering Iron Wire |To solder the components over the board|1       |4.96           |[Soldering Wire](https://amzn.in/d/06zNjX09)| Amazon India     |
|Movie ticket 1 |1st Movie ticket is needed to go to theater and test 1st board, and without it I not able to test the board is working or not|1       |6.65           |[Ticket booking platform](https://in.bookmyshow.com/explore/home)| Book My Show     |
|Movie ticket 2 |2nd Movie ticket is needed to go to theater and test 2nd board, and without it I not able to test the 2nd board is working or not (and I also not able to test both boards in 1 movie So I need 2 movie ticket's|1       |6.65           |[Ticket booking platform](https://in.bookmyshow.com/explore/home)| Book My Show     |
| | | Total | 77.44 |

LCSC & DigiKey BOM for the components on board is [here](https://github.com/RaviKachhwaha/CineQuake-LFE/blob/main/components_bom.csv)

!!Thanks to ALL!!

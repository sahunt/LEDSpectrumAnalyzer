# LED Spectrum Analyzer

This project uses LDP8806 LEDs to create a spectrum analyzer which reacts to sound input.

[![LED Spectrum Analyzer on YouTube](http://hackmycab.com/downloads/ytthumb2.jpg)](https://www.youtube.com/watch?v=iJcCQy9E0nU)

**Hardware**

[Arduino Uno](https://www.adafruit.com/products/50)

114 [LDP8806 LEDs](https://www.adafruit.com/products/1948)

[Shifty VU Shield](http://macetech.com/store/index.php?main_page=product_info&products_id=11)

The light bar is using an Arduino with a Vu shield to control the LEDs. The LDP8806 LEDs are individually addressable so they can make some nifty patterns. The audio is fed directly through an audio cable coming from the PC. The frequency of the audio is converted to data through an FFT library which tells the lights how to behave.

This project is based of the visualizatons from sound equalizers. The vertical bars show peaks to represent sound frequency. For this project, the vertical bars are chained together by the ends to create a horizontal bar which "peaks" at both ends.  

Will be updating later with additional information/tutorial.



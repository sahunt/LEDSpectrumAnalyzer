# LED Spectrum Analyzer

This project uses LDP8806 LEDs to create a spectrum analyzer which reacts to sound input via 3.5mm audio cable.

[![LED Spectrum Analyzer on YouTube](http://hackmycab.com/downloads/ytthumb2.jpg)](https://www.youtube.com/watch?v=iJcCQy9E0nU)

** Main Hardware**

[Arduino Uno](https://www.adafruit.com/products/50)

[114 LDP8806 LEDs](https://www.adafruit.com/products/1948)

[Shifty VU Shield](http://macetech.com/store/index.php?main_page=product_info&products_id=11)

The light bar is using an Arduino with a VU shield to control the LEDs. The LDP8806 LEDs are individually addressable so they can make some nifty patterns. The audio is fed directly through an audio cable coming from the PC. The frequency of the audio is converted to data through an FFT library which tells the lights how to behave.

The light display is based of the visualizatons from sound equalizers. The vertical bars show peaks to represent sound frequency. The vertical bars are chained together by the ends to create a horizontal bar which "peaks" at both ends.

##Todo/Wishlist

- Update with additional information/tutorial
- Better use of variables for empty LED colours
- Add light animations when no audio input is received
- Convert NUM_BARS and BAR_LENGTH to # LED var to improve accuracy
- Investigate possibility of having library work independant of volume (volume currently changes the intensity of the peaks)
- Investigate intigration with Stepmania to have lights react to game data

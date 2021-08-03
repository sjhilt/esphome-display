# esphome-display
This is a project I created with a Wemos D1 Mini a SSD1306 Display and some skilled wood working from my father. 

This project is using ESPhome with Home assistant running If you do not have either get those running first: 

https://hass.io (Home Assistant)
https://esphome.io (ESPHome)
SSD1306 Used: https://www.amazon.com/gp/product/B072Q2X2LL/
D1 Mini's Used: https://www.amazon.com/gp/product/B081PX9YFV/

Wood Box is made from Walnut, get creative here and make what ever you like, there is also some 3d printed cases on Thingiverse that I thought about using. 
https://www.thingiverse.com/tag:ssd1306

![Image of Box Off](https://github.com/sjhilt/esphome-display/blob/main/images/box_off.jpg)
# Build Steps

Using the D1 mini, this only requires I2C connetions as there is no other sensors or anything else on this, however you can edit the YAML as needed. 

PIN: 
SDA: D2
SCL: D1
Ground: G
VCC: 3.3 (You can use 3.3 or 5v on the display I used, but it dumps it down to 3.3 if you use 5 so just plug it in 3.3v

# Install Steps 
1) Place the `configuration.yaml` in the inside of yours, this will allow the display to read weather data from home assistant. 

2) In ESPHome addon, create a new board, and copy and paste `esphome_display.yaml` inside that file. Install it to the board and enjoy the sights. 

*Note i'm using a reed switch for my garage door states and if you do not have that you'll need to take it out, this is using another project that I'll upload and link here eventually so if you want to have one of those stay tuned. 


![Image of Box On](https://github.com/sjhilt/esphome-display/blob/main/images/box_on.jpg)

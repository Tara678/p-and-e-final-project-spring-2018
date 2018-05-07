# I'm Instrument

Make an human being into a musical instrument.

## Summary

This entire project lies on the single idea of transforming people into musical instruments.
We attached a conductive material unto a piece of fabric, which is then tied to a person. When that point is touched, a sound made by a specific musical instrument will be produced. For example, when you touch an interactive point on the knees, a drum sound will be heard. Each point features a different sound, and can be played at the same time to produce a complete musical piece.

## Component Parts

Our project relies heavily on capacitive touch so we used the Arduino Due board and the CapitiveSense library to execute that portion. We have 1 pin (pin 4) that is the send pin, and a total of 10 sensor (receive) pins, with a high value resistor (10 ohm) between them—which means we have 10 different sounds. We used the Simple Read library on Processing to transform the data received from Arduino so a sound can be produced. We created strings for our individual sound files, and paths to load and play the files. We then created 2 sets of booleans for each individual sound. The first for the sound itself, and the second for when it’s playing. We also had to work with ASCII charts to determine which values would be true or false for the booleans. If the conductive material is touched (sensor value is above 1000), Arduino will print a sensor output (Sensor.println). In Processing, int val stores the data received from Serial.port. Based on the the value (value), Processing will play different sounds according to those values.

Include what types of inputs/outputs/data it will use, and a block diagram showing how all those pieces are connected.

## Challenges

Every time we call it a day after a successful progress, something is bound to not work the next time we plug it in. For example, sometimes the touch part is sensitive and the sound will respond quickly, but sometimes it’s laggy. We realize after a couple incidents of this that it works better as time goes by—so we hypothesize that the set up works best after it’s been running for about 20-30 minutes. Since it’s a team project, we had to work on two machines. For a while the code that was written in Nathalia’s computer could not work on mine. After checking each individual line of the code, we finally realized it was the port. We also initially used the wrong resistor — we later realized that it’s crucial for us to use the 10 megaohm resistor in order for it to work. The resistor that we were using were not large enough to yield our sensor values. We also had to decrease our sensor value from 3000 to 1000, and then adjusting it to 1500 for some. This is because we notice there’s a delay in some, and hypersensitivity in others. After several rounds of trial and error, we figured that 1000 is our happy number (for now). We also had to figure out the right materials that would be sensitive enough to detect the touch, but is also flexible for us to play around with.

## Timeline

- Week 1: Write proposal
- Week 2: Check out hardware components from Hybrid Lab. Use conductive materials such as fruits and copper to test out the capacitive touch. Find music sound effects.
- Week 3: Add more musical sounds. Adjust touch sensitivity. Refine, test, debug. 
- Week 4: Build final prototype. Test, debug.
- Week 5: Present!

## Completed Work

# I'm Instrument

Make an human being into a musical instrument.

## Summary

This entire project lies on the single idea of transforming people into musical instruments.
We attached a conductive material unto a piece of fabric, which is then tied to a person. When that point is touched, a sound made by a specific musical instrument will be produced. For example, when you touch an interactive point on the knees, a drum sound will be heard. Each point features a different sound, and can be played at the same time to produce a complete musical piece.

## Component Parts

Our project relies heavily on capacitive touch so we used the Arduino Due board and the CapitiveSense library to execute that portion. We have 1 pin (pin 4) that is the send pin, and a total of 10 sensor (receive) pins, with a high value resistor (10 ohm) between them—which means we have 10 different sounds. We used the Simple Read library on Processing to transform the data received from Arduino so a sound can be produced. We created strings for our individual sound files, and paths to load and play the files. We then created 2 sets of booleans for each individual sound. The first for the sound itself, and the second for when it’s playing. We also had to work with ASCII charts to determine which values would be true or false for the booleans. If the conductive material is touched (sensor value is above 1000), Arduino will print a sensor output (Sensor.println). In Processing, int val stores the data received from Serial.port. Based on the the value (value), Processing will play different sounds according to those values.

Include what types of inputs/outputs/data it will use, and a block diagram showing how all those pieces are connected.

## Challenges

Every time we call it a day after a successful progress, something is bound to not work the next time we plug it in. For example, sometimes the touch part is sensitive and the sound will respond quickly, but sometimes it’s laggy. We realize after a couple incidents of this that it works better as time goes by—so we hypothesize that the set up works best after it’s been running for about 20-30 minutes. Since it’s a team project, we had to work on two machines. For a while the code that was written in Nathalia’s computer could not work on mine. After checking each individual line of the code, we finally realized it was the port. We also initially used the wrong resistor — we later realized that it’s crucial for us to use the 10 megaohm resistor in order for it to work. The resistor that we were using were not large enough to yield our sensor values. We also had to decrease our sensor value from 3000 to 1000, and then adjusting it to 1500 for some. This is because we notice there’s a delay in some, and hypersensitivity in others. After several rounds of trial and error, we figured that 1000 is our happy number (for now). We also had to figure out the right materials that would be sensitive enough to detect the touch, but is also flexible for us to play around with.

## Timeline

- Week 1: Write proposal
- Week 2: Check out hardware components from Hybrid Lab. Use conductive materials such as fruits and copper to test out the capacitive touch. Find music sound effects.
- Week 3: Add more musical sounds. Adjust touch sensitivity. Refine, test, debug. 
- Week 4: Build final prototype. Test, debug.
- Week 5: Present!

## Completed Work

![alt text]()

## References and links

https://www.adafruit.com/product/2340

https://www.youtube.com/watch?v=6fzHTwYVKrc

https://makeymakey.com


## References and links

https://www.adafruit.com/product/2340

https://www.youtube.com/watch?v=6fzHTwYVKrc

https://makeymakey.com


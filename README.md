# state-aware-garage-door
esphome code for a state aware garage door sensor and remote using 2 reed switches and a Raspberry Pi Pico W

I wanted to create a garage door sensor and remote that would enable me to keep tabs on my garage door remotely and also operate it remotely. I have the following requirements/parameters/limitations:
- Use a Raspberry pi pico W
- I have a home assistant instance to enable remote monitoring and automation
- Use 2 x reed switch sensors to guage the "open", "closed", "opening" or "closing" states of the door
- My garage door is a "dumb door" that uses a single button to open/close/stop/reverse the door
- My garage door motor has 2 pins on it that need to be shorted to operate the garage door (I'm using a mosfet transistor to act as a toggle switch)
- The code should work irrespective of which switch is used to operate the door and should update the status of the door; i.e. the esphome code or the external remote

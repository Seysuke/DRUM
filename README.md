The piezoelectric sensor modules already come with built-in resistors that help stabilize the signal, so there’s no need to add any external components when using them with an Arduino Leonardo.

As indicated by the arrow on the module, the small screw (trimmer) can be turned to adjust the sensor’s sensitivity — it's most likely a potentiometer or a variable resistor.

As for the button layout, the four sensors are connected to the analog pins A0, A1, A2, and A3 on the Arduino Leonardo. Each pin is mapped to a specific controller button:

A0 → BUTTON_X (Square)

A1 → BUTTON_Y (Triangle)

A2 → BUTTON_A (Cross / X)

A3 → BUTTON_B (Circle)

If you want to rearrange the drum positions without changing the code, you can simply swap the signal wires (e.g., the purple ones) and plug them into different analog pins. This allows you to remap the buttons physically through wiring rather than editing the code.

To finish up, attach the piezo buzzer so that its opening is directly aligned with the fabric of the drum. Be careful not to cover the hole with tape or other materials, as doing so can reduce the sensor’s sensitivity. Once everything’s in place — enjoy the rhythm and have fun!

P.S.: Any improvement or customization you want to try —whether it enhances your personal experience or makes things more convenient for others— is always welcome. If you decide to share your results or ideas, I’d truly appreciate it. Every contribution helps grow and enrich the community.

Regarding Arduino usage, I highly recommend watching tutorials on how to set it up using the XInput library, which is necessary for the code to run correctly. At times, when uploading changes, you might have to press the reset button a few times until the upload begins and you see a confirmation message. Once the upload starts, you can stop resetting.

One idea I explored was adding a small delay or timer before XInput initializes, giving you extra time to upload code without needing to reset manually. I couldn’t get it working myself, but if someone figures it out or finds a better method, it would be a great help for everyone in the community.

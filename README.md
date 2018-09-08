# Automations
Home Automation

hi this is my first project that have uploaded on github. I have been working on home automations for almost 6 months now and i have tried various new features over the existing ones.

One of the innovations that i made was contolling homne appliances such as tubelight, fans etc using clap. In this implementation we aim to control the home appliances such as tube lights and fan using clap. We use a sound sensor to detect the clap. Apart from that we are using Arduino Uno, Breadboard, Jumper wires, Relays, Bulb, Leds. We connect the sound sensor to the ‘analog in’ A0, A1, A2. We cannot use digital pins because the sound sensor provides a analog value as the output. First, we connect a led to check the circuit; the led can be connected at any pins. We have chosen pin 13 for led. The sensor gives the output as the difference between the analog values at its two pins.An ideal value for this difference should be 4 as it will eliminate the turning on of the circuit accidently due to some random noise. Next step in this is to connect bulb to this circuit instead of led. We accomplish this using a relay of either 7A/250V or 12A/120V. We need to use a relay in order to connect his power components to Arduino. Using multiple relays, we can connect multiple components simultaneously using a single Arduino. Finally, we connect our fully running Arduino to the main board of the room and get the desired clap automation. Alternating Current in India (220v) powers the home appliances. Arduino cannot control such high voltage, but a relay can be used to switch control between the high-power devices. 
 

Relay-Appliance Connection: 

Our home appliances (AC controlled) are usually connected with 2 wires attached to a plug.
One wire is connected directly to plug and the other wire is connected to relay first and then from relay to the plug. 
We use relay in NO (Normally Open) mode, it acts like a switch, since it is open.
When a trigger is applied it connects to COM (Common Connection) and the circuit gets closed.
So the toggling between the appliances works using NO and COM of relay. To check if the connection is properly made, run the following code:


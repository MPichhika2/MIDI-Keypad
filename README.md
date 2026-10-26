A MIDI-Keyboard

For this project, I designed a custom MIDI keypad PCB inspired by the MIDI Keypad project. The goal was to create a compact, customizable music controller that can send MIDI inputs to a computer using touch-sensitive keys, a rotary encoder, and a slide potentiometer.


The main components include a Seeed Studio XIAO ESP32-S3, seven capacitive touch pads, three SK6812 MINI-E RGB LEDs, an EC11 rotary encoder, and a Bourns slide potentiometer. As seen in my schematic view! 
<img width="1289" height="889" alt="Schematic" src="https://github.com/user-attachments/assets/44479a86-fb17-4532-abd4-d2e44c3c3819" />

I started by creating the circuit schematic in KiCad, assigning GPIO pins to the touch keys, LEDs, encoder, and slider. I connected the power and ground nets, added power flags, and fixed electrical rule errors.

Next, I assigned component footprints and created a custom footprint containing seven copper touch pads. I transferred everything into the PCB Editor, arranged the components, created the board outline, and routed the electrical connections using front and back copper layers.

<img width="1920" height="990" alt="new_footprint" src="https://github.com/user-attachments/assets/d3bc3234-0be2-4fb4-9401-bf627dfe3077" />

I also modified the LED footprints for front mounting, corrected silkscreen issues, and added a ground plane with a keepout underneath the capacitive touch pads.

Finally, I checked the design using KiCad's Design Rules Checker, achieving zero electrical errors and zero unconnected items. I also began customizing the PCB with rounded corners and planned music-themed artwork and personalized lettering.

<img width="1092" height="634" alt="final3" src="https://github.com/user-attachments/assets/7ec1e444-74c2-442f-9934-c4f973462289" />
<img width="1258" height="680" alt="final2" src="https://github.com/user-attachments/assets/e18f92f5-5c58-488d-add4-9da6f57e2704" />
<img width="722" height="444" alt="final" src="https://github.com/user-attachments/assets/152aa839-2c3f-4d97-aab5-252bb003ca99" />


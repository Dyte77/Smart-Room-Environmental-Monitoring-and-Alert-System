<h1>Smart Room Environmental Monitoring and Alert System.<h1/>


<h3>Project Overview.<h3/>
A system that monitors room environmental conditions (temperature and light intensity) in real-time, providing visual and audible alerts when sensor readings exceed defined thresholds. The system ensures optimal room conditions.


<h3>System Architecture.<h3/>
The system uses an Arduino UNO as the main controller connected to multiple components. Temperature is measured by a temperature sensor on pin A0, while light intensity is detected by another sensor (photoresistor)on pin A1.  Two LEDs provide visual feedback: a red LED on pin 13 flashes during high temperature alerts, and a yellow LED on pin 12 indicates low light conditions. A piezo buzzer on pin 8 sounds an audible alarm when needed.


<h3>How It Works.<h3/>
The system constantly reads sensor values every half-second. The temperature sensor's readings are converted from electrical signals to Celsius degrees using a mathematical formula. Both temperature and light values are shown on the Serial output.

When temperature rises above 35°C, the system enters alarm mode: the red LED flashes rapidly, the piezo buzzer plays alternating high and low beeps. For light control, the yellow LED turns on when the room is dim (light below 400) and turns off when bright enough.

Key Features
The system provides comprehensive monitoring with multiple alert methods. It shows real-time data on an LCD screen while also sending detailed information to a computer for recording. The alert system uses two channels simultaneously: visual (flashing LED), and audible (patterned beeps).. This ensures alerts are noticed immediately. The system also conserves energy by automatically controlling the yellow LED based on ambient light levels.

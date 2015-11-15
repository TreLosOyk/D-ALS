# D-ALS
D-ALS stands for Drone-Assisted Landing System.
First of all this is a University Project under the supervision of Angelos Antonopoulos and Theofilos Chanialakis, TUC, Chania, Crete. In this project we try to make a quad-copter(Drone) land on its own just by staring a base thru a fixed camera.

By using OpenCV 2.4.10 every frame from our drone-mounted camera is being processed in order to be determined the location and the orientation of the base.

#The Base
The base will be represented as three points in a Γ pattern (like QR Contours: Top,Right,Bottom). Those points' shape should be spherical show that they are multi-angle recognisable. Something like orange ping-pong ball will do the trick.

#System overview
The System will be consisted of:
-Camera
-RPi2
-AVR MCU
-Flight Controller
-RC PWM Receiver

Our application is designed to run on a Raspberry Pi 2 which will be mounted on a quad-copter. By utilizing the onboard Serial Connection of the RPi2, the RPi will be able to send info to a AVR MCU.

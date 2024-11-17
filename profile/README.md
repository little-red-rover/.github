# Little Red Rover

ROS enabled robots are (really) expensive, preventing many aspiring robotic engineers from accessing powerful ROS tools.

Little Red Rover (LRR) is a highly capable, differential drive, ROS (1 and 2) robot designed for an amateur budget.
While none of the rovers' specs are top of the line, LRR gives students, hobbyists, and educators a representative ROS experience and an entry point into the wonderful world of research robotics.
Extensive development tooling, example code / projects, and documentation is provided to smooth the learning curve.

## Use Cases

Little Red Rover was developed with educational use in mind. Each rover is affordable enought to be funded by a small course fee, and the detailed documentation and tutorials provide a starting point for a full curriculum.

LRR is perfect for robotics hobbyists interested in elevating their work. Breaking out of tinkery ecosystems like Arduino can be difficult, and LRR is an affordable starting point.

## How Does it Work?

At the heart of Little Red Rover is an ESP32-S3, which collects sensor data and issues commands to the drive base.
Sensor data is relayed over a TCP link to a host computer, which transforms the data into ROS messages on appropriate topics.
Algorithms running within ROS consume the sensor data and generate control commands for the rover, which are relayed back over TCP to the microcontroller.

## Features

* 360 degree LiDAR scanner @ 4000 hz with 8 m range
* 6 degree of freedom IMU
* Wheel encoders with 2340 pulses per rotation
* 5000 mAh battery with USB C charging
* Supports ALL major operating systems through Docker


## Learn More

[Docs](https://github.com/little-red-rover/lrr-docs)

[Template project](https://github.com/little-red-rover/lrr-template-project)

[ROS environment](https://github.com/little-red-rover/lrr-ros)

[Firmware](https://github.com/little-red-rover/lrr-firmware)

[Hardware](https://github.com/little-red-rover/lrr-hardware)

## Thanks

Little Red Rover is my Masters of Engineering (MEng) thesis for Cornell University.

Special thanks to my advisor, [Professor Tapomayukh Bhattacharjee](https://robotics.cornell.edu/faculty/tapomayukh-bhattacharjee-bio/) of the [EmPRISE Lab](https://emprise.cs.cornell.edu/). LRR was inspired by his course, Foundations of Robotics, and his help on the project has been invaluable.

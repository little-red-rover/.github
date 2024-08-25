# Little Red Rover

ROS enabled robots are (really) expensive, preventing many aspiring robotic engineers from accessing powerful ROS tools.

Little Red Rover (LRR) is a highly capable, differential drive, ROS (1 and 2) robot designed for an amateur budget.
While none of the rovers' specs are top of the line, LRR gives students, hobbyists, and educators a representative ROS experience and an entry point into the wonderful world of research robotics.
Extensive development tooling, example code / projects, and documentation is provided to smooth the learning curve.

## Use Cases

Little Red Rover was developed with educational use in mind. Each rover is affordable enought to be funded by a small course fee, and the detailed documentation and tutorials provide a starting point for a full curriculum.

LRR is perfect for robotics hobbyists interested in elevating their work. Breaking out of tinkery ecosystems like Arduino can be difficult, and LRR is an affordable starting point.

## Stackup

Little Red Rover is currently in developement, and the specs below may or may not be implemented already. For now, this section serves as a roadmap.

### Software ([README](https://github.com/usedhondacivic/little_red_rover/tree/main/SOFTWARE))
* ESP32 onboard. Publishes sensor data, encoded using protobuf, over a UDP BSD socket
* Dockerized development environment runs on any OS and communicates with the rover wirelessly
* Hardware abstraction node provided for handling robot connection and republishing deserialized messages

### Hardware ([README](https://github.com/usedhondacivic/little_red_rover/tree/main/HARDWARE))
* [FHL-LD20 Lidar](https://www.youyeetoo.com/products/youyeetoo-fhl-ld20)
* Custom circuit board integrated as the rovers body
* Wheel encoders and IMU for odometry
* Designed for low effort assembly and large scale production

## Thanks

LRR is part of my Masters of Engineering (MEng) thesis for Cornell University.

Special thanks to my advisor, [Professor Tapomayukh Bhattacharjee](https://robotics.cornell.edu/faculty/tapomayukh-bhattacharjee-bio/) of the [EmPRISE Lab](https://emprise.cs.cornell.edu/). LRR was inspired by his course, Foundations of Robotics, and his help on the project has been invaluable.
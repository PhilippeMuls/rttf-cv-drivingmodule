# RTTF_drivingmodule_CV

Simple Computer Vision solution to let the RTTF car drive the track (2020 version)

## Installation

1. Clone this repo in a folder on the Raspberry Pi of the car
2. Open up the docker compose file in to `~/projects/rttf-edgecar/docker-compose.yml`
3. Add the cloned directory as a mounted volume. In `aidrivingmodule` under `volumes` add:
  `- "../drivingmodule:/home/aidrivingmodule/catkin_ws/src/driving_module/src"`
4. If needed, stop, remove and rebuild the `aidrivingmodule` docker container with docker-compose

The code in this repo should then be executed when AI driving is enabled on the car.

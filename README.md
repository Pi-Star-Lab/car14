# car14

## Very very important: make sure the car's wheels are off the ground.

If you have a trained model, follow the following steps.

## Option 1: via WiFi

1. Power up the Raspberry Pi.
2. Connect the Pi to a monitor via an HDMI to micro HDMI cable.
3. Connect to the WiFi network (phone hotspot would work fine). Pi sometimes has issues connecting to iPhone hotspot.
4. Connect your PC to the same WiFi network.
5. On your PC, open a terminal and run: `ssh pistar@172.20.10.2`; the password is `onethrough8`.
6. `cd mycar` and run `python manage.py drive --model models/zach.h5`.
7. On a web browser navigate to `172.20.10.2:8887`.
8. From the dropdown menu select `Auto(S)steer`.

## Option 2: no WiFi

1. Power up the Raspberry Pi.
2. Connect the Pi to a monitor via an HDMI to micro HDMI cable.
3. Open a terminal, `cd mycar`, and run `python manage.py drive --model models/zach.h5`
4. On a web browser navigate to `127.0.0.1:8887`.
5. From the dropdown menu select `Auto(S)steer`.

If you need to train the car using imitation learning, follow the instructions [here](https://docs.donkeycar.com/guide/get_driving/) to collect the data and the instructions [here](https://docs.donkeycar.com/guide/deep_learning/train_autopilot/) to run the training script.

DJI Mini2 RC as a Joystick
===============
 - Connect your DJI Remote Controller to your PC and use it to play simulators
 - Currently confirmed working controllers: DJI Mini 2 RC (also known as RC-N1, RCS231, WM161b-RC-N1, RCN1)
 - 16/02/2024 - added full support of 4 buttons that are mapped as joystick buttons
 - inspired by (actually improved and modified for Mini 2 RC) [justin97530/miniDjiController](https://github.com/justin97530/miniDjiController)
-----------------------------------------------------------------------------

to run it
- install dependencies (you may need to install them under sudo)
- connect your RC via the bottom type-c USB connector to your laptop
- run "sudo python3 main.py -p /dev/ttyACM0"
- your RC will be set to simulator mode and it will pass stick values to the virtual joystick (/dev/js0)

If you have problems running it on Python 3.11, use this solution offered by [jim3692](https://github.com/jim3692) to run on 3.10.4

- Download Python 3.10.4 by running ```pyenv install 3.10.4```
- Set it as default for this project with ```pyenv local 3.10.4```
- Create a Python Virtual Environment with ```python -m venv .```
- Install the dependencies in the venv with ```pip install -r requirements.txt```
- Then run ```sudo python main.py -p /dev/ttyACM0```

You may need to run "sudo modprobe uinput" in case you have "OSError: [Errno 19] Failed to open the uinput device: No such device" error.

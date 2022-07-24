DjiMini2RCasJoystick
===============
 - Connect your DJI Remote Controller to your PC and use it to play simulators
 - Currently confirmed working controllers: DJI Mini 2 RC (also known as RC-N1, RCS231, WM161b-RC-N1, RCN1)
 - inspired by (actually improved and modified for Mini 2 RC) [justin97530/miniDjiController](https://github.com/justin97530/miniDjiController)
-----------------------------------------------------------------------------

to run it
- install dependencies (you may need to install them under sudo)
- connect your RC via bottom type-c usb connector to your laptop
- run "sudo python3 main.py -p /dev/ttyACM0"
- your RC will be set to simulator mode and it will pass stick values to virtual joystick (/dev/js0)

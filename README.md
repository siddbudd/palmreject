# Palm rejection for bash and xinput

Forked from https://github.com/olofmogren/palmreject/issues

## Tested on

- OS: Ubuntu 20.04 beta with Gnome 3.36. 
- Hardware: Cube i7 Stylus.
- Software: Stylus Labs Write

## Version notes

Code is temporarily hardwired to use my own device IDs, until I can find the bug causing the original version not to find my devices.

## Dependencies

bash and xinput

## Function

Turns off touchscreen input when stylus is near screen. Stylus status is checked every 100 ms, a timeout is by default set to 2 seconds for re-enabling the touchscreen after stylus input.

## Usage

Run "xinput list" to check the IDs of your devices and edit the respective lines in palmreject.sh.
Run ./palmreject.sh every time you login.

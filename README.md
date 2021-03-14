# Palm rejection for bash and xinput

## Source

olofmogren / palmreject

## Tested on

- OS: Ubuntu 20.04 beta with Gnome 3.36, Kubuntu 20.10
- Hardware: Cube i7 Stylus
- Software: Stylus Labs Write

## Version notes

Code is temporarily hardwired to use my own device IDs, until I can find the bug causing the original version not to find my devices.
Added rejection for eraser (my stylus comes with it and it palm should be rejected in both cases)

## Dependencies

bash and xinput (both preinstalled on Ubuntu)

## Function

- Turns off touchscreen input when stylus is near screen. 
- Stylus status is checked every 100 ms, a timeout is by default set to 2 seconds for re-enabling the touchscreen after stylus input.

## Usage

1. Run "xinput list" to check the IDs of your devices and edit the respective lines in palmreject.sh.
2. Run ./palmreject.sh every time you login.

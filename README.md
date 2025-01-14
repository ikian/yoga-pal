# Yoga-370 [![Circle CI](https://circleci.com/gh/RealOrangeOne/yoga-pal.svg?style=svg)](https://circleci.com/gh/RealOrangeOne/yoga-pal)

Command line tool for controlling screen rotation on Lenovo Yoga-370 laptops. This tool is specifically designed for and test on Yoga-370 laptops, other devices support may vary.

## Requirements
* Python 3
* Pip

## Installation
Installation can be done in 2 ways, both of which involve the `install.sh` script.
##### Option 1
1. Clone the repo
2. cd into it
3. run `install.sh`

##### Option 2
1. Download the `install.sh` file
2. Put the file in the directory you want to install into
3. run `install.sh`

## Development
If you wish to install this in a development environment, clone the repo, and then:

	scripts/build
    source env/bin/activate
	pip install --editable .

__Note__: Installation must be done with an active internet connection.

## Usage

### Rotate
	yoga rotate screen
	yoga rotate touch
	yoga rotate all
Rotates the screen, touchscreen, or both. All is used by default if no component is givens.

__Note__: Rotating touchscreen is likely done automatically with screen, and cannot be overriden. Only added as a catch-all.

Flags `--flip` and `--default` can be added to this command to specify the orientation required.

### Enable & Disable
    yoga enable trackpad
    yoga disable trackpad

    yoga enable touch
    yoga disable touch

    yoga enable all
    yoga disable all
Disables / Enables the trackpad, touch screen, or both. All is used by default if no component is given.

### Modes
    yoga mode laptop
    yoga mode tablet

    yoga mode list

Switches your device between the modes of yoga devices, configuring the optimum setup automatically. You can use `yoga mode list` to see all the available modes.

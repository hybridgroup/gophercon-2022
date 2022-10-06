# Parrot Minidrone

The Minidrone from Parrot uses a Bluetooth interface and programming API.

You can use [Gobot](https://github.com/hybridgroup/gobot) to control the drone from your notebook computer.

## What you need

    - Parrot Minidrone
    - Personal computer with Go 1.19+ installed
    - Works on Linux, macOS, or Windows

## Installation

For Mac users you'd need to:
- Open system preferences 
- Click on Security & Privacy
- Click on the privacy tab
- Select bluetooth
- Click add (+)
- Add your terminal application (e.g. iterm)


## Running the code
When you run any of these examples, you will compile and execute the code on your computer. When you are running the program, you will be communicating with the Minidrone using the Bluetooth interface.

### Initial testing
Therefore, you must connect to the Minidrone drone by knowing the correct name and MAC address for that drone.

To test the drone you need to run the `main.go` in the `step1` folder. The programs requires the MAC address of the drone, which would be one of the following:

- For the yellow drone use `d842d428-7310-d27d-e0e1-e1b4e7990a31`
- For the white drone use `b5ea65f9-060a-f1d5-9dcf-13f5a793520b`

For example, for the yellow drone:  
`cd step1`  
`go run main.go d842d428-7310-d27d-e0e1-e1b4e7990a31`

### Control the drone with your keyboard
To control the drone with keyboard:
- go to the keyboard folder
- run `main.go` and pass the MAC address of the drone as the parameter.

For example, for the white drone:  
`cd keyboard`  
`go run main.go b5ea65f9-060a-f1d5-9dcf-13f5a793520b`

Once it's running the following keys control the drone:

- Left square brcket `[` to take off
- Right square brcket `]` to land
- `w` moves the drone forward
- `s` moves the drone backward
- `a` moves the drone left
- `d` moves the drone right
- `esc` to exit the program

Note: For additional control keys check the code at `keyboard/main.go`
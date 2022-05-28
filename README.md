## Dependicies

1. Ubuntu 20.x "focal" LTS
2. OpenCV: `sudo apt-get install libopencv-dev`

## Usage

1. 
    `cmake .`, `make`
2. Run the executable binary
    `./ellipse input.avi`
3. Drag the mouse over the region of interest of the first frame by using the mouse left click, then execute by using mouse right click
4. Run python script to create output video
    `./genvid.sh`

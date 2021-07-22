# Magic-Piano

Magic Piano is a computer vision-based project that allows you to play a virtual piano using hand recognition through a camera.

## Pipeline

### 1. Hand detection

We get a frame from the camera and use Open-CV Hand Detector to recognize hands and get information about key points of the palm.

![](src/docs/hand.png)

### 2. Press detection

Next, we draw the piano on frame and use the coordinates of the key points to track the keypress. When pressed, the corresponding sound is played.

![](src/docs/press.png)

### 3. Displaying

At the last stage, we display the frame on the screen of the GUI created using PyQt5

![](src/docs/gui.png)

## How to use

First, you need to clone this repository to a folder that does not have Russian letters in the path.
Example:
```bash
cd C:/Users
git clone https://github.com/DumDereDum/Magic-Piano.git
```
Then, go inside the folder "Magic-Piano" and run .exe file

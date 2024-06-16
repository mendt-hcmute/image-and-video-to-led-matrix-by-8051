# image-and-video-to-led-matrix-by-8051
C code can be execute by Keil C, Python code can be execute by PyCharm or Spyder.

Python UI is created by using PyQt5
To processing image and video
  First, using function to load image or video.
  Second, loading completed, resize that components to grey image/video
  Third, resize it to 8x8. And base on brightness of that point to decide it will be 'HIGH' or 'LOW' in led matrix.
  Four, convert these result to HEX code. Using Serial to send code to microcontroller 8051.
  Additional, with video, need to remove some frame is duplicated, then send code to microcontroller. Its will be more simple.

To handling HEX code Receive by Serial can using Interrupt because it can be execute when serial received a byte. (RX = 1)

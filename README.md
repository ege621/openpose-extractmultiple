# openpose-extractmultiple
This code extracts keypoints from multiple videos in a directory in sequence using subprocess.

Originally, openpose only allows you to extrasct keypoints from a single video, which makes huge amounts of data extraction a hassle, especially for deep learning applications where a lot of data is needed.

Your video folder should be in the same directory with the .ipynb file for this to work. 

Please refer to the [original openpose arguments documentation](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/include/openpose/flags.hpp) if the provided commands do not work for you, since the commands you pick depend on the hardware you use and the resolution of the videos you wish to process.

Please note that openpose has CPU and GPU versions. It will take a SUBSTANTIAL amount of time to extract keypoints using the CPU.
If you encounter sudden crashes or, instant crashes when you run the code, you probably have to change the --net-resolution argument to something lower.

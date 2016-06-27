# CamControl
Laser coupled microscopy system based on OpenCV

Based on Debian architecture. Requires OpenCV, libv4l2, videodev2, ioctl. 
The software serves as a capturing system for the Müller-Wedel surgical microscope with 3 cameras attached. Acquisition happens via 4 channel PCI video card with a techwell 6805 single chip. The software refers to the cameras by enumeration from 1 to 3, where camera 1 (left) represents a CCD camera with no additional filtersystem. This is generally considered as a reference. CCD
camera 2 (middle) has a pre-installed filter designed for detecting fluorescence of pTurbo (ex 588/em 633) but requires additonal setting for excitation filter (behind microscope head, filter no. 1). CCD camera 3 (right) is equiped with a IR filter and highly sensitive to IR light, suitable for ICG. This camera requires excitation filter 2 to prevent overexposure.

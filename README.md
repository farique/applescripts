applescripts
============
Custom Apple Scripts

Folder Action Scripts
-------------

###Image Ratio Sort (common).scpt

Script sorts new added images by aspect ratio and moves to appropriate folders.

Example

    Input (added files): 1.jpg (1920x1200) 2.jpg (460x640) 3.jpg (970x1533) 4.jpg (600x900) 5.jpg (460x586) 6.jpg (700x525) 7.jpg (500x440)
    Output:
    ./1,14x1: 7.jpg
    ./16x10: 1.jpg
    ./1x1,0: 2.jpg
    ./1x1,27: 5.jpg
    ./1x1,58: 3.jpg
    ./2x3: 4.jpg
    ./4x3: 6.jpg

###Image Ratio Sort (GCD).scpt

Script sorts new added images by aspect ratio and moves to appropriate folders.
Aspect ratio is calculated using GCD (Greatest common divisor http://en.wikipedia.org/wiki/Greatest_common_divisor)

Example

    Input (added files): 1.jpg (1920x1200) 2.jpg (460x640) 3.jpg (970x1533) 4.jpg (600x900) 5.jpg (460x586) 6.jpg (700x525) 7.jpg (500x440)
    Output:
    ./1x1: 2.jpg
    ./230x293: 5.jpg
    ./25x22: 7.jpg
    ./2x3: 4.jpg
    ./4x3: 6.jpg
    ./8x5: 1.jpg
    ./970x1533: 3.jpg

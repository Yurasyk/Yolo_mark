# Yolo_mark for marking object orientation AFTER marking bounded boxes by the original Yolo_mark
**Windows** & **Linux** GUI for marking orientation of objects in images for training oriented Yolo v3 by the modified darknet framework for Oriented Y

* To compile on **Windows** open `yolo_mark.sln` in MSVS2013/2015, compile it **x64 & Release** and run the file: `x64/Release/yolo_mark.cmd`. Change paths in `yolo_mark.sln` to the OpenCV 2.x/3.x installed on your computer:

    * (right click on project) -> properties -> C/C++ -> General -> Additional Include Directories: `C:\opencv_3.0\opencv\build\include;`
        
    * (right click on project) -> properties -> Linker -> General -> Additional Library Directories: `C:\opencv_3.0\opencv\build\x64\vc14\lib;`

* To compile on **Linux** type in console 3 commands:
    ```
    cmake .
    make
    ./linux_mark.sh
    ```

Supported both: OpenCV 2.x and OpenCV 3.x

--------

1. To test, simply run 
  * **on Windows:** `x64/Release/yolo_mark.cmd`
  * **on Linux:** `./linux_mark.sh`

2. To use for labeling your custom images:

 * delete all files from directory `x64/Release/data/img`
 * copy all files from directory `x64/Release/data/img` created by the original Yolo_mark
 * run file: `x64\Release\yolo_mark.cmd`


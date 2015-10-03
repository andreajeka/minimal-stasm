# minimal-stasm
Minimal program included in the STASM folder can now be run with OpenCV 3.0.0 in Eclipse using MinGW

1. minimal.cpp is the driver program (containing main)
2. Source files are all *.cpp files
3. Header files are all *.h files
4. OpenCV library files need to be configured in Eclipse are:
  1. highgui
  2. core
  3. imgcodecs
  4. imgproc
  5. objdetect
  
###Configuring Eclipse linker for OpenCV
1. Go to Properties -> C/C++ Build -> Settings -> MinGW C++ Linker -> Libraries
2. Add entries to Libraries(-l). Each entry is each item in the following:
  1. opencv_highgui300
  2. opencv_core300
  3. opencv_imgcodecs300
  4. opencv_imgproc300
  5. opencv_objdetect300
3. Add a path entry to Library search path (-L) : "OPENCV3.0_DIR/build/lib"
4. Go to Properties -> C/C++ Build -> Settings -> GCC C++ Compiler -> Includes
5. Add entries to Include paths (-l) according to the location of your files. Possibly might be in "OPENCV3.0_DIR/source/include" or "OPENCV3.0_DIR/source/modules"


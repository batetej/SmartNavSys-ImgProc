COMPILER=arm-linux-gnueabihf-g++-4.9

all:
	$(COMPILER) main.cpp -g -o main.bin \
	-I/tmp/opencv/buildCross/installation/include \
	-L/tmp/opencv/buildCross/installation/lib \
	-lopencv_core -lopencv_imgproc -lopencv_imgcodecs 
	
	
	
asd:	
	-lopencv_highgui -lopencv_calib3d -lopencv_features2d \
	-lopencv_flann -lopencv_ml -lopencv_objdetect -lopencv_photo -lopencv_stitching \
	-lopencv_superres -lopencv_video -lopencv_videostab -lopencv_videoio \

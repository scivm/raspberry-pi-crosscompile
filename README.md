raspberry pi cross compilation
------------------------------

Based on this stack overflow article 
http://stackoverflow.com/questions/19162072/installing-raspberry-pi-cross-compiler/19269715#19269715 

Test the hello world program first: 
cd /opt/rpi/cmake-hello-world 
mkdir build 
cd build 
cmake -D CMAKE_TOOLCHAIN_FILE=$HOME/raspberrypi/pi.cmake ../ 
make 
scp CMakeHelloWorld pi@192.168.1.PI:/home/pi/ 
ssh pi@192.168.1.PI ./CMakeHelloWorld 
Now run the program from your PI 


OpenCV example 



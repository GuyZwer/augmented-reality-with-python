Thie is the AR project.
	
	in this project Im going to use OpenCV to program an AR in Python
	at first I thought to use Pygame, but I read on the net about it, and it
	doesnt look that it fit my need for this project and I was reading about
	AR that work great with Java, but since I dont know to program in Java,
	I decided to use my knowledge in Python and use OpenCV

	this is my first project EVER! so, Im so exciting to start progreming in
	Python. my source code will be publish hear for every one.
	for this project I will use toturials from the net
	and my resources is as folloing:
	https://www.python.org/
	http://docs.opencv.org/3.0-beta/doc/py_tutorials/py_tutorials.html
	https://www.enthought.com/products/canopy/
	https://www.jetbrains.com/pycharm/
	In this project I will mention the errors that popup during the installation.
	
	Im useing Fedora 19 (32-bit) on vmware
	I'm useing the documentation from the following:
	http://docs.opencv.org/3.0-beta/doc/py_tutorials/py_setup/py_setup_in_fedora/py_setup_in_fedora.html#install-opencv-python-in-fedora
	
	At the section "Configuring and Installing" I have the problem with make the files 
	and prepare them to installation
	My errors are as follow:
		/lib/libavcodec.so.54: undefined reference to `vpx_codec_vp9_dx_algo'
		/lib/libgbm.so.1: undefined reference to `wayland_buffer_is_drm'
		/lib/libavcodec.so.54: undefined reference to `vpx_codec_vp9_cx_algo'
		collect2: error: ld returned 1 exit status
		make[2]: *** [bin/opencv_perf_core] Error 1
		make[1]: *** [modules/core/CMakeFiles/opencv_perf_core.dir/all] Error 2
		make: *** [all] Error 2
		
	I codnt find on the net the reason for this issue, I just know that thos problem is somting with 
	libavcodec.so.54 file it dosnt contin the the value 'vpx_codec_vp9_dx_algo', so I deside to carry on.
	on the ~/.bashtc I added the path as follow:
	export PYTHONPATH=$PYTHONPATH:/usr/lib/python2.7/site-packages
	I log out and come back again and that I accomplish the yum update command.
	after that I 'make' again and I have no error and it finish successfully
	
	Now connect to python and type import cv2, and HOLLA! it works!!!
		
		
		

	
	
	

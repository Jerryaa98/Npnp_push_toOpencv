# Npnp_push_toOpencv

This is an cloned OpenCV directory with Newton Pnp solver in it.

This project was done in association with the robotics lab in the university during summer 2021. 

Newton PNP can be found here: https://github.com/rbdlabhaifa/Newton-PnP

in order to run the program on ubuntu/linux OS:-
1) clone the directory
2) cd ~/opencv_build/opencv/build
3) cmake -D CMAKE_BUILD_TYPE=RELEASE \
      -D CMAKE_INSTALL_PREFIX=/usr/local \
      -D INSTALL_C_EXAMPLES=ON \
      -D INSTALL_PYTHON_EXAMPLES=ON \
      -D WITH_TBB=ON \
      -D WITH_V4L=ON \
      -D WITH_QT=ON \
      -D WITH_OPENGL=ON \
      -D OPENCV_EXTRA_MODULES_PATH=../../opencv_contrib/modules \
      -D BUILD_EXAMPLES=ON ..
      
4) make -j4
5) bin/example_tutorial_pnp_registration
6) bin/example_tutorial_pnp_detection --method=9

Video Demo can be found here:-
https://www.youtube.com/watch?v=FVppFUGSOIQ&ab_channel=TheJojitto95

for comparison the opencv pnp solver:-
https://www.youtube.com/watch?v=49CvyrOW9gM&ab_channel=TheJojitto95

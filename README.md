# shape-custom

##this is a file and installation directory for my study in segmentation
##the youtube video and tutorial can be found here
##https://www.youtube.com/watch?v=udR6SwojYXo&list=PLhA3b2k8R3t3zhbjDmqHudUTZqvRdELgd&index=6


###(1). Setup conda in Ubuntu 16.04 env with ROS (need extra steps)

###1. installing conda
####download .sh file from homepage
####https://www.anaconda.com/products/individual#linux

####'''cd ~/Downloads'''

####bash <filename of the downloaded source>
####for me it was 
####bash Anaconda3-5.0.1-Linux-x86_64.sh

###1-1. (Only for ros users)After installation go to your home directory
###This step is done due to the fact that conda interupts the python2.7 environment for ROS

####gedit ~/.bashrc
####comment out Anaconda related python settings when using ROS
####http://wiki.ros.org/IDEs#Anaconda
####in my case when using Anaconda, uncomment all the lines. 
####Because my installation had issues in conda init

###2. install the package from github
####https://github.com/seth814/Semantic-Shapes
####when installing in desktop

####cd
####cd Desktop
####mkdir shape-custom
####git clone https://github.com/seth814/Semantic-Shapes

###3. activate conda env with py37 and install packages

####conda create -n shape-custom python=3.7
####activate shape-custom
####cd shape-custom/Semantic-Shapes
####pip install -r requirements.txt

###4. install pygame and pydensecrf
####sudo apt-get install python3-setuptools
####sudo easy_install3 pip
####sudo pip3 install pygame

####pip install git+https://github.com/lucasb-eyer/pydensecrf.git

###5. All installations done. It depends on your environment but when opencv is linked to python 2.7 dist
###you should run 
####unset PYTHONPATH

###6. check if collect.py is running
####python3 collect.py




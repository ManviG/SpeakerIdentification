Speaker recognition is the identification of a person from characteristics of voices. It can 
be used to authenticate or verify the identity of a speaker as part of a security process.

This project aims at identification of a new voice sample among the given voice samples. 

The easiest way to install some of these libraries is using Anaconda, others can be installed 
using pip or from source. mlpy requires the latest version of GNU Scientific Library (GSL)  
and also libc (system C compiler) version 2.14 (or above). If libc version is older than 2.14, a 
parallel installation of libc 2.14 (or above) has to be linked with the libsvm.so ​
shared library in Mlpy.

Dependency Installation procedure 
1. To install Anaconda 
  a. Download installer from 
    http://repo.continuum.io/archive/Anaconda2­4.1.0­Linux­x86_64.sh   ​
    using wget http://repo.continuum.io/archive/Anaconda2­4.1.0­Linux­x86_64.sh 
  b. Give proper permissions to the shell script to run it 
    i. sudo chmod +x script_name.sh 
  c. In terminal window type the following: 
      bash Anaconda2­4.1.0­Linux­x86_64.sh 
  e.  Restart the terminal to finish installation 
 
2. To install Theano and Keras, in your terminal type 
  a. sudo pip install theano 
  b. sudo pip install keras 
   
3. To install GSL libraries  
  a. Download the latest version from http://gnumirror.nkn.in/gsl/.
    i. wget http://gnumirror.nkn.in/gsl/gsl­2.1.tar.gz 
  b. Extract the contents of the .tar.gz file 
    i.  tar ­ xvzf <filename of the extracted tar file> 
  c.   Enter the directory and type  
    i.  ./configure 
    ii. sudo make 
    iii. sudo make install
    
4. To install mlpy 
  a. Download the latest version from http://sourceforge.net/projects/mlpy/files/ 
  b. Extract the contents of the .tar.gz file using tar ­xvzf <filename> 
  c. Enter the extracted directory and type sudo python setup.py install   
  
  
If above method of installation doesn’t work then follow these steps: 
1. git clone https://github.com/lukauskas/mlpy.git 
    a. To install git 
      i. yum install git 
      ii. git config ­­global user.name “testuser” 
      iii.git config ­­global user.email “testuser@example.com” 
      iv. cd mlpy 
2. sudo python setup.py install 
 
 
5. To install bob type  conda install bob.io.audio bob.io.base bob.bio.spear 


To run : 

The directory contains the python scripts for the implementation. The main 
scripts is ‘speaker_identification.py’, and it can be run using command line terminal. For training over new 
speech samples use the following command :
 
      python speaker_identification.py train /<path to train directory  for training> 
 
For testing over a pre trained model use the following command :
      
    python speaker_identification.py test <phone_number> /<path to test file for test >


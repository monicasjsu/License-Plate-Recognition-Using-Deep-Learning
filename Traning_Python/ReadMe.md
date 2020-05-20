# Prerequisites
``pip install -r requirements.txt``


# Install Darknet
```
git clone https://github.com/pjreddie/darknet.git
cd darknet
mv ../custom darknet
wget https://pjreddie.com/media/files/darknet53.conv.74
```

# Run Darknet

If not using CUDA and OpenCV
```
make
```

Otherwise edit MakeFile and enable OpenCV and CUDA if needed and then 
```
OPENCV=1
GPU=1
CUDNN=1

export PKG_CONFIG_PATH=/path/to/the/file
cd darknet
make
```

 



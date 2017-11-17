# OpenCV for Raspberry-Pi(라즈베리파이를 위하 OpenCV)
라즈베리파이에 OpenCV와 OpenCV-Python을 컴파일 없이 설치할 수 있게 미리 빌드한 데비아 패키지 설치 파일입니다. 
이것을 이용하면 2시간 정도를 절약할 수 있고 빌드 도중 발생하는 다양한 문제로 부터 해방될 겁니다.
라즈베리파이 3 모델 B+에서 빌드 되었습니다.

pre-built debian package files of OpenCV for Raspberry-Pi. You can install OpenCV and OpenCV-Python package to your Raspberry-Pi without compile.
It will save you from stressfull task and a couple of hours time. This was compiled on RaspberryPi 3 Model B+.


# Instruction

## 1. apt update
``` 
sudo apt update
sudo apt upgrade
```
If you are busy, you can skip 'upgrade', but 'update' is necessary.

시간을 절약하려면 'upgrade'는 안해도 되는데, 'update'는 꼭 해야 합니다.

## 2. install dependency packages(종속 라이브러리 설치)
```
sudo apt install -y libxine2  libqtgui4 libjasper1 libqt4-test libqt4-opengl
```

## 3. Download and Install
```
git clone 
cd opencv-for-rpi
sudo dpkg -i OpenCV*.deb
```

## 4. Check the result(결과 확인)
```
$ pkg-config —modversion opencv
```





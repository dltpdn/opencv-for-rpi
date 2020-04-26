# OpenCV for Raspberry-Pi(라즈베리파이를 위한 OpenCV)
These are Debian package installation files that are pre-built to install OpenCV and OpenCV-Python on Raspberry-Pi without compilation process.
Using it will save your time about two hours and will free you from various problems that arise during the build.
It was compiled on RaspberryPi 3 Model B.

라즈베리파이에 OpenCV와 OpenCV-Python을 컴파일 없이 설치할 수 있게 미리 빌드한 데비아 패키지 설치 파일입니다.
이것을 이용하면 2시간 정도를 절약할 수 있고 빌드 도중 발생하는 다양한 문제로 부터 해방될 겁니다.
라즈베리파이 3 모델 B에서 빌드했습니다.


# Instruction

## 1. apt update
```
$ sudo apt update
$ sudo apt upgrade
```
If you are busy, you can skip 'upgrade', but 'update' is necessary.

시간을 절약하려면 'upgrade'는 안해도 되는데, 'update'는 꼭 해야 합니다.

## 2. Download
Download files that you want to install from releases page.
릴리즈 페이지에서 원하는 버전을 선택해서 다운로드 받으세요.

* https://github.com/dltpdn/opencv-for-rpi/releases

## 3. Installation
```
~/opencv-for-rpi/stretch/3.4.0 $ sudo apt-get install -y ./OpenCV*.deb
```
or
```
~/opencv-for-rpi/stretch/3.4.0 $ sudo dpkg -i ./OpenCV*.dev
~/opencv-for-rpi/stretch/3.4.0 $ sudo apt install -f
```

## 3. Check the result(결과 확인)
```
~ $ pkg-config —modversion opencv  #opencv 3.4.0
```
```
~ $ dpkg -l |grep opencv
```

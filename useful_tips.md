# RaspberryPi-For-Makers

## 1장
### 헤더리스 이미지 만들기
SD카드 이미지 수정만으로 파이를 세팅하는 방법을 [headless_setup.md](https://github.com/raspberry-pi-maker/RaspberryPi-For-Makers/blob/master/tips/chap-01/headless_setup.md) 를 통해 확인할 수 있습니다.<br /><br />

### SD 카드 이미지 사이즈 변경
백업해둔 SD카드 이미지를 복원하려고 할때 같은 용량의 SD카드라 할지라도 제조사가 다르면 복원이 안되는 경우가 있습니다. 아마 많은 분들이 이런 경험이 있을 겁니다. 특히 작은 사이즈의  SD카드를 이용한 복원은 아예 불가능하죠. 이 문제를 해결하려면 백업해둔 SD카드 이미지(img 파일)의 크기를 줄여야 합니다. 백업 img 파일은 2개의 파티션으로 이루어져 있습니다. 하나는 boot 파티션이며 ExFAT 파일 시스템을 이용하기 때문에 PC에서도 제대로 보입니다. 하지만 두번째 파티션은 리눅스 파일 시스템이기 때문에 Windows PC에서는 이 파일 시스템 접근이 어렵습니다. 따라서 Windows에서 파티션 수정이 쉽지 않습니다. 구글링을 해보면 대부분 리눅스(파이 포함)에서 SD카드 이미지의 크기를 줄이는 방법을 설명합니다. 그런데 문제는 이 과정이 상당히 복잡하고 어렵다는 것입니다. 이 과정을 스크립트 파일을 이용해 쉽게 작업할 수 있는 방법을 알려드립니다. 제가 해본 여러가지 중에 가장 효율적인 방법이었습니다.
 [sdcard_resize.md](./tips/chap-01/sdcard_resize.md) 를 통해 확인할 수 있습니다.<br /><br />


### VSCode를 이용한 원격 파이썬 디버깅
2017년 책을 쓸 당시에는 VSCode에서 sftp extension을 이용한 원격작업을 권장했습니다. 하지만 이제 마이크로소프트의 무료 편집기인 VSCode의 Remote Development 확장을 이용하면 로컬컴퓨터에서 작업하는 것처럼 완벽한 코드 수정이 가능할 뿐 아니라 Visual Studio와 같은 통합개발환경에서나 가능하던 GUI 디버깅 또한 가능하기 때문에 개발 속도를 높일 수 있습니다. [vscode.md](https://github.com/raspberry-pi-maker/RaspberryPi-For-Makers/blob/master/tips/chap-01/vscode.md) 를 통해 확인할 수 있습니다.<br /><br />

### USB-TTL을 이용한 시리얼 콘솔 연결
가끔씩 외부에서 키보드, 모니터, 인터넷 등이 없는 환경에서 노트북에서 파이를 연결해 작업해야 하는 경우가 있을 수 있다. 이 경우 시리얼 콘솔 사용법을 알고 있으면 큰 도움이 될 수 있다. [serial_console.md](https://github.com/raspberry-pi-maker/RaspberryPi-For-Makers/blob/master/tips/chap-01/serial_console.md) 를 통해 확인할 수 있습니다.<br /><br />


## 4장
### 쌍극 스테퍼모터(NEMA 모터) 제어
책에서는 단극 스테퍼 모터만 다루었는데 3D 프린터를 비롯한 현장에서 많이 사용하는 NEMA 스테퍼 모터와 drv8825, tmc2100 등의 드라이버 사용법을 [bipollar_stepper_motor.md](https://github.com/raspberry-pi-maker/RaspberryPi-For-Makers/blob/master/tips/chap-04/bipollar_stepper_motor.md) 를 통해 확인할 수 있습니다.<br /><br />


## 7장
### OpenCV 소스코드 빌드
OpenCV는 아주 활발하게 업데이트가 발생하는 오픈소스 패키지입니다. apt-get 명령어를 이용한 OpenCV  설치 대신 최신 소스코드를 직접 빌드해서 사용하고자 하는 분들은 [opencv.md](https://github.com/raspberry-pi-maker/RaspberryPi-For-Makers/blob/master/tips/chap-07/opencv.md)를 참조하시길 바랍니다.

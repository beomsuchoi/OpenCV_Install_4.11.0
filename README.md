# OpenCV_Install_4.11.0

---

**Copyright 2025 beomsuchoi**  
**GitHub:** https://github.com/beomsuchoi/OpenCV_Install_4.11.0  
**Licensed under Apache License Version 2.0**  
**Refered to https://docs.opencv.org/4.x/d7/d9f/tutorial_linux_install.html**  

---

## 설치 가이드

Ubuntu 22.04에서 OpenCV 4.11.0을 자동으로 설치하는 스크립트입니다.


### 단계별 설치
```bash
git clone https://github.com/beomsuchoi/OpenCV_Install_4.11.0.git
cd OpenCV_Install_4.11.0
chmod +x 4.11.0.sh
./4.11.0.sh
```

### 설치 확인
```bash
pkg-config --modversion opencv4
```

### !!설치 후 해야할 것, 주의할 점!!

Ubuntu 22.04에서 OpenCV 4.11.0을 자동으로 설치하는 스크립트입니다. OpenCV와 관련된 ROS humble용 cv_bridge, 빌드용 ament_cmake를 재설치해줘야 합니다. 아래 코드는 복붙 X
```
sudo apt-get purge opencv* -y
sudo apt-get purge libopencv* -y
sudo apt-get autoremove -y
```

코드 내부에 기존 openCV를 삭제하는 명령어가 있음.

---

**RO:BIT 19th Beomsu Choi**

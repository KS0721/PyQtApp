# PyQtApp 만들어 보기

### QTDesigner를 다운로드 및 설치(이미지를 누르면 다운로드 페이지로 이동)

<a href="https://build-system.fman.io/qt-designer-download">
  <img src="https://github.com/user-attachments/assets/d69503d6-fcf6-491b-9776-d850729b6a45" alt="image" width="200"/>
</a>

## VScode 실행
1. 기상환경 설정
```
conda create -n pyqtapp001 python=3.9
conda activate pyqtapp001
```
2. VScode에서 QTDesigner 설치
```
pip install PyQt6
```
3.  QTDesigner를 이용해서 만든 pyqtapp.ui라는 UI 파일
  <img src="https://github.com/user-attachments/assets/12bb468b-c76a-4f84-bd7a-d63dd2405c84" alt="image" width="250"/>

4.  main.py를 만든 후 QTDesigner사이트에 있는 코드 복붙
```
from PyQt6 import uic
from PyQt6.QtWidgets import QApplication

# pyqtapp.ui는 본인이 만든 파일명 이름으로 바꾸기
Form, Window = uic.loadUiType("pyqtapp.ui")

app = QApplication([])
window = Window()
form = Form()
form.setupUi(window)
window.show()
app.exec()
```
5. 결과 화면
  <img src="https://github.com/user-attachments/assets/3deedfc7-5621-4bb3-b61f-e3ffcf7ebb2e" alt="image" width="250"/>

6. 추가 결과 화면
  <img src="https://github.com/user-attachments/assets/f9ce9d01-d72b-400e-98fd-9ea5dd35106c" alt="image1" width="250"/>
  <img src="https://github.com/user-attachments/assets/985743aa-9ac9-4a04-a262-a6e94e88bd25" alt="image2" width="250"/>





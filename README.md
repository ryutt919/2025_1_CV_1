OpenCV 기반 웹캠 녹화 및 화면 반전 프로그램

이 프로그램은 OpenCV를 사용하여 웹캠 영상을 실시간으로 출력하고, 녹화 및 좌우 반전 기능을 제공

**기능 설명**
1. **웹캠 영상 실시간 출력**
   - OpenCV의 `VideoCapture(0)`를 사용하여 웹캠을 실행하고 실시간으로 화면에 출력

2. **녹화 기능 (`R` 키)**
   - waitKey를 사용하여 `R` 키를 누르면 **녹화가 시작되며**, VideoWriter에 의해 영상이 `webcam_rec.avi` 파일로 저장
   - 녹화 중일 때는 화면에 **빨간 테두리**가 표시
   - 다시 `R` 키를 누르면 **녹화가 중지**

3. **화면 좌우 반전 기능 (`SPACE` 키)**
   - waitKey를 사용하여 `SPACE` 키를 누르면 **실시간 영상이 좌우 반전**

4. **프로그램 종료 (`ESC` 키)**
   - waitKey를 사용하여 `ESC` 키를 누르면 프로그램이 종료

5. 해당 기능들을 putText를 통해 테두리가 있는 글씨로 표시

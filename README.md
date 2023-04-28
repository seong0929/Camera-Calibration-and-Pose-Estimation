# Camera-Calibration-and-Pose-Estimation
 내 카메라를 캘리브레이션하고 간단한 AR 기법을 응용

1. chessboard녹화(주의점: (10, 7)보드판 전체가 보여야 한다.)
2. camera_calibration을 실행(주의점: chessboard와 같은 폴더에 있어야 한다.)
3. 실행 중에 space바와 enter키를 연달아서 입력한다.(동영상의 퀄리티가 떨어져 300번 반복하였습니다.)
![image](https://user-images.githubusercontent.com/50050003/235073444-746e39e3-a050-4f2e-acf6-ffaef2aee1c9.png)
4. camera_calibration의 나온 값을 pose_estimation_chessboard의 K와 dist_coeff에 입력한다.
5. pose_estimation_chessboard 실행

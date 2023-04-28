# Camera-Calibration-and-Pose-Estimation
 내 카메라를 캘리브레이션하고 간단한 AR 기법을 응용

1. chessboard녹화(주의점: (10, 7)보드판 전체가 보여야 한다.)
2. camera_calibration을 실행(주의점: chessboard와 같은 폴더에 있어야 한다.)
3. 실행 중에 space바와 enter키를 연달아서 입력한다.(동영상의 퀄리티가 떨어져 300번 반복하였습니다.)
![image](https://user-images.githubusercontent.com/50050003/235089241-60feff32-9a61-4337-b5e6-d9f2725ebe6f.png)
4. camera_calibration의 나온 값을 pose_estimation_chessboard의 K와 dist_coeff에 입력한다.
5. pose_estimation_chessboard 실행
![image](https://user-images.githubusercontent.com/50050003/235089330-ebdd4f71-b872-439a-bafa-2a659af99015.png)

아래 코드 수정으로 도형을 바꿀 수 있다.
<pre>
<code>
# Prepare a 3D star for simple AR
box_lower = board_cellsize * np.array([[3,0,0],[4,2,0],[2,4,0],[4,4,0],[5,6,0],[6,4,0],[8,4,0],[6,2,0],[7,0,0],[5,1,0]])
box_upper = board_cellsize * np.array([[3,0,-1],[4,2,-1],[2,4,-1],[4,4,-1],[5,6,-1],[6,4,-1],[8,4,-1],[6,2,-1],[7,0,-1],[5,1,-1]])
</code>
</pre>

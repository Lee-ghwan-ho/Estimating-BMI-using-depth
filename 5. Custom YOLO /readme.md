Custom YOLOv8x-pose model 
=============

# 1. 데이터 셋 구축
-------------

약 4,300장의 이미지에서 ROBOFLOW를 이용하여 24개의 주요관절 keypoint 좌표를 직접 ANNOTATION 하였다.
![roboflow](https://github.com/user-attachments/assets/2826d131-2878-4166-810f-ec51242f9783)


## 결과
![000231_F_33_162560_13607772](https://github.com/user-attachments/assets/26a94004-3d8d-416f-88dd-5216eda72e15)

5: Neck(nk), 12: Center waist(cw), 13: Left waist(lw), 14: Right waist(rw), 15: Hip(h), 18: Right hipline(rl), 19: Left hipline(ll). 추가됨


### 24개 주요관절 keypoint를 활용하여 신체학적 특징 추출 성공.
![image](https://github.com/user-attachments/assets/2108a4b2-9676-4d9c-9f14-10194f0d4f98)
------------------------------------------------------------------------------------------

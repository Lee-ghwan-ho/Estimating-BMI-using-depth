
# Depth map을 efficientnet-b7으로 학습하는 과정 

  - 1. 저체중 및 과체중 이미지 개수가 부족하기때문에, 좌우 반전을 시켜 데이터를 추가
    2. RGB 이미지와 마스크 이미지를 불러와 224로 수정 후 텐서로 변환
    3. 전체 이미지를 정규화 한후 마스크를 곱해줘 배경 제거
    4. tf_efficientnet_b7_ns 사전학습 모델을 불러오고 회귀용 Linear(2560→1) 레이어 추가
    5. 학습


---
# Depth map만을 학습한 mae 결과 
![image](https://github.com/user-attachments/assets/4f94b559-ee50-4b51-ba5c-64fe6c0401e9)
MAE : 3.0187
---

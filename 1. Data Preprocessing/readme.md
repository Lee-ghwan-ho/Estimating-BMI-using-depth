# Data Preprocessing
---
## Reddit
  1. 데이터 크롤링 ( ex: F355'11_[235lbs__146.8lbs_=_88.2lbs]_took_me_4_years_in_total_with_2_pregnancies_inbetween..png)
  2. - 이미지에서 사람수에 따라 분류
(데이터의 대부분은 운동전 후 두명으로 구성되어있지만 다른 경우도 있음. 4장이 들어있는 경우도 있어서 분류 필요)
     - " 지우기 
     -  kg, cm 애들 이동 시키기 
     - 정규 표현식으로 패턴검증
     - 패턴이 일정한 이미지는 우리 데이터셋형식 이름에 맞게 수정 (F-18-5'11-185.jpg -> 0_F_18_180340_8391452.png)
     - YOLO를 사용해 무릎과 눈이 있는 사진들만 복사
     - 오류 형식 확인
     - reddit 형식에 맞지 않는 애들은 직접 수정
     - lb,lbs 글자 삭제
     - 마지막으로 형식이 맞지 않았던애들을 잘 맞췄기때문에 우리 데이터셋 형식에 맞게 다시 이름 수정
     - ![데이터셋 전처리 이미지](https://github.com/user-attachments/assets/df25d8bf-4158-4ba9-bc00-9bbff5cc773f)

---
## korean 
  1. 사람이 있는 부분만 CROP해서 사용
  2. YOLOv8을 사용해 사람이 있는 부분만 Crop
  3. 원래 데이터셋 형식대로 이름 수정 (F0150105_F_51_1605_456 -> 0081_F_51_160500_4560000)
![그림1](https://github.com/user-attachments/assets/36467bc0-87f3-4b06-adf0-558de3f98c60)

---

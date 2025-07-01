
# depth 이미지에서 뽑아낸 2560개의 feature와 신체학적 정보를 뽑아낸애들을 잘 정리해서 합치는 과정 (train,val,test 모두)

  - 1. YOLO로 뽑아낸 json 파일을 통해 신체학적 특징 추출( Head_Widht ,Hip_Width, Waist_Width, Height ) -> train_measurements.csv , val_measurements.csv, test_measurements.csv
    2. 위와 같이 구해낸 특징들을 다시 비율로 다시 계산 (Head_Hip_Ratio, Head_Waist_Ratio, Head_Height_Ratio, Hip_Waist_Ratio, Hip_Height_Ratio, Waist_Height_Ratio) ->, test_measurements_ratio.csv
    3. 면적 비율 구하기 (knee_ratio, hip_ratio, waist_ratio, neck_ratio, waist_to_hip_ratio)
    4. 앞서구한 2560개의 feature + 2,3에서 구한 신체학적 특징 결합 (train, test)
    5. 이후 ML로 각각 예측
    6. Optuna로 머신러닝 조합을 찾음 ![image](https://github.com/user-attachments/assets/d33ceed8-8194-4000-a293-e6f831cb1816)



---
# 
![image](https://github.com/user-attachments/assets/cc20e1fc-4b0a-4c5f-a82c-8287c6e3aaaf)

---


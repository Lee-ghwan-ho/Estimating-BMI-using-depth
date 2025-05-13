


# image에서 Depth 추출  
![depth 구하기](https://github.com/user-attachments/assets/540a92e1-5bb0-4415-8c4e-a09ebf25e84e)

---
# Depth anything을 통해 Depth를 추출하였다면?
  1. _depth가 붙은 이미지 이름을 삭제해준다. (0_F_15_162560_6123497_depth ->0_F_15_162560_6123497)
  2. mask들 중 0번 이미지를 사람이 있는 mask라고 일단 뽑아낸다
  3. 다른 mask들은 수작업으로 확인후 교체해준다(mask 처리가 잘 되지 않는 경우는 데이터 삭제)

---

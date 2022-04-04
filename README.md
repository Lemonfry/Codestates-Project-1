# ds-section6-project-1
딥러닝을 이용한 독일 교통 표지판 데이터 분류

딥러닝 모델을 이용해 독일 표지판 데이터 분류를 수행하고, 국내 표지판도 분류할 수 있을지 확인하기

1. 데이터셋

* GTSRB 데이터 : https://sid.erda.dk/public/archives/daaeac0d7ce1152aea9b61d9f1e19370/published-archive.html
  1. GTSRB_Final_Training_Images(훈련용)
  2. GTSRB_Final_Test_Images(테스트용)
  3. GTSRB_Final_Test_GT(테스트 데이터의 라벨)

* 한국 도로교통공단 도로안전표지일람표 : https://www.koroad.or.kr/kp_web/safeDataView.do?board_code=DTBBS_030&board_num=100178

2. CNN 모델을 구축한 후, 원본 모델과 dropout을 적용한 모델, 증강된 데이터를 이용한 모델을 훈련

3. 예측 정확도는 0.9 이상으로 나타났으며, 독일과 국내 표지판 중 비슷한 모양이 있던 표지판은 성공적으로 분류하였습니다.

* 다음 사이트들을 참고했습니다.
  * https://github.com/chsasank/Traffic-Sign-Classification.keras
  * https://junstar92.tistory.com/114
  * https://colab.research.google.com/github/frogermcs/GTSRB-TensorFlow-Lite/blob/master/notebooks/GTSRB_TensorFlow_MobileNet.ipynb

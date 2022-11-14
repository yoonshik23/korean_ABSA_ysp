# korean_ABSA_ysp
## 1. 학습  
대회에서 제공한 데이터를 data 경로에 넣고 train.ipynb 코드를 실행.  

train.ipynb 코드는 gpu 환경에서 실행 되어야 함.  

코드가 정상 종료 되면 10개의 .pt 학습 모델이 saved_model5 경로에 생성 됨.  

## 2. 예측
2_1. train.ipynb 코드를 실행하거나 학습 완료 된 모델을 따로 saved_model5 경로에 넣어준 후 predict.ipynb 실행.  
(10개 파일의 경로, 파일명)  
saved_model5/polarity_classificationsaved_model_epoch_0.pt  
saved_model5/polarity_classificationsaved_model_epoch_1.pt  
saved_model5/polarity_classificationsaved_model_epoch_2.pt  
saved_model5/polarity_classificationsaved_model_epoch_3.pt  
saved_model5/polarity_classificationsaved_model_epoch_4.pt  
  
saved_model5/category_extractionsaved_model_epoch_0.pt  
saved_model5/category_extractionsaved_model_epoch_1.pt  
saved_model5/category_extractionsaved_model_epoch_2.pt  
saved_model5/category_extractionsaved_model_epoch_3.pt  
saved_model5/category_extractionsaved_model_epoch_4.pt  

2_2. 아래와 같이 모델 경로 변수에 코드 기준 saved_model5 폴더 경로 넣고, 뒤에 모델명 붙이는 형태로 변수 수정하기.  
category_extraction_model_path = '../saved_model5/category_extraction'  
polarity_classification_model_path = '../saved_model5/polarity_classification'  

2_3. 
predict.ipynb 코드는 cpu 환경에서 실행 가능.  

코드가 정상 종료 되면 네 개의 .pkl 파일과 한 개의 .json 파일이 saved_model5 경로에 생성 됨.  

.json 파일이 대회 제출용 test 데이터에 대한 예측 결과임.  

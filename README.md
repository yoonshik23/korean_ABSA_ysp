# korean_ABSA_ysp
## 1. 학습  
대회에서 제공한 데이터를 data 경로에 넣고 train.ipynb 코드를 실행.  

train.ipynb 코드는 gpu 환경에서 실행 되어야 함.  

코드가 정상 종료 되면 10개의 .pt 학습 모델이 saved_model5 경로에 생성 됨.  

## 2. 예측
train.ipynb 코드를 실행하거나 학습 완료 된 모델을 따로 saved_model5 경로에 넣어준 후 predict.ipynb 실행.  

predict.ipynb 코드는 cpu 환경에서 실행 가능.  

코드가 정상 종료 되면 네 개의 .pkl 파일과 한 개의 .json 파일이 saved_model5 경로에 생성 됨.  

.json 파일이 대회 제출용 test 데이터에 대한 예측 결과임.  

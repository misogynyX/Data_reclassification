# Reclassification



NLP 모델을 학습시키기 위한 데이터셋 재정비 를 목표로 하는 저장소입니다.

Reclassification article.csv for training NLP model




# 목표

------

1. NLP 모델의 목표는 input 기사가 여성문제를 다루는 기사인지(1) 아닌지(0) 구별하는 것입니다.
2. 모델을 훈련시키기 위해서는 기사 ` text`와 해당 텍스트가 여성문제를 다루는지 아닌지(0/1) 표시한 ` label ` 으로 구성된 데이터셋이 필요합니다.
3. 해당 데이터셋은 `article.csv` 를 활용합니다.
4. 필요한 작업은 `article.csv` 에서 여성문제를 다루는 기사라고 레이블링`1 ` 된 기사 중에서 여성문제를 다루고 있지 않은 기사의 label을` 0 ` 으로 고치는 것입니다.
5. index 번호를 모은 text를 공유해주시면 감사하겠습니다.


# 방법

------

1. article.csv 를 다운받아 본인의 google drive 에 저장합니다.
2. 오분류처리.ipynb 을 이용하여 오분류된 기사의 index 번호를 모아서 공유해주세요.
3. 오분류처리 대상은 `label == 1` 이고 `tags != gender` 인 기사입니다.


# 여성 문제를 다루는 기사 기준 (논의 필요)

------


```
1. 여성범죄는 여성문제로 봅니다.
2. 저출산, 고령화 문제는 여성 문제로 보지 않습니다.('저출산' 단어가 잘못된 경우이므로)
3. 단, 저출생과 여성의 경력 단절이 함께 언급될 경우 여성문제로 봅니다.(논의 필요)
4. 여성의 코르셋을 조장하는 기사는 <언론이또>가 다루지 않으므로 우선 여성문제에서 제외했습니다.
```

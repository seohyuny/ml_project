# Machine Learning Project
### 당뇨병 예측 머신러닝 분석 프로젝트 입니다.
---

INDEX. Ⅰ___Team DBDBDeep 소개___


![조서현](https://github.com/seohyuny/ml_project/assets/154740829/299c4cb0-c98b-4358-b88d-c363000d818c)
![김유진](https://github.com/seohyuny/ml_project/assets/154740829/8dd8cbe7-5bec-4098-8d37-ed0dcf6e52e9)
![이수현](https://github.com/seohyuny/ml_project/assets/154740829/fd0e5ac6-50d6-49d6-96d0-d2240eb42a89)


조서현 / 김유진 / 이수현

---

INDEX. Ⅱ___프로젝트 방향___

![프로젝트방향](https://github.com/seohyuny/ml_project/assets/151902232/eb27707c-fafa-484b-99ba-dacb9e104beb)

**당뇨의 발병 원인 분석**</br>
&nbsp;&nbsp;&nbsp; 1) 유전적 원인 </br>
&nbsp;&nbsp;&nbsp; 2) 환경적 원</br>

___Concept___

[환경적 요인(생활습관) 당뇨 예측]

- ##### 참고문헌
  - [당뇨학회]<https://www.diabetes.or.kr/general/info/info_01.php?con=2>

- ##### 프로젝트에 사용된 분석 라이브러리

## :books: skill
- Programming <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white">
- Framework <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white">
- Tools <img src="https://img.shields.io/badge/jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white"> <img src="https://img.shields.io/badge/visualstudiocode-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white">
- Git <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=jupyter&logoColor=white"> <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">

```
import pandas
import numpy
import sklearn
import streamlit
import joblib
import wordcloud
```

--- 

___Process___

- ##### DataSets
  - [NHIS_2018] <https://www.cdc.gov/nchs/nhis/nhis_2018_data_release.htm>
  - Sample Adult file : samadult.csv, familyxx.csv

- ##### 분석 변수
[NHIS_2018](https://www.cdc.gov/nchs/nhis/nhis_2018_data_release.htm)

```
# 당뇨병 분석 변수 선정
import pandas as pd
df_a = pd.read_csv('samadult.csv')
df_a = df_a[['SEX','AGE_P','R_MARITL','DIBEV1','HYPEV','PREGNOW','DEP_2','AFLHCA18','BMI',
            'AFLHC29_','AFLHC31_','AFLHC32_','AFLHC33_','SMKEV','ALC1YR','CHLEV','VIGNO',
            'AUSUALPL','ASICNHC','HIT1A']]
```

![diabetes_age_count3](https://github.com/seohyuny/ml_project/assets/154740829/5b359a1c-bb3d-46e0-82bd-c98868b64571) ![cholesterol](https://github.com/seohyuny/ml_project/assets/154740829/84c3562f-3262-44bd-a775-1c0cd0ebbba2)


![diabetes_age_sex](https://github.com/seohyuny/ml_project/assets/154740829/1b8c6494-6fd8-42c6-ad52-510920ad11b3)




- ##### Data 전처리 (dataset 정보 및 가공)

- 사용한 colunms
![image](https://github.com/seohyuny/ml_project/assets/154740829/23c10fdf-8f9e-49fd-84d2-6eebbb2bcf6e)

- Data perprocessing

1) 기본 데이터프레임 생성
2) EDA (탐색적 데이터 분석)
3) 설문 답변 1/2로 정형화
4) null값 및 이상치 데이터 정제
5) 컬럼명 재구성
6) 스케일링 및 데이터 csv 저장

- ##### Machine-Learning (Model 정보)

1) SVC
2) Decisiontree
3) KNN
4) Adaboost
5) Naivebayes
6) Randomforest
7) XGBoost

![image](https://github.com/seohyuny/ml_project/assets/154740829/eb76dd4a-e5e5-4160-b4d5-5909615dcd2c)  ![image](https://github.com/seohyuny/ml_project/assets/154740829/47010c45-f1db-40d7-9f5c-d181a994c172)


## 최종 Model

- Adaboost


![image](https://github.com/seohyuny/ml_project/assets/154740829/27294c40-a89d-4278-a5df-8e485e6a2c67)


## 서비스화

![image](https://github.com/seohyuny/ml_project/assets/154740829/835449d1-f8f5-4977-967b-8868b5a81c97)



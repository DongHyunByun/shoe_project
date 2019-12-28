# shoe_project

2019 1학기 데이터마이닝 project

- 기간 : 2019.03.01~2019.06.30
- 내용 : 이동경로 데이터와 발크기 데이터를 이용한 발크기와 이동경로간의 상관관계 파악.
        이동경로 데이터는 "map my walk"어플을 이용하여 추출, 사용자의 발크기, 성별등의 데이터는 설문조사를 통해 획득
- 기술스택 : python, scikit learn, numpy, pandas, graphviz, pydotplus

- 폴더설명 :
  1. convert_to_csv
    - input file  : "folder"폴더 속 gpx files
    - output file : "처리후"폴더
    어플을 통해 추출한 한사람의 gpx파일들을 csv파일들로 변환한다. 시간, 고도, 경도, 위도, 신발크기, 사용자 키값 6가지가 att를 추출한다.
  2. preprocess
    - input file  : "folder"폴더 속 1~6조의 데이터
    - output file : "처리후"폴더
    각 조별로 특정 조원들의 key, 발사이즈, 이동경로, 평균이동속도를 추출.
  3. tree_for_datamining
    - input file  : man.csv, woman.csv
    남자와 여자로 분리된 전처리된 csv파일을 이용하여 의사결정나무 학습. scikit learn 모듈을 이용. graphviz를 이용하여 시각화.
   
   
   

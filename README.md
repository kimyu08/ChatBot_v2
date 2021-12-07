# ChatBot_v2 딥러닝을 활용한 의도 분석 챗봇

Test.py로 실행.

OS: Window
UI: Python tkinter
Algorithm: Levenshtein Distance(편집거리), KoNLPy(Komoran 형태소분석), CNN (의도분석)
Library: Tensorflow(Keras 머신러닝)
IDE: Microsoft Visual Studio

채팅 형식의 사용자의 의도를 분석하여 주문.


 흐름 및 설명
 
  1. 의도분석 모델 생성 (의도에 맞는 문자들을 만들어 데이터 셋으로 사용)
  
  2. 편집거리 알고리즘를 활용하여 메뉴에 대한 오탈자를 수정하여 개체명 인식을 좀더 효율적으로 가능하게 바꿔준다.
  
  3. 오탈자 수정된 문장을 형태소 분석을 진행. 불필요한 조사 제거
  
  4. 형태소 분석 후 형태소들을 의도분석 모델을 이용하여 의도 분석.
  
  5. 4개의 의도(포장, 배달, 주문, 알수없음) 분류 점수 중 가장 값이 높은 것을 의도로 선정

  6. 필요한 개체명(메뉴, 수량) 등을 파악하여 출력




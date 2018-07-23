### 20180709 TWL : GitHub 정적 블로그 저장소, Kaggle 소개



- #### Git / GitHub / Git bash 관련 사항 정리

  - Fork → Clone → 수정 작업 → Add → Commit → Push 개념 복습

  - git push -f : 강제로 pust 진행

  - git pull --rebase : GitHub → Local PC 소스 복사. 현재 작업중인 소스 Merge. 변경이력 기록 X.

  - 터미널 명령어를 사용하는 이유

    - 대용량 데이터를 다룰 시 원격 서버(ex. AWS)에서 직접 작업
    - 해당 원격 서버에 소스트리가 없다면 터미널 명령어를 사용해야 함

    

- #### GitHub에 정적 블로그 저장소 만들기

  - Ruby

    - Python과 흡사한 구조의, 일본에서 개발한 언어
    - Python vs. Ruby : 무엇이 더 좋은가?  → 유저들의 논쟁 거리
    - 웹 언어로는 많이 사용되나, 데이터 분야에서는 Python이 더 많이 사용됨
    - Ruby를 설치하는 이유 
      1. 정적 블로그 관리할 때 Local PC에서 수정 내역을 확인해보기 위함
      2. Jekyll(지킬)을 사용해서 다양한 기능을 활용하기 위함 (지킬이 루비로 만들어짐) 

  - 블로그를 위한 환경 셋팅

    - GitHub에 저장소 만들기 & 테마 선택하기
    - Ruby (언어), Atom (편집기), Sourcetree (버전 관리) 설치
    - GitHub Web → Local PC : Clone

  - Jekyll 설치

    - Ruby, Ruby Devkit 설치

    - 윈도우 CMD 실행

    - 다음의 명령어를 순서대로 입력

      ~~~
      cd C:\							  # C 드라이브로 이동
      mkdir jekyll				       # jekyll 폴더 생성
      cd jekyll						  # jekyll 폴더로 이동
      gem install jekyll				   # gem을 이용하여 jekyll을 설치
      gem install minima	 			   # minima 설치
      gem install tzinfo-data			   # 필요한 gem 설치
      gem install jekyll-feed		        # 필요한 gem 설치
      gem install bundler		    	   # 필요한 gem 설치
      jekyll new . 		     		   # 사이트 생성 (끝에 콜론('.') 누락 없도록 주의!)
      bundle exec jekyll serve --watch	# 사이트 구동
      ~~~

    - IE (또는 Chrome) 에서 127.0.0.1:4000 으로 접속

  - 사이트 내용 설정

    - Local PC 상에서 원하는 Theme 파일 적용
    - _config.yml 파일 수정
    - Jekyll 서버 정지 (Ctrl + C) 및 재 구동 (Jekyll serve --watch) : 수정 내역 반영 여부 확인
    - GitHub WEB Repository로 Add → Commit → Push : 수정 내역의 WEB 반영 여부 확인

  - 참고 사이트

    ~~~
    https://www.youtube.com/watch?v=qWrcgHwSG8M
    https://blog.psangwoo.com/coding/2017/04/02/install-jekyll-on-windows.html
    http://namhoon.kim/139
    ~~~

    

- #### Kaggle 소개

  - Kaggle : 개발자에게 GitHub이 있다면 데이터 사이언티스트에게는 Kaggle이 있음

  - Titanic : Kaggle 입문용 경진대회. 타이타닉호 사망자 통계 분석.

  - Kaggle Tutorial, Kernel을 참조해서 데이터 분석 방법을 익히자.

  - 1일 1 Commit 할 소재가 없다면 Kaggle Competition의 다른 사람 것을 따라해보자.

  - 캐글러의 관심사는 무엇일까? 

    - Kaggle Survey 2017 결과를 파이썬으로 분석한 커널 확인

      ~~~
      Survey : https://www.kaggle.com/kaggle/kaggle-survey-2017
      Survey Kernel : https://www.kaggle.com/ash316/novice-to-grandmaster
      Python 분석 : https://colab.research.google.com/drive/10SuqOyUNbDDlYOQQqueMTlkNqrX7BjlS
      ~~~

    - 앞으로 크게 주목받을 것은? TensorFlow. Deep Learning. 

    - 데이터 사이언스를 어디서 공부하는가? Kaggle. 온라인 강의. Stack Overflow 등.

    - 어떻게 학습하는 것이 유용한가? Project. 코스 수강. Stack Overflow. Kaggle 등.

    - 좋은 컴퓨터가 필요한가? 그렇지는 않음. 딥러닝은 Cloud service 사용하면 됨.

    - 블로그 / 팟캐스트 추천 : KDnuggets Blog. Becoming a Data Scientist. Siraj Raval.

    - 인터넷 강의 사이트 추천 : Coursera, Udacity, Edwith(Coursera Machine Learning 분석 중!)

    - 어떤 기술이 필요할까? 파이썬. 통계 지식. 시각화. SQL.

    - Data Science로 Job을 구할 때 고려 요소는? 배울수 있는 직장인지, 사용하는 언어가 무엇인지 등.

    - Job을 구할 때 필요 요소는? 관련 직무 경험, Kaggle 참여 경험, GitHub 포트폴리오 등.

  - 참고

    ~~~
    - 지도학습 : 특정 상황별로 결과값이 분류된 데이터를 가지고 진행하는 방법
    - 비지도학습 : 분류되지 않은 데이터를 가지고 진행. 클러스터링 등을 통해 직접 분류해야 함.
    ~~~



- #### 숙제

  - TWL
  - Tutorial 정리 : A, C, D, G 조 (순서대로 월, 화, 목, 금)
  - 아나콘다 설치 + jupyterlab 설치
  - Kaggle Survey 2017 데이터 셋 다운로드 받아서 아나콘다에서 실행

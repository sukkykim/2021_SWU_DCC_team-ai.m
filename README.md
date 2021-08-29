# 2021_SWU_DCC_team-ai.m
2021년 서울여자대학교 데이터청년캠퍼스 team ai.m (산학 협력 프로젝트)

oneclick_code.ipynb

<generate face - face shifter - GPEN> 과정을 모두 담은 코드
아래 코드를 각각 따로 실행한 것을 하나의 코드로 정리한 것(같은 내용 - 자동화)
코드 실행 : 런타임 유형 변경 후 실행(환경에 따라 학습 속도가 차이 날 수 있음)
런타임 유형 : GPU(colab pro 이용)
generateface_with_styleGAN.ipynb
**
styleGAN2를 이용하여 가상 인물을 생성**
최종적으로 51개의 데이터로 이틀 학습시킨 이미지의 퍼포먼스가 가장 좋았다
코드 실행 : 런타임 유형 변경 후 실행(환경에 따라 학습 속도가 차이 날 수 있음)
런타임 유형 : GPU(colab pro 이용)
face_swapping.ipynb

**face swapping을 이용하여 생성 얼굴을 상품 이미지 속 얼굴로 대체 : 대체 방법01**
맨 처음에 사용한 대체 기법. 여러가지 이슈가 있어 해결 중 face shifter로 대체 기법 변경
코드 실행 : 런타임 유형 변경 후 실행
런타임 유형 : GPU
face_shifter.ipynb

**face shifter를 이용하여 생성 얼굴을 상품 이미지 속 얼굴로 대체 : 대체 방법02**
최종 사용 결정한 대체 기법
face swapping의 발전형으로, 뛰어난 퍼포먼스 결과를 보여 최종 사용하기로 결정
코드 실행 : 런타임 유형 변경 후 실행(코드 내 google mount가 있음)
런타임 유형 : GPU
GPEN.ipynb

**GPEN을 이용하여 대체한 이미지를 고화질로 변경**
face shifter로 이미지 대체 후 화질이 저하되는 이슈 발견 > 이를 해결하기 위해 얼굴 부위만 국한하여 복원 처리하는 GPEN 사용
추가로, 대체 결과에 이목구비의 이상(눈, 코 등이 겹치는 현상)이 있을 시 한차례 blur 처리한 후 GPEN 사용
해당 코드는 블러 처리를 제외한 얼굴 부위만 국한하여 복원 처리(GPEN)하는 코드
코드 실행 : 런타임 유형 변경 후 실행
런타임 유형 : GPU
facedetection_with_v2.ipynb

**mobilenet_v2를 이용하여 사측으로부터 제공받은 데이터를 얼굴 유무로 분류**
여러 얼굴 감지 기법의 비교를 통해 최종 사용하고자 한 분류 기법
높은 퍼포먼스르 보여(해당 내용 발표 자료 참고) 1. 이미지 crop 2. 70% 이상 감지 이미지 만 선택하여 얼굴 분류
코드 실행 : 런터임 유형 변경 후 실행(코드 내 google mount가 있음)
런타임 유형 : GPU
styleCLIP.ipynb

**styleCLIP을 이용하여 얼굴 변형 : 변형 방법01**
제공하고자 하는 서비스의 추가 기법(변형용)
코드 실행 : 런타임 유형 변경 후 실행
런타임 유형 : GPU
beautyGAN.ipynb

**beautyGAN을 이용하여 얼굴 변형 : 변형 방법02**
제공하고자 하는 서비스의 추가 기법(변형용)
코드 실행 : 런타임 유형 변경 후 실행
런타임 유형 : GPU

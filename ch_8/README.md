## 8_02
### 박스모델
가로- 부모 요소의 크기만큼 자동으로 늘어남
세로 - 콘텐츠 크기만큼 늘어남

+ width 
+ height
  + 기본값 auto : 브라우저가 너비를 계산
  + 단위 : px em vw 등 단위로 지정

### 요소가 커질 수 있는 최대 가로/ 세로 너비
+ max-height  
+ max-width 
  + 기본 값 none : 최대 너비 제한 없음
  + 단위 : px em vw 등 단위로 지정
+ min-height  
+ min-width
  + 기본 값 0 : 단위 적지 않아도 됌
  + 단위 : px em vw 등 단위로 지정

## 8_03

### px 픽셀
### % 상대적 백분율
### em 요소의 글꼴 크기
요소의 글꼴 크기 기준
### rem 루트 요소의 글꼴 크기 
html 요소의 글꼴 크기 기준
### vw 뷰포트 가로 너비의 백분율
### vh 뷰포트 세로 너비의 백분율

% 0px과 0vw 0em등은 모두 같은 값이므로 0이라고 단위 없이 작성하자

## 8_04

### margin 외부 여백 
단축 속성
0px 위아래좌우
0px 0px 위아래,좌우
0px 0px 0px 위,좌우,아래
0px 0px 0px 0px 위, 우, 아래, 좌(시계방향)
+ auto 
+ 0
+ 음수 값 가능

## 8_05
### padding 내부 여백
내부 여백이 생기면 요소 전체의 크기가 늘어남
단축 속성
0px 위아래좌우
0px 0px 위아래,좌우
0px 0px 0px 위,좌우,아래
0px 0px 0px 0px 위, 우, 아래, 좌(시계방향)
+ auto 
+ 0 : 내부 여백 없음
+ 단위 : px em vw 등 단위로 지정
+ % 부모 요소의 가로 너비에 대한 비율로 지정


## 8_06
### border 
요소의 테두리 선을 지정하는 단축 속성

속성-순서는 상관없으나 아래처럼 속성하자
위 아래 좌 우 각각 따로 속성 지정 가능
  위아래좌우
  위아래,좌우
  위,좌우,아래
  위, 우, 아래, 좌(시계방향)

+ 선 두께 border-width 
+ 선종류 border-style
  none
  solid 실선
  dashed 파선
  등등
+ 선색상 border-color
  기본값 : 블랙
  
  % 색상 표현 방법
  1. 색상 이름
  2. hex 색상코드 #숫자
  3. RGB 빛의 삼원색 rgb()
  4. RGBA 빛의 삼원색 + 투명도 rgba()

## 8_07
### border-radius
요소 테두리 둥글게 깍는 속성
특정 모서리만 깍을 수 있음
+ 기본값 0
+ 단위 : px em vw 등 단위로 지정

## 8_08
### box-sizing 크기 계산
box-sizing:content-box;
+ 기본 값 content-box : 요소의 내용으로 크기 계산/ 내용은 그대로 유지 되기 때문에 padding과 border까지 합한 크기만큼 요소 크기 전체 늘어남
+  border-box : 요소의 내용+padding+border를 다 합쳐 요소의 내용으로 봄


## 8_09
### overflow
요소가 넘쳤을때
+ 기본값 visible : 그대로 보여주기
+ hidden : 넘치는 부분 제거
+ auto : 넘치는 부분있는 쪽에 스크롤 생성. 없으면 생기지 않음
+ scroll : 넘치는 부분이 있든 없든 무조건 스크롤 만듦
+ overflow-x
+ overflow-y

## 8_10
### display
요소의 화면출력 특성
+ block 상자요소
+ inline 글자 요소
+ lnline-block 글자요소 + 상자요소
+ flex 플렉스 박스 1차원 레이아웃
+ grid 그리그 2차원 레이아웃
+ none 화면에서 사라짐
+ 기타

## 8_11
### opcity
요소의 투명도
+ 기본값 1: 불투명= 투명도 없음
+ 0: 투명

## 8_12 
### 글꼴

#### font-style
+ normal : 기울기 없음
+ italic : 이텔릭체
+ oblique : 기울어진 글자
  
#### font-weight
+ normal 400 : 기본 두께
+ bold 700 : 두껍게
+ 100~900 : 100단위의 숫자 9개

#### font-size
+ 16px : 기본 크기
+ 단위 : px em rem 등 단위로 지정

#### line-height
한 줄의 높이/행간과 유사
+ (권장)숫자 : 요소의 글꼴 크기의 배수로 지정
+ 단위 : px em rem 등 단위로 지정
#### font-family
글자의 서체 지정
여러 개의 서체를 후보로 등록할 수 있음(쉼표로 구분)
사용 가능한 글꼴을 브라우저가 고르게됨. 후보가 모두 안되면 글꼴 계열 중에 하나를 고르게 됨
글꼴 계열을 필수로 작성해야함
+ serif : 바탕체 계열
+ sans-serif : 고딕체 계열
+ monospace : 고정너비 글꼴 계열
+ cursive : 필기체 계열
+ fantasy : 장식 글꼴 계열

## 8_13
### 문자
+ color : 글자의 색상
  기본값 : rgb(0,0,0) 검정색
+ text-align
  + (기본 값) left
  + center
  + right
  + justify
+ text-decoration 문자의 장식(선)
  + (기본 값) none 장식 없음
  + underline 밑줄
  + overline 윗줄
  + line-through 중앙 선

## 8_14
### 배경
+ background-color 요소의 배경 색상 
  + (기본 값)transparent 투명

+ background-image 요소의 배경이미지 삽입
  + : url("경로");

+ background-repeat
  + (기본 값)repeat 이미지를 수직 수평반복
  + repeat-x 이미지를 수평반복
  + repeat-y 이미지를 수직반복
  + no-repeat; 이미지 반복 없음
+ background-position 요소의 배경 이미지 위치
  + 방향 : 위, 아래, 좌, 우, 중앙
  + 단위 : px em rem 등 단위로 지정
+ background-size 요소의 배경 이미지 크기
  + (기본 값)auto : 이미지의 실제 크기
  + cover 비율을 유지, 요소의 더 넓은 너비에 맞춤
  + contain 비율을 유지, 요소의 더 짧은 너비에 맞춤
+ background-attachment 요소의 배경 이미지 스크롤 특성
  + (기본 값)scroll 이미지가 요소를 따라 같이 스크롤
  + fixed 이미지가 뷰포트에 고정. 스크롤 없음
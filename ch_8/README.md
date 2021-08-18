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

## 8_15
### 배치

#### 속성
position
: 요소의 위치 지정 기준
#### 값
+ static : 기본 값
+ relative : 요소 자신을 기준
+ absolute : **위치상** 부모 요소를 기준
+ fixed : 뷰포트 기준
+ sticky : 스크롤 영역 기준

% relative를 자신을 기준으로 해서 위치를 지정하지 않음
% 본인 자리였던 위치가 텅 빈 채로 남아있게 되는데 이는 오류나 마찬가지임

## 8_16
### 요소 쌓임 순서 (stack order)
어떤 요소가 사용자와 더 가깝게 있는지(위에 쌓이는지) 결정. 사용자가 봤을때 어떤 요소가 가장 앞에 있는지

1. 요소에 position 값이 있는 경우 위에 쌓임(기본값 static이 있으면 제외)
2. 1번 조건이 같으면, z-index 속성의 숫자 값이 높을 수록 위에 쌓임
3. 1,2번 조건까지 같은 경우, HTML의 다음 구조일 수록 위에 쌓임

## 8_17
#### 속성
z-index
: 요소의 쌓임 정도를 지정
#### 값
+ auto : 기본 값 = 0 : 부모 요소와 동일한 쌓임 정도
+ 숫자 : 숫자가 높을 수록 위에 쌓임 (매우 큰 숫자 입력 지양)

% position 속성의 값으로 absolute, fixed가 지정된 요소는 display 속성이 block으로 변경된다.

## 8_18
#### 속성
플렉스(정렬) flex
: 1차원 레이아웃을 설정
: x축, y축 정렬

+ display:flex;를 부여한 요소
: flex container
+ display:flex;를 부여한 요소의 자식 요소
: flex items

#### flex container에 부여 가능한 속성

+ display
컨테이너의 화면 출력 특성  
  값
  + flex : 블록요소와 같이 컨테이너 정의
  + inline-flex  : 인라인 요소와 같이 컨테이너 정의


+ flex-direction
  주 축을 설정 (수평정렬인지,수직정렬인지)
  주축을 바꾸면 다른 속성 값들도 전부 뒤집히기 때문에 잘 안 씀
  
  값
  + row : (기본 값) 행 축 (좌->우)
  + row-reverse 행 축 (우->좌)
  + column 열 축 (위->아래)
  + column-reverse 열 축 ( 아래->위)


+ flex-wrap
  줄 바꿈 처리 여부/ 줄 바꿈 처리가 없으면 요소들이 꾸역꾸역 한 줄에 다 들어가려고 함 / 줄바꿈 처리가 있으면 다음 줄에 요소들이 들어감
  값
  + nowrap : (기본 값) 묶음 없음
  + wrap : 여러 줄 묶음


+ flex-flow
+ justify-content
  flex-direction로 설정한 주축의 정렬 방법(주축을 바꾸지 않고 주로 수평 정렬 할 때 사용됨)
  값
  + flex-start : (기본 값)flex items을 시작점으로 정렬(왼쪽정렬)
  + flex-end : flex items을 끝점으로 정렬 (오른쪽 정렬)
  + center : flex items을 가운데 정렬

+ align-content
  교차 축의 **여러 줄** 정렬 방법 (주로 수직 정렬 할 때 사용) / 여러 줄이기 때문에 flex-wrap:wrap이여야 함 / 두 줄 이상일 때만 적용됌-그래서 잘 안 씀
  값
  + stretch (기본값) : flex items을 시작점으로 정렬
  + flex-start : (기본 값)flex items을 시작점으로 정렬
  + flex-end : flex items을 끝점으로 정렬
  + center : flex items을 가운데 정렬


+ align-items
교차 축의 **한 줄** 정렬 방법
  값
  + stretch (기본값) : flex items을 교차축으로 늘림
  + flex-start : (기본 값)flex items을 시작점으로 정렬
  + flex-end : flex items을 끝점으로 정렬
  + center : flex items을 가운데 정렬
  
#### flex items에 부여 가능한 속성

+ order
  flex 아이템의 순서
  값
  + 0 : ( 기본값) 순서 없음
  + 숫자 : 숫자가 작을 수록 먼저 
  
+ flex


+ flex-grow
  flex items의 증가 비율
  값
  + 0 :(기본 값) 증가 비율 없음
  + 숫자 : 증가 비율


+ flex-shrink
  flex 아이템의 감소 비율
  값
  + 1 :(기본 값) 증가 비율 없음
  + 숫자 : 감소 비율

% 개발자 도구를 실제로 보면 요소가 1:1:2의 사이즈를 갖지 않음. 이는 요소의 내용부분의 크기가 제작각이기 때문.
이를 해결하고자 하면 요소의 내용의 너비를 0으로 해주면 됨(flex-basis로 해결)

+ flex-basis
  flex items의 공간 배분 전 기본 너비
  값

  + auto : (기본 값)요소의 content너비
  + 단위 : px, em, rem 등 단위로 지정
+ align-self

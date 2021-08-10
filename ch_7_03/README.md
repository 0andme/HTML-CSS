### 선택자 종류
- 기본
  + 전체 선택자  *
  + 태그 선택자 **ABC**
  + 클래스 선택자 **.ABC**
  + ID 선택자 **#ABC**
- 복합
  + 일치 선택자 **ABCXYZ** : 선택자 ABC와 XYZ두 개를 동시에 만족하는 요소 선택
  + 자식 선택자 **ABC>XYZ**: 선택자 ABC의 자식요소 XYZ 선택
  + 하위 선택자 **ABC XYZ** : 선택자 ABC의 하위 요소 XYZ 선택
  + 인접 형제 선택자 **ABC+XYZ** : 선택자 ABC의 다음 형제 요소 XYZ **하나**를 선택
  + 일반 형제 선택자 **ABC~XYZ** : 선택자 ABC의 다음 형제 요소 XYZ **모두**를 선택
- 가상클래스
- : 어떠한 행동을 했을 때의 동작
  + : hover
  + : active
  + : focus
  + : first-child
  + : last-child
  + : nth-child(n)
  + : not(XYZ)
- 가상 요소
  + ::before
  + ::after
- 속성
  + [ ABC ] : 속성 ABC를 포함한 요소 선택
  + [ ABC = "XYZ"] : 속성 ABC를 포함하고 값으로 XYZ인 요소 선택

# DA36-mini1-quick-doctor

## 팀 : NCT 247 
![](https://velog.velcdn.com/images/ae__0519/post/8feb5d43-b1c5-4ee0-a4c6-3da45d2520f5/image.png)

## 프로젝트 이름 : Quick Doc (빠르게 의사를 만날 수 있다.)
병원 키오스크 : 병원에서 셀프로 접수와 수납이 가능한 키오스크 구현 

## 사용자 요구사항 명세서
#### 접수
1. 사용자는 접수 버튼을 누르면 환자 정보 입력하는 메뉴를 볼 수 있어야 합니다.
2. 사용자는 환자 정보(이름, 주민번호, 전화번호)를 입력할 수 있어야 합니다.
3. 사용자는 환자 정보 입력 후 진료 과목(내과/이비인후과/소아과) 선택 창을 볼 수 있어야 합니다.
4. 진료 과목 선택 후 담당의(각 과목당 2명)를 선택할 수 있어야 합니다.
5. 사용자는 모든 선택 끝난 후 접수 내역(이름, 주민번호, 전화번호, 진료 과목, 담당의)를 확인할 수 있습니다. 
6. 마지막으로 환자의 예약 번호를 확인 할 수 있습니다.

#### 수납
1. 사용자는 수납버튼을 누르면 예약번호를 입력하는 창을 볼 수 있습니다.
2. 예약번호 입력 후 진료내역을 확인 할 수 있습니다.
3. 진료내역을 확인 한 후 결제창으로 이동합니다. (카드/ 현금)
4. 결제 후 영수증과 처방전(환자정보/ 진료날짜/ 진료내역) 발급창을 확인 할 수 있습니다.

## 회의
![](https://velog.velcdn.com/images/ae__0519/post/bfefeb15-13f7-4cbd-a1f3-31df695b5da9/image.png 

## 코드진행
**2024.09.30**
모듈(3가지) : patient, department, admin

#### 수정1
 진료과목과 담당의사는 사용자가 입력한 값이 아니라, 우리가 지정한 값 dictionary 형태로 저장 및 출력
 ![](https://velog.velcdn.com/images/ae__0519/post/d48781c6-c6ac-4787-801d-19a8e7dfcb2c/image.png)

 #### 수정2
하나의 모듈로 재정리 : consultation
![](https://velog.velcdn.com/images/ae__0519/post/f7a7102b-ba79-4a7b-b9b7-2985a1158b3e/image.png)


**2024.10.01 - 2024.10.03**
#### 오류발생1
사용자가 입력한 정보, 선택한 진료과목, 담당의사가 출력이 안되는 상황

#### 오류발생2
![](https://velog.velcdn.com/images/ae__0519/post/f83e5cfe-8a9f-47f6-96b2-d7520eed4f34/image.png)
당시 접수 조회시 하나씩 밀려서 출력이 되는 오류 발생
코드 진행 시 잘못 기입으로 일어난 비교적 간단한 오류로 마무리

#### 관리자 페이지
admin 페이지 추가 및 정리(민하님)

#### 오류발생3
1. txt 파일로 저장자체가 안됨
2. txt 파일로 불러오는데 객체 주소만 출력되고 내용이 출력 안됨.
![](https://velog.velcdn.com/images/ae__0519/post/086158cb-1aa0-4adf-82ee-9ba4e3632c5e/image.jpg)

해결
1. 파일의 상대경로 말고 절대경로 이용하기
2. txt 파일을 정리된채로 부르기 위해 strip(), split도 사용

## 문서 정리 마무리
**기획안 및 WBS 템플릿 마무리
**![](https://velog.velcdn.com/images/ae__0519/post/14850567-6ec1-4300-b509-afb512743602/image.png)

**PPT 계획서**
![](https://velog.velcdn.com/images/ae__0519/post/9321f7e7-f9d3-4518-ba46-a1f06261dc6a/image.png)

**PPT 일부**
![](https://velog.velcdn.com/images/ae__0519/post/21af2f50-d4ae-4463-aeb6-2dd8952b622e/image.png)


**시연영상**
https://youtu.be/r2Bs4C5yWr8?si=8NCJT0YvKWjb5xFE

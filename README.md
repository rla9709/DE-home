# DE:home 
> 아래의 글을 누르면 해당 홈페이지로 이동합니다. <br>
> <a href="https://www.mydehome.com/dehome/main/mainpage">디홈으로 이동</a>


# Description
## 프로젝트명 : 디홈(DE:home)

> 그린 컴퓨터 아카데미 자바 과정 이수 하면서 만든 두번째 팀 프로젝트입니다.

<strong>1팀 구성</strong><br>
팀장 : 김경윤(본인)<br>
팀원 : 박소은<br>
팀원 : 김준형<br>
팀원 : 권연진<br>
팀원 : 이동현<br>

## 개발기간
2021/06/01 ~ 2021/07/04(33일)

## 프로젝트의 목적<br>
### MZ세대를 중심으로 중고거래는 하나의 문화로 자리잡고 있습니다.<br>
### 그와 더불어 코로나로 인해 세상은 많은 것이 변했습니다.<br>
### '집콕'이라는 단어는 요즘 하나의 콘텐츠로 자리 잡았습니다.<br><br>

### 인테리어와 중고거래를 합쳐 인테리어 제품을 중고로 거래하고,<br>
### 실제 인테리어 업체와 연결될 수 있는 <br>
### 종합 플랫폼 웹을 개발 해보았습니다.<br><br><br>


## 사용된 기술 스택

### 프레임워크
<img src="https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=Spring&logoColor=white"/>&nbsp; 
### 언어
<img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=Java&logoColor=white"/>&nbsp; 
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=JavaScript&logoColor=white"/>&nbsp;
### 관련 기술
<img src="https://img.shields.io/badge/JQuery-0769AD?style=flat-square&logo=JQuery&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=HTML5&logoColor=white"/>&nbsp; 
<img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=CSS3#&logoColor=white"/>&nbsp; 
<img src="https://img.shields.io/badge/bootstrap-7952B3?style=flat-square&logo=bootstrap&logoColor=white">
### DB
<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white"/>&nbsp;
### 배포
<img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=AmazonAWS&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/Ubuntu-E95420?style=flat-square&logo=Ubuntu&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/Tomcat-F8DC75?style=flat-square&logo=ApacheTomcat&logoColor=white"/>&nbsp;
<br><br><br>

## 홈페이지메인화면
![image](https://user-images.githubusercontent.com/74701876/125226183-8aef0e00-e30b-11eb-8b1f-b8307b2db358.png)
<br><br><br>

## 데이터베이스 ERD(ERDCloud로 작성)
![erd](https://user-images.githubusercontent.com/74701876/125284062-f78dfb00-e353-11eb-83ea-0fc0e30e179b.png)


<br><br><br>
## 내가 수행한 작업
> <b>회원가입</b> - 회원가입, 로그인, 아이디 찾기, 비밀번호 찾기, 카카오/네이버 로그인(RestAPI), 이메일인증번호 전송기능 구현<br>
> <b>중고거래</b> - 중고거래(등록, 수정, 삭제, 더보기버튼 AJAX 사용), 1 대 1 채팅기능(AJAX)<br> 
> <b>ERD<b> - ERDCloud로 ERD 제작<br>
> <b>배포</b> - AWS ubuntu서버 배포(EC2, RDS, ACM)<br>
<br><hr>

# 내가 수행한 작업 설명

  
## 회원가입/로그인 상세
> - 회원가입 : 이메일 인증
> - 로그인 : 카카오/네이버 소셜 로그인
> - 아이디 찾기, 비밀번호 찾기

 
### 회원가입 화면

![회원가입 화면](https://user-images.githubusercontent.com/74701876/125241271-360cc100-e326-11eb-9de7-97e75aadead4.png)
![image](https://user-images.githubusercontent.com/74701876/125241416-5dfc2480-e326-11eb-90c9-08837fa9b7f3.png)
![image](https://user-images.githubusercontent.com/74701876/125241471-71a78b00-e326-11eb-8ccb-9457522b3f6b.png)
 
- 회원 가입시 필요한 정보 입력
- 닉네임, 아이디는 중복검사 필수
- 각 항목별 유효성 검사 후 회원가입

### 회원가입 이메일 인증 - AJAX, SMTP

> AWS배포할 경우 SMTP 25번 포트사용이 제한 되기 때문에 이메일 인증 로직은 돌아가지만 실제로 전송은 되지않아서<br>
> 로컬에서는 가능하지만 실제 배포된 사이트에서는 이메일 인증 기능은 제외시켜놨습니다.

<br><br>
<img src="https://user-images.githubusercontent.com/74701876/125241615-a287c000-e326-11eb-8078-3e52ca8547f8.jpg" width="550"  height="310" />
<img src="https://user-images.githubusercontent.com/74701876/125241649-ae738200-e326-11eb-8241-563e4872dacb.jpg" width="550"  height="310" />
<img src="https://user-images.githubusercontent.com/74701876/125241693-bcc19e00-e326-11eb-8421-e88489e9ded5.jpg" width="550"  height="310" />
<img src="https://user-images.githubusercontent.com/74701876/125241731-c64b0600-e326-11eb-88e6-2537cfd2f6b7.jpg" width="550"  height="310" />
<br><br>
#### - 이메일을 입력하고 전송하면 이메일을 보냈다고 알림 확인
#### - 3분의 카운트가 시작되고 3분이 지나면 시간초과로 재전송 
#### - 입력한 이메일계정으로 들어가서 인증번호 6자리 확인
#### - 인증번호 6자리 입력 후 인증번호가 일치한다는 표시가 input박스 아래에 표시됩니다.(틀릴 경우 틀렸다고 표시)

<br><br>
### 로그인 - RestAPI, AJAX 

> 일반로그인<br>
> 카카오<br>
> 네이버

  <br>
  
![image](https://user-images.githubusercontent.com/74701876/125241797-dbc03000-e326-11eb-9851-e6b0c00556fd.png)
<img src="https://user-images.githubusercontent.com/74701876/125245778-ed580680-e32b-11eb-84e8-2f211e689232.png" width="500" height="340" />
<img src="https://user-images.githubusercontent.com/74701876/125246241-838c2c80-e32c-11eb-9d24-3eb69ba474c6.png" width="500" height="340" />
<img src="https://user-images.githubusercontent.com/74701876/125245852-06f94e00-e32c-11eb-837c-9321d2b9ef61.png" />
<img src="https://user-images.githubusercontent.com/74701876/125246203-6e170280-e32c-11eb-8fb9-60cf19c6bdd9.png" width="500" height="340"/>

<br><br>
>  카카오/네이버 로그인일 경우
> - 카카오 OR 네이버 로그인 클릭
> - 카카오/네이버 아이디로 로그인 -> 홈페이지 정보제공 동의 창
> - 동의 하면 헤더 상단 추가정보 등록 출력
> - 추가정보 등록을 완료하면 서비스 이용가능

> 일반 로그인일 경우
> - 회원가입한 아이디/비밀번호 입력
> - 로그인 후 서비스 이용 가능

<hr>

## 중고거래

### 중고거래 상세
> - 중고거래 메인 : 지역별, 카테고리별 물건 확인
> - 중고물품 등록
> - 중고물품 상세 
> > 구매자 : 관심 등록, 구매 채팅<br>
> > 판매자 : 등록된 물품 수정, 삭제
> - 1 대 1 실시간 채팅(AJAX)
> - 대화목록 실시간 확인

<hr>


### 중고거래 메인화면

![image](https://user-images.githubusercontent.com/74701876/125278507-cca0a880-e34d-11eb-943a-fdf070c76abb.png)

#### 상단 헤더 카테고리별 또는 중고거래 선택시 들어옴
#### 최근에 올린 순서대로 화면에 출력
#### 지역검색시 해당 지역 거래 목록 출력
#### 물품별 제목, 동네, 가격, 관심 눌러진 갯수 출력(트리거로 하트 누를때 마다 컬럼 1씩 증가 처리)
#### 거래완료 될  경우 목록에서 사라짐
<br><br>

### 중고거래 상품등록

![내상품등록](https://user-images.githubusercontent.com/74701876/125279125-84ce5100-e34e-11eb-8080-bd3ec6a94041.png)

#### 제목, 내용, 물건 사진, 가격 작성
#### 가격은 직접작성과 무료나눔으로 나눔
<br><br>

### 중고거래 메인 더보기 페이징

![image](https://user-images.githubusercontent.com/74701876/125279321-c5c66580-e34e-11eb-918f-1c9ee772f5f8.png) 

#### 최초 9개의 물품 출력, 더보기버튼 클릭시 3개씩 더 출력됨
#### AJAX로 더보기 페이징 구현
<br><br>

### 중고거래 물품 상세보기

![image](https://user-images.githubusercontent.com/74701876/125279367-d545ae80-e34e-11eb-8f66-e8b60e921c59.png)

- 판매자
> 조회수 증가 X<br>
> 작성한 글 수정, 삭제 버튼 출현<br>


- 구매자
> 조회수 증가 O(쿠키로 한 게시물 상세페이지 입장시 최초 1회에만 1증가)<br>
> 채팅으로 거래하기 버튼 출현


<br><br>

### 판매자, 거래자 1대1 채팅(AJAX)

![image](https://user-images.githubusercontent.com/74701876/125279733-3f5e5380-e34f-11eb-81a9-65e61576792f.png)
  
#### 판매자와 거래자는 제품을 교환하기 위해 대화 가능<br>
#### AJAX를 활용한 실시간 채팅<br><br>
> 판매를 할 경우 구매자와의 대화방에서 판매확정을 지을수 있음

<br><br>

### 대화 목록
  ![image](https://user-images.githubusercontent.com/74701876/125280645-40dc4b80-e350-11eb-9239-878f7bf7c29d.png)
  
  #### 판매 목록과 구매 목록에 관한 대화방이 구분되어 있음
  #### 판매 완료가 됐을 경우 판매완료 표시로 변경

## AWS 배포
<br><br>
EC2 인스턴스를 사용해서 무료버전으로 배포<br><br>
데이터베이스는 RDS에 저장<br><br>
Decorate Home을 줄여서 DE:home이라고 부르기로 했지만 도메인이 남아있질 않아서 mydehome을 선택<br>
<br><br>

## 마무리

  
  
#### 여러가지 기능을 도입해서 넣어보았고 많이 배울 수 있는 프로젝트였다.
#### AWS로 배포하면서 ubuntu도 써보고 리눅스 명령어도 처음 써봤다.

  
  
### 아쉬운점
- Spring Security를 사용해서 좀더 보안성이 좋은 프로그램을 만들고 싶다.
- AWS를 사용해서 배포하기는 했지만 아직 이해했다고 보기는 힘들것 같다.
- 사진 파일은 S3에 저장하고 싶었는데 시간부족과 지식의 부족함으로 FTP를 사용해서 ubuntu 가상 서버에 만든 폴더에 넣을 수 밖에 없는게 아쉬움.
- 시간이 부족해서 조금더 완벽한 프로그래밍을 못한게 아쉽다.







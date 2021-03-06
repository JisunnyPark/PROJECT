# PROJECT_PORTFOLIO : JISEON PARK
>안녕하세요 <br>
>비트캠프 교육 기관에서 진행했던 <br>
>최종 3차 팀 프로젝트 기술서입니다. <br>

# Description
* 프로젝트 명 : 국내 레저 여행 상품 예약 사이트 - 베스트립 'Bestrip'
* 내  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 용 :
  Spring를 이용한 웹 사이트 제작 프로젝트
* 참 여 &nbsp; 인 원 : 5명

* 개 발 &nbsp; 기 간 : 2021.06.24 ~ 2021.07.13 (약 3주)
* 사 용 &nbsp; 기 술
  * Spring 4.3.16, MyBatis, BootStrap
  * Java8(1.8), JSP, Apache Tomcat 9.0
  * HTML, CSS, Java Script, JQuery, GitHub
  * Oracle SQL 20.4.1.407
* 담 당 &nbsp; 업 무 
  * 커뮤니티 게시판 기능 구현
    * 게시글, 댓글 CRUD, 페이징, 검색, 조회수, 이미지 파일 화면 출력, 로그인 조건 처리
  * UI 구현 
    * 게시판 네비게이션 바, 메인 메뉴 헤더, 로그인, 회원가입
  * 팀 회의록 작성 및 관리
  * DB ERD, PPT 설계(발표 자료 관리)
 
 # View 
 * 메인 메뉴 헤더
 <img src = "https://user-images.githubusercontent.com/79893752/124296933-7b4a2980-db95-11eb-926e-44298fb1fd8a.png" width="100%">

 * 로그인
 <img src = "https://user-images.githubusercontent.com/79893752/124294739-00800f00-db93-11eb-92e2-dcf4891875fa.png" width="100%">
     
 * 커뮤니티 게시판
 <img src = "https://user-images.githubusercontent.com/79893752/124298047-c3b61700-db96-11eb-862a-8a9c2ddac19c.png" width="100%">

# Implementation
>커뮤니티 (자유, 여행 정보 게시판)
 * 로그인 조건 처리 - 로그인 했을 경우에만 글, 댓글 쓰는 버튼 생성
<div>
   <img src = "https://user-images.githubusercontent.com/79893752/124351025-f7467f00-dc32-11eb-8c7a-dc5c8cd98dd2.png" width="45%" height="250px">
   <img src = "https://user-images.githubusercontent.com/79893752/124350887-2c9e9d00-dc32-11eb-8bdc-a6b9f73f6d3a.png" width="50%" height="250px">
</div>
<div>
<img src = "https://user-images.githubusercontent.com/79893752/124307641-14cc0800-dba3-11eb-8756-9f3c3d84eb3a.png" width="45%" height="300px">
<img src = "https://user-images.githubusercontent.com/79893752/124350577-5a82e200-dc30-11eb-87cd-7b5b3e53f4c2.png" width="50%" height = "100px">
</div>

---

* CRUD (글 작성) - View(JSP)로 부터 사용자 입력 정보를 받아 Controller로 전송하여 글 등록 처리 
<div>
<img src = "https://user-images.githubusercontent.com/79893752/124308538-5e692280-dba4-11eb-9a55-699d18d62bd0.png" 
     width="45%" height="300px">
<img src = "https://user-images.githubusercontent.com/79893752/124351712-f6175100-dc36-11eb-86bb-822d76ffd521.png"                   width="50%" height="300px">
</div>
 
 ---
 
* CRUD (글 상세 보기) - 로컬에서 이미지 파일 화면 출력 (등록 Controller로 부터 업로드한 이미지를 View에서 불러오기)
<div>
<img src = "https://user-images.githubusercontent.com/79893752/124353053-fd425d00-dc3e-11eb-9233-899112d295de.png" 
width="40%" height="350px">
<img src = "https://user-images.githubusercontent.com/79893752/124353165-df292c80-dc3f-11eb-9c2e-a1e3c4b6d3c4.png" 
width="58%" height="350px">
</div>
<img src = "https://user-images.githubusercontent.com/79893752/124353283-99209880-dc40-11eb-874d-6670e3160e45.png" 
width="100%">

* CRUD (글 상세 보기) - 조회수 증가 (update문을 통해 게시글을 클릭하면 조회수 1씩 증가 되도록 처리)
<div>
<img src = "https://user-images.githubusercontent.com/79893752/124353569-4516b380-dc42-11eb-86d0-5adcc7ba702b.png" 
width="40%" height="200px">
<img src = "https://user-images.githubusercontent.com/79893752/124353690-f4538a80-dc42-11eb-8661-ebc39d39cbde.png" 
width="55%" height="200px">
</div>

<hr>
* CRUD (글 수정/삭제) - 본인이 작성한 글만 수정, 삭제할 수 있도록 View에서 조건 설정
<div>
<img src = "https://user-images.githubusercontent.com/79893752/124309364-915fe600-dba5-11eb-9c88-5e9cbc7bb807.png" width="45%">
<img src = "https://user-images.githubusercontent.com/79893752/124357352-fa9f3200-dc55-11eb-94c5-1db2cb7022a7.png" width="50%"> 
</div>

---
 
* CRUD (댓글 작성) - @RequestParam을 사용하여 게시글 번호 참조하여 댓글 작성 처리
<div>
<img src = "https://user-images.githubusercontent.com/79893752/124353945-755f5180-dc44-11eb-94e9-2a121d3a0a47.png" width="40%">
<img src = "https://user-images.githubusercontent.com/79893752/124354036-ef8fd600-dc44-11eb-9ed9-f07e15a79aab.png" width="55%" height="200px">
</div>
<img src = "https://user-images.githubusercontent.com/79893752/124353980-a0e23c00-dc44-11eb-90c0-c33c0ca7fb28.png" width="100%">
 
---

* CRUD (댓글 수정) - window 함수 사용하여 댓글 수정 창 열고 댓글 수정 작업 처리
<div>
<img src = "https://user-images.githubusercontent.com/79893752/124354168-a0967080-dc45-11eb-9740-3f29d9e91c0c.png" width="50%">
<img src = "https://user-images.githubusercontent.com/79893752/124354222-f10dce00-dc45-11eb-8b02-cc38be81ae52.png" width="45%">
</div>

---

* 페이징 및 검색 처리 - Criteria, PageMaker 파일 생성하여, Controller에서 값을 받고 View로 전송하며 기능 구현
<div>
<img src = "https://user-images.githubusercontent.com/79893752/124357921-e14bb500-dc58-11eb-81a5-326c0c07763c.png" width="50%" height="350px">
<img src = "https://user-images.githubusercontent.com/79893752/124357580-3be41180-dc57-11eb-9579-b36903fda6f9.png" width="40%" height="350px">
</div>
<img src = "https://user-images.githubusercontent.com/79893752/124358594-fa099a00-dc5b-11eb-8f2f-e419a7753f82.png" width="90%" height="200px">
<div>
<img src = "https://user-images.githubusercontent.com/79893752/124358801-e448a480-dc5c-11eb-8f5b-f180e43ea8b9.png" 
width="50%" height="450px">
<img src = "https://user-images.githubusercontent.com/79893752/124358922-84063280-dc5d-11eb-8f38-4d6737ea3d71.png" width="48%" height="300px">
</div>

# 요구 사항 관리 대장
* 커뮤니티 게시판
 <img src = "https://user-images.githubusercontent.com/79893752/124299754-c154bc80-db98-11eb-92ae-47946fa26a3e.png" width="100%">

# ERD 
* 커뮤니티 게시판
 <img src = "https://user-images.githubusercontent.com/79893752/124300728-d2ea9400-db99-11eb-87b0-31735f7d7802.png" width="100%">
 
 # 스토리 보드
 * 커뮤니티 게시판
 <img src = "https://user-images.githubusercontent.com/79893752/124301381-b569fa00-db9a-11eb-863f-ec937938d46d.png" width="100%">

  # 프로젝트 기술서
  * 3차 프로젝트 - 2021.06.24 ~ 2021.07.13 (약 3주)
  <img src = "https://user-images.githubusercontent.com/79893752/124350422-a41efd00-dc2f-11eb-8d1d-d74b4f03bf56.png" width="100%">
  
  * 2차 프로젝트 - 2021.06.04 ~ 2021.06.13 (2주)
  <img src = "https://user-images.githubusercontent.com/79893752/124350205-3920f680-dc2e-11eb-86f7-f68790347e74.png" width="100%">

  * 1차 프로젝트 - 2021.04.29 ~ 2021.05.06 (1주)
  <img src = "https://user-images.githubusercontent.com/79893752/124350220-58b81f00-dc2e-11eb-8876-bb9d9c578103.png" width="100%">




  
  
 


 

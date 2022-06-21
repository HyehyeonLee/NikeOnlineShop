# 나이키 온라인 쇼핑몰 사이트 (jsp, servlet)
개발 환경 : java 1.8.0, eclipse, MySQL 8.0.21, window 10, apache-tomcat-8.5.57 <br />
개발 기간 : 2020.09.02 ~ 2020.09.11 <br />
개발 인원 : 4명(김태립, 이혜현, 진영웅, 추주헌)<br />
참고 사이트 : https://www.nike.com/kr/ko_kr/ (한국 나이키 온라인 스토어) <br />
PPT : https://url.kr/5aq2ye (google drive link) PPT 미리보기🔽 <br />

## 1. 개요
MVC model 2 기반으로 한 Servlet & JSP 쇼핑몰<br />
나이키로 선택한 이유 - 나이키는 대중적인 브랜드로, 온라인 스토어 사이트 또한 남녀노소를 위한 사이트로 제작되었다고 생각하여 벤치마킹 시 실력 향상에 도움이 될 것이라도 판단했습니다.

## 2. 역할 분담
<ul>
  <li>김태립 : 검색 기능, 고객 센터, 장바구니</li>
  <li>이혜현 : 상품 관리, 매출 현황 조회, 프론트엔드</li>
  <li>진영웅 : 상품 관리, 아이디·비밀번호 찾기, 구매 목록</li>
  <li>추주헌 : 로그인 및 회원 가입, 게시판, 회원 정보 조회, 상품 정렬, 장바구니</li>
</ul>

## 3. DB 설계
Table : product, order, member, bulletinboard, cart, service

## 4. 기능 설명
### 4-1. 사용자 기능
<ul>
  <li>회원 가입, 로그인, 아이디·비밀번호 찾기</li>
  <li>상품 목록 페이지 : 카테고리 별로 DB에 저장 돼 있는 상품 정보를 화면에 나오도록 구현, <br />
    상품을 신상품순, 높은 가격순, 낮은 가격순으로 정렬할 수 있는 정렬 기능 구현
  </li>
  <li>상품 상세 설명 페이지 : 사이즈, 수량을 선택할 수 있도록 JS로 구현</li>
  <li>장바구니 기능 : 상품 수량 수정, 상품 삭제 기능, 상품 일부 선택 기능 구현</li>
  <li>구매 기능, 구매 목록 페이지 : 구매하기 버튼을 클릭 시 구매 완료 페이지로 이동, 구매 목록과 총 지출을 보여줌</li>
  <li>검색 기능 : 상품의 키워드 입력 시 검색 가능</li>
  <li>고객 센터 : 공지 사항 등 게시판</li>
  <li>매장 안내 : google 지도 api를 이용하여 가까운 나이키 매장을 검색할 수 있도록 함</li>
  <li>게시판 : 나이키 회원만 작성할 수 있는 게시판, 계층형 게시판으로 구현, 파일 첨부 기능 구현</li>
</ul>

### 4-2. 관리자 기능
관리자 id로 로그인 시 관리자 페이지 접속 가능
<ul>
  <li>회원 정보 조회, 구매 목록 조회 : 회원 정보와 회원의 구매 목록 조회 가능</li>
  <li>상품 추가 : 상품을 추가, 삭제, 수정할 수 있음</li>
  <li>월별 매출 현황 : 월별 매출 현황을 볼 수 있는 그래프를 chart.js로 구현</li>
  <li>기간 별 매출 현황 : 기간 별 매출을 판매 수량이 높은 상품 순서대로 조회할 수 있도록 구현</li>
</ul>

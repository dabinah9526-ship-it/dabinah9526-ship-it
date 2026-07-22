<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:6C63FF,50:E094A3,100:FCE1E8&height=220&section=header&text=DABIN%20LEE&fontSize=48&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=BACKEND%20DEVELOPER&descAlignY=58&descSize=17" />

<div align="center">

안녕하세요, 이다빈입니다 👋

Java와 Spring Boot를 중심으로 서버 개발을 공부하고 있습니다.기능이 실행되는 것에서 끝내지 않고, 권한과 데이터가 맞게 처리되는지 직접 확인합니다.



</div>

한눈에 보기

프로젝트

구분

담당

주요 기술

바로가기

K-STEP

개인

기획·DB·서버·화면 연동

React, Express, Oracle

Repository

UNIPET

팀

쇼핑몰·커뮤니티

Spring Boot, MyBatis, MySQL

Repository

따iT

팀·진행 중

스터디·커뮤니티

Flutter, Firebase

Repository

Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=java,spring,mysql,nodejs,express,react,vue,flutter,dart,firebase,git,github&perline=6" />

</div>

구분

기술

프로젝트에서 사용한 내용

Backend

Java, Spring Boot, MyBatis

UNIPET의 상품·게시판 서버 로직과 SQL 연동

Backend

Node.js, Express

K-STEP REST API와 인증·피드·채팅·알림 처리

Database

Oracle, MySQL

테이블 설계, JOIN, CRUD, 트랜잭션 처리

Frontend

React, Vue.js, JSP, JavaScript

API 응답을 화면에 연동하고 사용자 상태에 따라 UI 처리

Mobile

Flutter, Dart

따iT의 스터디·채팅·커뮤니티 화면과 기능 개발

Cloud DB

Firebase Auth, Firestore, Storage

로그인 사용자 확인, 실시간 데이터, 이미지·파일 업로드

Collaboration

Git, GitHub

기능 브랜치, 커밋, Push, Pull Request 협업

구현 프로젝트

<details open>
<summary><b>✈️ K-STEP — 한국 여행 SNS 개인 프로젝트</b></summary>

<br>

한국 여행 사진과 장소, 이동 루트를 함께 기록하고 공유하는 SNS입니다.

항목

내용

기간

2026.05.27 ~ 2026.06.09

인원

1명

역할

기획, DB 설계, API, 화면 구현, 테스트

기술

React, Node.js, Express, Oracle, JWT, bcrypt, Multer

규모

Oracle 테이블 22개, Express API 라우트 68개

직접 구현한 기능

회원·인증

회원가입 및 로그인

JWT 기반 사용자 인증

bcrypt 비밀번호 암호화

아이디·닉네임 중복 확인

아이디 및 비밀번호 찾기

프로필 조회·수정

비공개 계정 설정

사용자 차단 및 차단 해제

여행 피드

피드 작성·수정·삭제·상세 조회

최대 10장의 이미지 업로드

지역·카테고리·해시태그 검색

여행 장소와 이동 순서 저장

팔로우한 사용자 피드 조회

비공개 계정·팔로우·차단 관계에 따른 조회 제한

사용자 소통

댓글 작성·수정·삭제

좋아요와 여행 루트 저장·취소

팔로우·팔로우 취소

비공개 계정의 팔로우 요청 수락·거절

댓글·좋아요·팔로우 알림

스토리·채팅

스토리 등록·조회·삭제

본 스토리와 보지 않은 스토리 구분

스토리 조회자 목록

채팅방 생성 및 메시지 전송

나에게만 삭제·모두에게 삭제

사용자 접속 상태 확인

서버에서 신경 쓴 부분

피드·이미지·여행 장소를 같은 DB 커넥션에서 저장

전체 작업 성공 시 commit, 오류 발생 시 rollback

사용한 Oracle 커넥션을 finally에서 반환

비공개 계정, 팔로우, 차단 여부를 서버에서 검증

로그인 사용자에 따라 좋아요·저장 상태를 함께 응답

코드 바로 보기

Express API

React 화면

Oracle DB 백업

프로젝트 README

</details>

<br>

<details>
<summary><b>🐾 UNIPET — 반려동물 통합 플랫폼 팀 프로젝트</b></summary>

<br>

반려동물 쇼핑, 커뮤니티, 병원·미용실·호텔링 예약 기능을 제공하는 웹 서비스입니다.

항목

내용

기간

2026.04.09 ~ 2026.04.30, 이후 유지보수

인원

5명

담당

쇼핑몰, 커뮤니티

기술

Java, Spring Boot, MyBatis, MySQL, JSP, jQuery, JavaScript

직접 구현한 기능

쇼핑몰

상품 목록과 상세 페이지

카테고리·가격·추천 대상 필터

최신순·가격순·리뷰순·평점순 정렬

장바구니 상품 추가·수량 변경·삭제

상품 찜 등록·해제

상품평 작성·수정·삭제

이미지 상품평 슬라이드

작성자와 관리자 권한에 따른 버튼 구분

커뮤니티

통합·지역 게시판 목록과 상세 조회

게시글 작성·수정·삭제

카테고리, 지역, 검색, 정렬, 페이징

공지사항·비공개 글·임시저장

게시글 첨부파일

댓글 작성·수정·삭제

게시글 추천·신고·알림

관리자와 일반회원 권한 구분

개선한 기능

금칙어 필터링

정확히 일치하는 단어만 걸러지던 문제 확인

공백·특수문자를 포함한 표현도 찾도록 정규식 적용

게시글 제목·본문·댓글에서 공통 메서드 사용

금칙어 목록을 BAD_WORD 테이블로 이동

MyBatis로 사용 상태가 활성화된 단어만 조회

권한 처리

공지사항은 관리자만 작성·삭제하도록 제한

상품평은 작성자만 수정·삭제할 수 있도록 처리

관리자는 상품평 삭제만 가능하도록 구분

화면의 버튼 조건과 서버 권한 검사를 함께 수정

코드와 작업 내역 바로 보기

프로젝트 전체

상품 관련 화면

커뮤니티 화면

MyBatis SQL

이다빈 커밋 내역

</details>

<br>

<details>
<summary><b>📚 따iT — 자격증 학습 관리 Flutter 팀 프로젝트</b></summary>

<br>

자격증 일정 관리, 스터디, 커뮤니티 기능을 제공하는 모바일 앱입니다.

항목

내용

상태

개발 진행 중

담당

스터디, 커뮤니티

기술

Flutter, Dart, Firebase Auth, Firestore, Firebase Storage

협업

기능 브랜치 개발 및 Pull Request

직접 구현한 기능

스터디 생성·참여

스터디 목록 실시간 조회

모집 상태·공개 여부·키워드 필터

스터디 생성·수정·상세 조회

목표 시험일과 모집 인원 설정

공개·비공개 스터디 구분

즉시 참여와 승인 후 참여 방식 구분

참여 신청 수락·거절

그룹 관리

방장·매니저·일반회원 권한 구분

그룹원 목록과 공부 시간 순위

회원 초대

그룹원 신고·추방

스터디 나가기

하위 컬렉션을 포함한 스터디 삭제

공부 관리

일반 타이머와 포모도로 타이머

시작·일시정지·재시작·종료

과목 추가·수정·삭제

과목별·일자별 공부 시간 저장

오늘 공부 시간과 누적 기록

앱 이탈 횟수를 이용한 집중 점수

시험일까지의 D-Day와 목표 달성률

스터디원 공부 시간 순위

그룹 채팅·퀴즈

실시간 그룹 채팅

답장할 메시지 선택

방장 공지 작성

사진·파일 업로드

업로드 진행률 표시

OX·객관식·주관식 문제 등록

문제 전송과 답안 확인

커뮤니티

게시판 종류별 게시글 조회

Firestore 실시간 목록과 상세 조회

게시글 작성·수정·삭제

문서를 지우지 않는 소프트 삭제

제목·내용·작성자 검색

자격증 태그 필터

최신순·조회순·좋아요순·댓글순 정렬

인기 게시글 분리

로그인 사용자만 작성·수정하도록 처리

코드와 작업 내역 바로 보기

스터디 코드

커뮤니티 코드

이다빈 커밋 내역

프로젝트 전체

</details>

Troubleshooting

<details>
<summary><b>K-STEP — 여러 테이블의 저장 결과가 어긋날 수 있는 문제</b></summary>

<br>

피드 등록 시 기본 내용은 FEED, 이미지는 FEED_IMAGE, 여행 장소는 ROUTE_SPOT 테이블에 저장됩니다. 저장 작업을 하나의 Oracle 커넥션에서 처리하고 모두 성공했을 때만 commit했습니다. 오류가 발생하면 전체 작업을 rollback해 피드와 첨부 정보가 서로 어긋나지 않도록 했습니다.

</details>

<details>
<summary><b>UNIPET — 공백과 특수문자로 금칙어 필터를 피하는 문제</b></summary>

<br>

금칙어 사이에 공백이나 특수문자를 넣으면 필터를 통과하는 문제를 확인했습니다. 글자 사이의 공백·특수문자를 인식하도록 정규식을 적용하고, 게시글과 댓글에서 같은 공통 메서드를 사용하도록 수정했습니다. 금칙어는 DB에서 추가하거나 사용 여부를 변경할 수 있게 했습니다.

</details>

<details>
<summary><b>따iT — 타이머 화면의 잦은 갱신과 시간 표시 문제</b></summary>

<br>

타이머가 동작할 때 화면 전체가 자주 다시 그려지며 버벅이는 부분과 초·분 표시가 맞지 않는 문제를 확인했습니다. 화면 갱신 범위를 줄이고 초 단위 내부 값과 사용자에게 보여주는 시간 형식을 나누어 처리했습니다. 타이머 종료 시에는 공부 기록과 누적 시간을 Firestore에 저장하도록 연결했습니다.

</details>

About Me

<details>
<summary><b>개발을 시작하기 전 경험 보기</b></summary>

<br>

러시아에서 고등학교와 대학교 졸업

해외 법인 운영 및 경영지원 경험

러시아어 통번역과 해외 업무 지원

한국 화장품 유통 회사 운영

외국인 환자의 입국·진료 지원 및 러시아어 의료통역

여러 업무의 처음부터 끝까지 직접 확인해 온 경험을 바탕으로, 개발에서도 화면·서버·DB가 연결되는 전체 흐름을 살펴보고 있습니다.

</details>

<div align="center">

Contact

Email · dabinah26@naver.comGitHub · dabinah9526-ship-it

</div>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:FCE1E8,50:E094A3,100:6C63FF&height=120&section=footer" />

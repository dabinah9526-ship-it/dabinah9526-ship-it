<div align="center">

# 이다빈

### Backend Developer

Java와 Spring Boot를 중심으로 서버 개발을 공부하고 있습니다.  
개인·팀 프로젝트를 진행하며 DB 설계, API 연동, 권한 처리와 오류 수정을 경험했습니다.

<br>

[![GitHub](https://img.shields.io/badge/GitHub-dabinah9526--ship--it-181717?style=flat-square&logo=github)](https://github.com/dabinah9526-ship-it)
[![Email](https://img.shields.io/badge/Email-dabinah26%40naver.com-2563EB?style=flat-square)](mailto:dabinah26@naver.com)

<br>

[Tech Stack](#tech-stack) · [Projects](#projects) · [Troubleshooting](#troubleshooting) · [About Me](#about-me) · [Contact](#contact)

</div>

---

<a id="tech-stack"></a>

## Tech Stack

| 구분 | 기술 |
|:---:|:---|
| **Backend** | ![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![MyBatis](https://img.shields.io/badge/MyBatis-000000?style=flat-square) ![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white) ![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white) |
| **Database** | ![Oracle](https://img.shields.io/badge/Oracle-F80000?style=flat-square&logo=oracle&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![Firebase](https://img.shields.io/badge/Firebase-DD2C00?style=flat-square&logo=firebase&logoColor=white) |
| **Frontend & Mobile** | ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white) ![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white) ![Dart](https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white) |
| **Tools** | ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white) |

---

<a id="projects"></a>

## Projects

아래 프로젝트 이름을 누르면 상세 내용을 확인할 수 있습니다.

| 프로젝트 | 구분 | 담당 | 주요 기술 |
|:---|:---:|:---|:---|
| **K-STEP** | 개인 프로젝트 | 기획, DB, API, 화면 연동 | React, Express, Oracle |
| **UNIPET** | 팀 프로젝트 | 쇼핑몰, 커뮤니티 | Spring Boot, MyBatis, MySQL |
| **따iT** | 팀 프로젝트 | 스터디, 커뮤니티 | Flutter, Firebase |

<br>

<details>
<summary><b>01. K-STEP | 한국 여행 SNS 개인 프로젝트</b></summary>

<br>

한국 여행 사진과 장소, 이동 루트를 기록하고 공유하는 SNS입니다.

### 프로젝트 정보

| 구분 | 내용 |
|:---|:---|
| 기간 | 2026.05.27 ~ 2026.06.09 |
| 인원 | 1명 |
| 담당 | 기획, DB 설계, API 개발, React 화면 및 서버 연동 |
| 기술 | React, Node.js, Express, Oracle, JWT, bcrypt, Multer |

### 구현 기능

| 구분 | 구현 내용 |
|:---|:---|
| **회원 및 인증** | 회원가입 및 로그인<br>JWT 기반 사용자 인증<br>bcrypt 비밀번호 암호화<br>아이디·닉네임 중복 확인<br>아이디 및 비밀번호 찾기<br>프로필 조회·수정<br>비공개 계정 설정<br>사용자 차단 및 차단 해제 |
| **여행 피드** | 피드 작성·수정·삭제<br>피드 목록 및 상세 조회<br>다중 이미지 업로드<br>지역·카테고리·해시태그 검색<br>여행 장소 및 이동 순서 저장<br>팔로우한 사용자 피드 조회<br>비공개 계정의 피드 조회 제한<br>차단한 사용자와 차단당한 사용자의 피드 제외 |
| **댓글 및 사용자 활동** | 댓글 작성·수정·삭제<br>좋아요 등록·취소<br>여행 루트 저장·취소<br>팔로우·팔로우 취소<br>비공개 계정의 팔로우 요청<br>팔로우 요청 수락·거절<br>댓글·좋아요·팔로우 알림 |
| **스토리 및 채팅** | 스토리 등록·조회·삭제<br>본 스토리와 보지 않은 스토리 구분<br>스토리 조회자 목록<br>채팅방 생성<br>메시지 전송<br>나에게만 메시지 삭제<br>모든 사용자에게 메시지 삭제<br>사용자 접속 상태 확인 |
| **서버 처리** | 피드·이미지·여행 장소를 같은 DB 커넥션에서 저장<br>전체 저장 성공 시 `commit`<br>오류 발생 시 `rollback`<br>사용한 Oracle 커넥션을 `finally`에서 반환<br>비공개·팔로우·차단 상태를 서버에서 확인<br>로그인 사용자에 따라 좋아요·저장 여부를 함께 응답 |

### 코드 보기

| 구분 | 링크 |
|:---|:---|
| Repository | [K-STEP Repository](https://github.com/dabinah9526-ship-it/react_project_kstep) |
| Backend | [Express API 코드](https://github.com/dabinah9526-ship-it/react_project_kstep/tree/main/express-back/routes) |
| Frontend | [React 화면 코드](https://github.com/dabinah9526-ship-it/react_project_kstep/tree/main/react-front/src) |
| Database | [Oracle DB 파일](https://github.com/dabinah9526-ship-it/react_project_kstep/tree/main/kstep_db_backup) |

</details>

<br>

<details>
<summary><b>02. UNIPET | 반려동물 통합 플랫폼 팀 프로젝트</b></summary>

<br>

반려동물 쇼핑, 커뮤니티, 병원·미용실·호텔링 예약 기능을 제공하는 웹 서비스입니다.

### 프로젝트 정보

| 구분 | 내용 |
|:---|:---|
| 기간 | 2026.04.09 ~ 2026.04.30 |
| 인원 | 5명 |
| 담당 | 쇼핑몰, 커뮤니티 |
| 기술 | Java, Spring Boot, MyBatis, MySQL, JSP, jQuery, JavaScript |

### 구현 기능

| 구분 | 구현 내용 |
|:---|:---|
| **쇼핑몰** | 상품 목록 및 상세 페이지<br>상품 카테고리 필터<br>가격 및 추천 대상 필터<br>최신순·가격순·리뷰순·평점순 정렬<br>장바구니 상품 추가·수량 변경·삭제<br>상품 찜 등록·해제<br>상품평 작성·수정·삭제<br>이미지 상품평 슬라이드<br>작성자와 관리자에 따른 버튼 권한 구분 |
| **커뮤니티** | 통합·지역 게시판<br>게시글 목록 및 상세 조회<br>게시글 작성·수정·삭제<br>게시판 카테고리 및 지역 필터<br>게시글 검색·정렬·페이징<br>공지사항<br>비공개 게시글<br>게시글 임시저장<br>게시글 첨부파일<br>댓글 작성·수정·삭제<br>게시글 추천·신고·알림 |
| **금칙어 필터 개선** | 정확히 일치하는 단어만 걸러지던 문제 확인<br>공백과 특수문자가 포함된 표현도 찾도록 정규식 적용<br>게시글 제목·본문·댓글에 공통 필터 적용<br>금칙어 목록을 `BAD_WORD` 테이블로 이동<br>MyBatis를 통해 활성화된 금칙어만 조회<br>코드 수정 없이 DB에서 금칙어 추가 및 사용 여부 관리 |
| **회원 권한 처리** | 공지사항은 관리자만 작성·삭제<br>일반회원 화면에서 공지 작성 버튼 숨김<br>상품평 작성자만 수정·삭제 가능<br>관리자는 상품평 삭제만 가능<br>화면의 버튼 조건과 서버 권한 조건을 함께 수정 |

### 코드 및 커밋 보기

| 구분 | 링크 |
|:---|:---|
| Repository | [UNIPET Repository](https://github.com/Medo-skb/Unipet) |
| 상품 | [상품 화면 코드](https://github.com/Medo-skb/Unipet/tree/main/unipet/src/main/webapp/WEB-INF/product) |
| 커뮤니티 | [커뮤니티 화면 코드](https://github.com/Medo-skb/Unipet/tree/main/unipet/src/main/webapp/WEB-INF/board) |
| Database | [MyBatis SQL 코드](https://github.com/Medo-skb/Unipet/tree/main/unipet/src/main/resources/mybatis-mapper) |

</details>

<br>

<details>
<summary><b>03. 따iT | 자격증 학습 관리 Flutter 팀 프로젝트</b></summary>

<br>

자격증 일정 관리와 스터디, 커뮤니티 기능을 제공하는 모바일 앱입니다.

### 프로젝트 정보

| 구분 | 내용 |
|:---|:---|
| 상태 | 개발 진행 중 |
| 담당 | 스터디, 커뮤니티 |
| 기술 | Flutter, Dart, Firebase Auth, Firestore, Firebase Storage |
| 협업 | 기능 브랜치 개발 및 Pull Request |

### 구현 기능

| 구분 | 구현 내용 |
|:---|:---|
| **스터디 생성 및 참여** | 스터디 목록 실시간 조회<br>모집 상태별 필터<br>공개·비공개 스터디 구분<br>키워드 검색<br>스터디 생성·수정<br>스터디 상세 조회<br>목표 시험일 및 모집 인원 설정<br>즉시 참여와 승인 후 참여 구분<br>참여 신청 수락·거절 |
| **그룹 관리** | 방장·매니저·일반회원 권한 구분<br>그룹원 목록<br>공부 시간 순위<br>회원 초대<br>그룹원 신고<br>그룹원 추방<br>스터디 나가기<br>스터디 삭제<br>관련 하위 컬렉션 삭제 |
| **공부 기록** | 일반 타이머<br>포모도로 타이머<br>시작·일시정지·재시작·종료<br>과목 추가·수정·삭제<br>과목별 공부 시간 저장<br>일자별 공부 기록 저장<br>오늘 공부 시간 표시<br>누적 공부 시간 표시<br>앱 이탈 횟수를 이용한 집중 점수<br>시험일까지의 D-Day<br>목표 공부 시간 달성률<br>스터디원 공부 시간 순위 |
| **그룹 채팅 및 문제** | 실시간 그룹 채팅<br>작성자와 전송 시간 표시<br>메시지 답장<br>방장 공지 작성<br>사진 업로드<br>파일 업로드<br>업로드 진행률 표시<br>OX 문제 등록<br>객관식·주관식 문제 등록<br>문제 전송 및 답안 확인 |
| **커뮤니티** | 게시판 종류별 게시글 조회<br>Firestore 실시간 목록 조회<br>게시글 상세 조회<br>게시글 작성·수정·삭제<br>문서를 완전히 지우지 않는 상태 변경 방식의 삭제<br>제목·내용·작성자 검색<br>자격증 태그 필터<br>최신순·조회순·좋아요순·댓글순 정렬<br>인기 게시글 표시<br>로그인 사용자 확인<br>작성자에 따른 수정·삭제 권한 처리 |

### 코드 및 커밋 보기

| 구분 | 링크 |
|:---|:---|
| Repository | [따iT Repository](https://github.com/4288-yerim/flutterteam03) |
| 스터디 | [스터디 코드](https://github.com/4288-yerim/flutterteam03/tree/dev/lib/study) |
| 커뮤니티 | [커뮤니티 코드](https://github.com/4288-yerim/flutterteam03/tree/dev/lib/community) |

</details>

---

<a id="troubleshooting"></a>

## Troubleshooting

각 항목을 누르면 문제와 해결 내용을 확인할 수 있습니다.

<details>
<summary><b>K-STEP | 여러 테이블의 저장 결과가 어긋날 수 있는 문제</b></summary>

<br>

| 구분 | 내용 |
|:---|:---|
| 문제 | 피드 등록 시 기본 내용은 `FEED`, 이미지는 `FEED_IMAGE`, 여행 장소는 `ROUTE_SPOT` 테이블에 저장됩니다. |
| 해결 | 모든 저장 작업을 하나의 Oracle 커넥션에서 처리하고, 정상적으로 완료된 경우에만 `commit`했습니다. 중간에 오류가 발생하면 전체 작업을 `rollback`해 피드와 첨부 정보가 서로 어긋나지 않도록 처리했습니다. |

</details>

<details>
<summary><b>UNIPET | 공백과 특수문자로 금칙어 필터를 피하는 문제</b></summary>

<br>

| 구분 | 내용 |
|:---|:---|
| 문제 | 금칙어 사이에 공백이나 특수문자를 넣으면 필터를 통과하는 문제를 확인했습니다. |
| 해결 | 글자 사이의 공백과 특수문자를 인식하도록 정규식을 적용하고, 게시글 제목·본문·댓글에서 같은 공통 메서드를 사용하도록 수정했습니다. 금칙어 목록은 DB에서 관리하도록 변경했습니다. |

</details>

<details>
<summary><b>따iT | 타이머 버벅임과 시간 표시 문제</b></summary>

<br>

| 구분 | 내용 |
|:---|:---|
| 문제 | 타이머 실행 중 화면이 자주 갱신되면서 버벅이고, 초와 분이 맞지 않게 표시되는 문제를 확인했습니다. |
| 해결 | 화면의 갱신 범위를 줄이고 내부에서 사용하는 초 단위 값과 사용자에게 보여주는 시간 형식을 나누어 처리했습니다. 타이머 종료 후에는 공부 기록과 누적 시간을 Firestore에 저장하도록 연결했습니다. |

</details>

---

<a id="about-me"></a>

## About Me

<details>
<summary><b>개발을 시작하기 전 경험</b></summary>

<br>

| 경험 |
|:---|
| 러시아에서 고등학교와 대학교 졸업 |
| 해외 법인 운영 및 경영지원 |
| 러시아어 통번역 및 해외 업무 지원 |
| 한국 화장품 유통 회사 운영 |
| 외국인 환자 입국·진료 지원 |
| 러시아어 의료통역 |

개발 전에는 여러 업무의 처음부터 끝까지 직접 확인하고 처리했습니다.  
이 경험을 바탕으로 개발에서도 화면, 서버와 DB가 연결되는 전체 흐름을 확인하고 있습니다.

</details>

---

<a id="contact"></a>

<div align="center">

## Contact

**Email**  
[dabinah26@naver.com](mailto:dabinah26@naver.com)

**GitHub**  
[dabinah9526-ship-it](https://github.com/dabinah9526-ship-it)

</div>

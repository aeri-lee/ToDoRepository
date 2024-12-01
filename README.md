# 하루 일정 관리 "My Day" 프로젝트
- 프로젝트 기간 : 2024.11.25 ~ 2024.12.01
- 참여 인원 : 1인(혼자 진행)
<br />

## 프로젝트 소개
- 사용자가 자신의 할 일 목록을 관리할 수 있는 웹 애플리케이션입니다.
- 사용자는 할 일을 추가하고, 수정하고, 완료 여부를 체크하는 등 기본적인 할 일 관리 기능을 제공합니다.
- 깔끔한 코드 작성, 데이터베이스 관리, 사용자 인터페이스 설계에 중점을 두고 개발되었습니다.
<br />

## 개발 환경
- 백엔드 : java, Spring Framework, eGovFramework, MyBatis, JSP, JSTL
- 프론트엔드 : HTML, CSS, JavaScript, jQuery
- DB : Oracle, DBeaver
- IDE : Eclipse
<br />

## 프로젝트 구조
- 깃허브 구조

## 프로세스 흐름도
<img height=500px width=300 src="https://github.com/user-attachments/assets/073a2038-ffb9-4c7d-896a-fb01a8686044">



## 테이블 설계
### 엔티티 관계도
 <img height=200px width=300 src="https://github.com/user-attachments/assets/b27c745e-f713-49c5-a2b9-e896888020e3">

### 테이블 정의서
 
- TB_BOARD 테이블
<table border="1" >
  <thead>
    <tr>
      <th>컬럼 이름</th>
      <th>데이터 타입</th>
      <th>제약 조건</th>
      <th>설명</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>BOARD_ID</td>
      <td>VARCHAR2(36)</td>
      <td>PRIMARY KEY</td>
      <td>고유 ID</td>
    </tr>
    <tr>
      <td>TITLE</td>
      <td>VARCHAR2(200)</td>
      <td>NOT NULL</td>
      <td>할 일 내용</td>
    </tr>
    <tr>
      <td>CNST</td>
      <td>VARCHAR2(2000)</td>
      <td></td>
      <td>할 일 상세 내용</td>
    </tr>
    <tr>
      <td>COMPLETE_YN</td>
      <td>VARCHAR2(1)</td>
      <td>DEFAULT 'N'</td>
      <td>완료 여부</td>
    </tr>
    <tr>
      <td>ID</td>
      <td>VARCHAR2(10)</td>
      <td>NOT NULL</td>
      <td>사용자 ID</td>
    </tr>
    <tr>
      <td>CREATE_DT</td>
      <td>DATE</td>
      <td></td>
      <td>생성일자</td>
    </tr>
    <tr>
      <td>UPDATE_DT</td>
      <td>DATE</td>
      <td></td>
      <td>수정 일자</td>
    </tr>
    <tr>
      <td>TODO_DATE</td>
      <td>DATE</td>
      <td>NOT NULL</td>
      <td>완료 일자</td>
    </tr>
  </tbody>
</table>

- TB_MEMBER 테이블
<table border="1" >
  <thead>
    <tr>
      <th>컬럼 이름</th>
      <th>데이터 타입</th>
      <th>제약 조건</th>
      <th>설명</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>ID</td>
      <td>VARCHAR2(10)</td>
      <td>PRIMARY KEY</td>
      <td>사용자 ID</td>
    </tr>
    <tr>
      <td>PASS</td>
      <td>VARCHAR2(100)</td>
      <td>NOT NULL</td>
      <td>사용자 비밀번호</td>
    </tr>
    <tr>
      <td>NAME</td>
      <td>VARCHAR2(50)</td>
      <td>NOT NULL</td>
      <td>이름</td>
    </tr>
    <tr>
      <td>EMAIL</td>
      <td>VARCHAR2(100)</td>
      <td>NOT NULL</td>
      <td>이메일</td>
    </tr>
    <tr>
      <td>CREATE_DT</td>
      <td>DATE</td>
      <td></td>
      <td>생성일자</td>
    </tr>
  </tbody>
</table>


<br />

# 페이지 별 기능

<br />

# 개선 목표

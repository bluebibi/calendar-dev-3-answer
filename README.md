## 프로젝트: calendar-dev
본 프로젝트는 한국기술교육대학교 컴퓨터공학부 4학년 "웹서비스컴퓨팅및실습" 수업에서 Assignment로 활용하는 프로젝트입니다. 

### Assignment 3
#### 제목: Domain 객체 및 Dao 객체 재정리 및 CalendarService 제작과 이벤트 레벨 관리 및 트랜잭션 테스트 하기
#### 기한: 2014년 10월 26일 (일요일) 23시 59분 
- calendar-dev를 pull 하여 최신 버전으로 업데이트하기
- 요구 사항 1 - Domain 객체 및 Dao 객체 재정리
  - 변경된 스키마 학습 및 DB에 반영
    - src/main/resources/database/calendar-schema.sql
  - 추가된 다음 클래스/이늄 학습 
    - EventAttendee.java
    - EventLevel.java
  - 변경된 다음 클래스 학습
    - Event.java
  - [코딩 요구 사항 1-1] JdbcEventAttendeeDao.java에 있는 //TODO Assignment 3 구현 (총 6 개)
  - [코딩 요구 사항 1-2] JdbcEventDao.java에 있는 //TODO Assignment 3 구현 (총 2 개)
  - [코딩 요구 사항 1-3] DaoJUnitTest.java에 있는 //TODO Assignment 3 구현 (총 1 개)
  - [주의 1-1] Event 클래스에서 Attendee는 별도의 클래스 EventAttendee에서 정의 
  - [주의 1-2] Event의 레벨 관리 부분 주목
- 요구 사항 2 - CalendarService 제작과 이벤트 레벨 관리 및 트랜잭션 테스트 하기
  - [코딩 요구 사항 2-1] DefaultCalendarService.java에 있는 //TODO Assignment 3 구현 (총 17 개)
  - [주의 2-1] 이벤트 레벨 관리는 교재에서 학습한 것과 로직이 거의 동일함
    - 요구 사항: 각 이벤트들은 처음에 NORMAL 레벨이지만 주기적으로 numLike가 10이상인지에 대한 조건을 확인하여 조건이 맞다면 HOT 레벨로 업그레이드 한다. 
  - [주의 2-2] CalendarServiceTest.java는 완벽하게 코딩이 되어 있음. 이곳에 존재하는 테스트를 완벽하게 성공시켜야 함
  - [주의 2-3] 5.2.4절에서 학습한 트랜잭션 관련 코드를 upgradeEventLevels() 메소드에 넣어 주어야 함

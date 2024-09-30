# 프로젝트 설명

여러 러닝 대회 일정을 표시하고, 대회에서 같이 뛸 사람을 모집하거나 러닝 동호회 회원등을 모집할 수 있는 웹서비스를 개발한다.

회원간의 소통이 가능하도록 CRUD 기능을 구현하고, 친구추가 및 실시간 채팅 기능도 도입한다.

# 개요

- 프로젝트 명칭: RunMate

- 개발인원: 1인
- 개발 기간: 2024-09-30~
- 프로젝트 핵심 기능
    - 게시판: CRUD 기능
    - 실시간 채팅: WebSocket 사용한 실시간 채팅 기능 구현
    - 회원가입 및 로그인: Security 사용한 회원가입 및 로그인 구현, OAuth 를 사용하여 여러 로그인 방법 제공.



# 요구사항 분석

## 1. 기능적 요구사항

- ### 1. 러닝 대회 등록 및 관리  
    - 운영자는 대회 이름, 일정, 장소를 입력하여 새로운 대회 정보를 입력할 수 있어야 한다.  

    - 사용자는 모든 러닝 대회 목록을 조회할 수 있어야 한다.

    - 사용자는 특정 대회를 클릭해 상세 정보를 확인할 수 있어야 한다.

<br>

- ### 2. 팀원 모집 공고

    - 사용자는 대회를 선택하고, 원하는 수의 팀원 모집 공고를 작성할 수 있어야 한다.

    - 사용자는 대회에 참여할 팀에 지원할 수 있어야 한다.
    - 사용자는 자신이 속한 팀의 모집 상태(지원자 수, 모집 마감 여부) 등을 확인할 수 있어야 한다.

<br>

- ### 3. 러닝 동호회 및 번개모임 모집

    - 사용자는 자신만의 동호회를 개설하고, 활동 지역, 시간대를 입력하며 소개 및 상세 활동 계획을 작성할 수 있어야 한다.

    - 사용자는 동호회에 가입하거나 탈퇴할 수 있어야 한다.

    - 동호회 회원들은 활동 내용을 게시판에 공유할 수 있어야 한다.

<br>

- ### 4. 회원 간 소셜 기능

    - 사용자는 다른 회원에게 친구 요청을 보낼 수 있어야 하며, 친구 요청을 수락/ 거절할 수 있어야 한다.

    - 친구 추가된 회원 간의 1:1 채팅 기능을 지원하며, 실시간으로 메시지를 주고받을 수 있어야 한다

    - //새 메시지 도착 시 사용자에게 알림을 제공해야 한다.?

<br>


- ### 5. 소통 게시판

    - 자유 게시판에는 모든 사용자가 자유롭게 글을 작성하고, 게시물을 업로드 할 수 있어야 한다.

    - 동호회 전용 게시판에는 특정 인원 이상의 동호회에 한해서 관리자가 생성하며, 동호회 회원만 게시글을 작성할 수 있다.

    - 게시판에는 댓글 및 대댓글을 작성할 수 있어야 한다.

- ### 6. 관리자 기능

    - 관리자는 모든 대회 일정을 추가, 수정, 삭제할 수 있다.
    
    - 관리자는 특정 사용자를 관리하거나 제재할 수 있어야 한다.

    - 관리자는 특정 회원에 대해 동호회장으로서 동호회 관리에 관한 권한을 넘겨줄 수 있어야 한다.

    - 관리자는 게시판의 부적절한 게시글을 삭제할 수 있어야 한다.

- ### 7. 회원가입 및 로그인

    - 사용자는 회원가입, 혹은 소셜 로그인 등을 통해 회원 가입 및 로그인을 할 수 있어야 한다.

    - 사용자는 비밀번호를 분실할 경우, 이메일을 통하여 비밀번호를 재설정 할 수 있어야 한다.

    - 사용자는 자신의 프로필을 수정할 수 있어야 한다.

    

<div align="center">

<!-- logo -->

### TeamVerse - 협업 툴 프로젝트 🛠

[<img src="https://img.shields.io/badge/-readme.md-important?style=flat&logo=google-chrome&logoColor=white" />]() [<img src="https://img.shields.io/badge/-demo video-blue?style=flat&logo=youtube&logoColor=white" />](https://www.youtube.com/watch?v=1Er1CtSh3UA&t=12s) [<img src="https://img.shields.io/badge/release-v1.0.0-yellow?style=flat&logo=google-chrome&logoColor=white" />]()  
<br/> [<img src="https://img.shields.io/badge/프로젝트 기간-2025.03~2025.04-green?style=flat&logo=&logoColor=white" />]()

</div> 

<br/>

## 📝 프로젝트 소개
**TeamVerse**는 팀 기반 프로젝트 관리, 업무(Task) 관리, 채팅 및 피드 기능을 지원하는 협업 툴입니다.  
단순한 일정 관리 툴을 넘어, 실제 협업 환경에서 필요한 기능을 통합하여 개발했습니다.

**주요 기능**
- 팀 생성, 팀원 초대 및 역할 관리
- 프로젝트 생성 및 관리
- 업무(Task) 등록 및 Gantt 차트 시각화
- 실시간 채팅(WebSocket 기반)
- 피드(게시글) 작성, 댓글 및 좋아요(리액션) 기능
- 파일 업로드 및 다운로드 지원

<br/>

## 🎥 프로젝트 시연 영상
|TeamVerse 주요 기능 시연 영상|
|:---:|
|[<img src="https://img.youtube.com/vi/1Er1CtSh3UA/0.jpg" width="400"/>](https://www.youtube.com/watch?v=1Er1CtSh3UA&t=12s)|

👉🏻 [YouTube 시연 영상 보러가기](https://www.youtube.com/watch?v=1Er1CtSh3UA&t=12s)


<br/>

## ⚙ 기술 스택
### Backend
<div>
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Java.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/SpringBoot.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/SpringSecurity.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/SpringDataJPA.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Mysql.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/WebSocket.png?raw=true" width="80">
</div>

### Infra
<div>
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/AWSEC2.png?raw=true" width="80">
</div>

### Tools
<div>
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Github.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Notion.png?raw=true" width="80">
</div>

<br/>

## 🗂️ 주요 데이터베이스 테이블
|Table|Description|
|:---|:---|
|users|사용자 계정 정보|
|teams|팀 정보|
|projects|프로젝트 정보|
|tasks|업무(Task) 정보|
|task_dependencies|업무 간 의존성 관리|
|team_members|팀원 및 역할 관리|
|posts|피드(게시글) 데이터|
|comments|게시글 및 업무에 대한 댓글|
|chat_messages|프로젝트 채팅 메시지|
|private_chat_message|개인 채팅 메시지|
|file_info|업로드된 파일 정보|
|likes|게시글 및 업무에 대한 리액션|
|invites|팀 초대 요청 관리|
|activity_logs|사용자 활동 기록|
|user_emojis|사용자별 즐겨찾는 이모지|

<br/>

## 🛠️ 프로젝트 아키텍처
> MVC 기반 설계 + 실시간 통신(WebSocket)  
> DB는 MariaDB, 보안은 JWT 인증을 기반으로 구성되었습니다.

![architecture](https://user-images.githubusercontent.com/80824750/208294567-738dd273-e137-4bbf-8307-aff64258fe03.png)

<br/>

## 🤔 기술적 이슈와 해결 과정
- **WebSocket 인증 처리**
  - WebSocket 연결 시 JWT 토큰을 검증하여 인증된 사용자만 채팅 가능하도록 구현
- **JPA Lazy Loading 문제**
  - 엔티티 순환 참조 방지를 위해 `@JsonIgnoreProperties`, `@JsonIgnore`를 적극 사용
- **파일 업로드/다운로드 기능**
  - AWS S3를 연동해 확장성을 고려했으며, 대용량 파일도 처리할 수 있도록 개선 예정

<br/>

## 💁‍♂️ 프로젝트 팀원
|Backend|Frontend|
|:---:|:---:|
| ![](https://github.com/your-github-id.png?size=120) | (프론트엔드 팀원 추가 시 여기에) |
|[변다혜](https://github.com/your-github-id)| |

> 프로젝트의 Back-end, API 설계, 데이터베이스 모델링을 담당했습니다.

---


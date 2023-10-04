## 🧽강남구, 송파구, 서초구에 있는 자동차 소유주를 위한 세차장 추천 서비스🧼

<br/>

##  ✔ 시작가이드
### 🚘 각 종 프로그램의 버전 및 사전설치:
- Mysql 8.0.34
- Node.js 18.15.0
- Npm 9.5.0
- Linux Ubuntu 22.04

###  🚘 Installation
```
# git clone https://github.com/pleaseCodemyname/1st_project.git
```
### 🚘 Run
```
# apt install -y npm
# npm install -g nodemon
# npm init -y
# npm install express morgan path body-parser cookie-parser axios sync-mysql dotenv
# nodemon app.js
```
<br/>

### ✔ 기술스택

|Category|Language|
|:--:|:--|
|OS|![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black) ![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)|
|Frontend|![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) |
|Backend|![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white) ![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)|
|Database|![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)|

<br/>

### ✔ 프로젝트 개요

- 팀명 : 수료가목표
- 인원 : 2인 [ 윤상현, 이효빈 ]
- 기간 : 4일 [ 2023.04.24.(월) ~ 2023.04.27.(목) ]
- 문서 : Wireframe, Table configuration, API report, Architecture

<br/>

### ✔ 프로젝트 목적
- 데이터베이스를 활용한 웹 프로그래밍
- CRUD 기능을 활용한 웹 서비스 구현
<br/>

### ✔ 아키텍처
![그림1](https://github.com/westmini427/Weatherdata-project/assets/127065150/6b3d2858-e1bf-42b2-afb0-6cea4c588564)

<br/>

### ✔ 프로젝트 요약

- 서초구, 강남구, 서초구에 있는 세차장 데이터를 반영한 데이터 조회.

- 고객 정보 생성, 조회, 수정, 삭제 / 세차장 정보 추가, 수정, 수정, 삭제가 가능한 서비스.

- 고객의 위치를 바탕으로 인근에 위치한 세차장 10곳을 추천하는 서비스.
<br/>

<!-- ### ✔ 개발 과정
![그림1](https://github.com/westmini427/Weatherdata-project/assets/127065150/e7d9930c-1990-41d8-b819-3d2259dc827a)

- 데이터베이스 설계와 API 명세서를 설정 후, 이를 토대로 개발을 진행했습니다. -->

<br/>

<!-- ### ✔ 초기 화면 구성
![Alt text](wireframe.png) -->

<br/>

<!-- ### ✔ 실행 화면
![Alt text](%EB%A9%94%EC%9D%B4%EC%9B%A8%EB%8D%94.gif) -->

## 화면 구성 📺
| 메인 페이지  |  관리자 페이지   |
| :-------------------------------------------: | :------------: |
|  <img width="329" src="https://github.com/pleaseCodemyname/1st_project/blob/main/1st_project_main_page.png"/> |  <img width="329" src="https://github.com/pleaseCodemyname/1st_project/blob/main/1st_project_admin_page.png"/>|  
| 관리자 페이지2   |  사용자 페이지   |  
| <img width="329" src="https://github.com/pleaseCodemyname/1st_project/blob/main/1st_project_admin_page2.png"/>   |  <img width="329" src="https://github.com/pleaseCodemyname/1st_project/blob/main/1st_project_user_page.png"/>     |

---
## 주요 기능 📦

### ⭐️ 송파구, 서초구, 세차장 정보를 조회할 수 있는 기능
- 100개 이상의 세차장 위치 정보 제공
- 추후 사용자 인근 세차장까지 추천해주는 기능 추가 및 업로드 예정

### ⭐️ 기본에 충실한 CRUD 기능
- 사용자의 정보를 생성, 조회, 수정, 삭제 할 수 있는 관리자 페이지 기능
---
<!-- ## 아키텍쳐

### 디렉토리 구조
```bash
├── README.md
├── package-lock.json
├── package.json
├── strapi-backend : 
│   ├── README.md
│   ├── api : db model, api 관련 정보 폴더
│   │   ├── about
│   │   ├── course
│   │   └── lecture
│   ├── config : 서버, 데이터베이스 관련 정보 폴더
│   │   ├── database.js
│   │   ├── env : 배포 환경(NODE_ENV = production) 일 때 설정 정보 폴더
│   │   ├── functions : 프로젝트에서 실행되는 함수 관련 정보 폴더
│   │   └── server.js
│   ├── extensions
│   │   └── users-permissions : 권한 정보
│   ├── favicon.ico
│   ├── package-lock.json
│   ├── package.json
│   └── public
│       ├── robots.txt
│       └── uploads : 강의 별 사진
└── voluntain-app : 프론트엔드
    ├── README.md
    ├── components
    │   ├── CourseCard.js
    │   ├── Footer.js
    │   ├── LectureCards.js
    │   ├── MainBanner.js : 메인 페이지에 있는 남색 배너 컴포넌트, 커뮤니티 이름과 슬로건을 포함.
    │   ├── MainCard.js
    │   ├── MainCookieCard.js
    │   ├── NavigationBar.js : 네비게이션 바 컴포넌트, _app.js에서 공통으로 전체 페이지에 포함됨.
    │   ├── RecentLecture.js
    │   └── useWindowSize.js
    ├── config
    │   └── next.config.js
    ├── lib
    │   ├── context.js
    │   └── ga
    ├── next.config.js
    ├── package-lock.json
    ├── package.json
    ├── pages
    │   ├── _app.js
    │   ├── _document.js
    │   ├── about.js
    │   ├── course
    │   ├── index.js
    │   ├── lecture
    │   ├── newcourse
    │   ├── question.js
    │   └── setting.js
    ├── public
    │   ├── favicon.ico
    │   └── logo_about.png
    └── styles
        └── Home.module.css -->

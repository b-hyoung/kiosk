# 키오스크였던것

## 🎯 **프로젝트 개요**

| 항목 | 설명 |
| --- | --- |
| 📛 **프로젝트명** | 지민시치가 알려줄 예정 |
| 📝 **목적** | 지민시치가 알려줄 예정 |
| 👥 **대상 사용자** | 지민시치가 알려줄 예정 |
| 🧩 **핵심 기능** | 지민시치가 알려줄 예정 |

## 🛠️ **개발 환경**

## 🧑‍🤝‍🧑 **역할 분담**

| 항목 | 내용 |
| --- | --- |
| 🧠 **IDE** | Visual Studio Code (VSCode) |
| 🌐 **Frontend** | Vanilla JavaScript |
| 🔙 **Backend** | FastAPI (Python 3.10+) |
| 🗄️ **Database** | PostgreSQL |
| 🐳 **Dev Tool** | Docker + Docker Compose |
| 🧪 **Test** | `pytest`, Postman 등 |
| 🗃️ **버전 관리** | Git + GitHub |
| 🧩 **배포 계획** | (예: Netlify + Render, Railway, EC2 등) |

| 역할 | 이름 |
| --- | --- |
| 기획 | 박지민 |
| 디자인 | 박지민,빅토리아 |
| 프론트 | 박지민,빅토리아 |
| 백엔드 | 박형석,금태호 |
| 뭐 | 누렁이 |
| 기타 | 박지민 |
| 등 | 김지민 |
| 등 | 박지민였던것 |

## 🔧 폴더 구조 (예시)

```bash
project-root/
├── frontend/          # 정적파일 (HTML, JS, CSS)
│   ├── index.html     # 메인 HTML
		├── pages/         # HTML (페이지 Viewer)
│     ├── login.html
│     ├── signup.html
│   ├── js/            # JS파일 (페이지 기능)
|     ├── login.js
|     ├── signup.js      
│   └── css/           # CSS
|     ├── login.css
|     ├── signup.css
backend/
└── app/
    ├── main.py               # FastAPI 진입점
    ├── routes/               # API 라우팅 모음 ex) /user/login
    │   ├── user_routes.py      # 🔑 로그인/회원가입 등 유저 관련 API
    │   └── group_routes.py     # 👥 모임/그룹 관련 API ex) group/post
    ├── models/               # DB 모델 (ORM or Pydantic)
    │   ├── user.py
    │   └── group.py
    ├── schemas/              # 요청/응답용 Pydantic 스키마
    │   ├── user_schema.py
    │   └── group_schema.py
    └── services/             # 비즈니스 로직 분리 (선택적)
        ├── user_service.py
        └── group_service.py
├── docker/
│   └── Dockerfile / docker-compose.yml
├── README.md
└── .env
```

## 🔄 **API 설계 요약 (예시)**

| 기능 | Method | Endpoint | 설명 |
| --- | --- | --- | --- |
| 회원가입 | POST | `/api/user/signup` | 회원정보 등록 |
| 로그인 | POST | `/api/user/login` | 로그인 처리 |
| 그룹 리스트 | GET | `/api/group/` | 모든 그룹 목록 조회 |
| 그룹 생성 | POST | `/api/group/` | 새로운 그룹 만들기 |

※ 상세 스펙은 Swagger를 통한 API 링크 공유
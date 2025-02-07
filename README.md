# CS-study

## 🚄 KTB 바이너리는 호남선 CS 스터디
카카오테크 부트캠프(KTB) 바이너리는 호남선 팀이 진행하는 **2차 CS 스터디 페이지**입니다.  
1차 스터디는 **노션에서 도서를 바탕으로 진행**했으며 자료는 아래에서 확인 가능합니다.

📖 **1차 스터디 자료**: [🔗 노션 링크](https://www.notion.so/goormkdx/2-15ac0ff4ce3180c08667ef6b3b0a2cda?pvs=4)  (접근 권한 요청 필요)
📚 **활용 교재**: _이것이 취업을 위한 컴퓨터 과학이다 with CS 기술 면접_ - 강민철 저  
📆 **기간**: `2024-12-19` ~ `2025-01-31`

---

## 📌 스터디 소개 
🚀 본 스터디는 컴퓨터 과학 핵심 개념을 심층적으로 학습하고, **이론과 실무 적용 능력을 강화하는 것을 목표**로 합니다.  

1. **스터디 진행**
   - 매주 목요일 22시 진행 (필요 시 일정 조율 가능)
   - 각 주차별 주제는 사전에 정하고 발표자는 발표 자료 준비 후 PR 제출

2. **발표 자료 및 PR**
   - 발표 자료는 **PR을 통해 제출**
   - 발표 후 **GitHub Wiki에 발표 피드백 기록**
   - 발표 자료는 **각 주차별 폴더(`week-XX/`)에 정리**

3. **태그 관리 (`git tag`)**
   - 발표가 끝난 후 해당 주차 발표 자료를 태그로 기록
   ```bash
   git tag -a week-02 -m "Week 02 발표 완료"
   git push origin week-02
   ```
   - 특정 주차의 발표 자료를 확인할 때:
   ```bash
   git checkout week-02
   ```

---

## 😀 멤버
| 이름 | 닉네임 | GitHub |
|------|--------|--------|
| 신효경 | Hayden | [@hayden-shin](https://github.com/hayden-shin) |
| 이중현 | Keen | [@keen1014](https://github.com/keen1014) |
| 이세현 | Jack | [@SeHyeonLee-dev](https://github.com/SeHyeonLee-dev) |
| 현지우 | Semi | [@boojang](https://github.com/boojang) |

---

## 🌿 브랜치 및 커밋 규칙

### 📌 **브랜치 규칙**
```
week-XX/닉네임-주제
```
📌 **예제**:
- `week-02/hayden-ci-cd`
- `week-03/keen-docker`
- `week-04/semi-microservices`

### 📝 **커밋 메시지 규칙**

```
[주차-닉네임] feat: 설명
```
📌 **예제**
```
[2-hayden] feat: CI/CD 개념 정리 및 도식 추가
[2-hayden] fix: CI/CD 예제 코드 수정
[2-hayden] refactor: 발표 자료 구조 개선
[3-keen] feat: Docker 컨테이너 실습 추가
[3-keen] docs: 발표 자료 관련 README 업데이트
[4-semi] feat: 마이크로서비스 디자인 패턴 정리
```

---

## 📅 스터디 일정

### 🔗 참고 자료

- [System Design 101](https://github.com/ByteByteGoHq/system-design-101)
- 기타 유용한 자료를 각 주차별로 공유 예정

### 📖 주제 및 담당자

#### 📡 Communication Protocols

- REST API vs. GraphQL – 발표자: TBD
- How does gRPC work? – 발표자: TBD
- What is a webhook? – 발표자: TBD
- How to improve API performance? – 발표자: TBD
- HTTP 1.0 → HTTP 1.1 → HTTP 2.0 → HTTP 3.0 (QUIC) – 발표자: TBD
- SOAP vs REST vs GraphQL vs RPC – 발표자: TBD
- Code First vs. API First – 발표자: TBD
- HTTP status codes – 발표자: TBD
- What does API gateway do? – 발표자: TBD
- How do we design effective and safe APIs? – 발표자: TBD
- TCP/IP encapsulation – 발표자: TBD
- Why is Nginx called a “reverse” proxy? – 발표자: TBD
- What are the common load-balancing algorithms? – 발표자: TBD
- URL, URI, URN - Do you know the differences? – 발표자: TBD

#### 🚀 CI/CD

✅ CI/CD Pipeline Explained in Simple Terms – 잭: `1주차`
✅ Netflix Tech Stack (CI/CD Pipeline) – 잭: `1주차`

#### 🏛 Architecture Patterns

- MVC, MVP, MVVM, MVVM-C, and VIPER – 발표자: TBD
- 18 Key Design Patterns Every Developer Should Know – 발표자: TBD

#### 🗄 Database

- A nice cheat sheet of different databases in cloud services – 발표자: TBD
- 8 Data Structures That Power Your Databases – 발표자: TBD
- How is an SQL statement executed in the database? – 발표자: TBD
- CAP theorem – 발표자: TBD
- Types of Memory and Storage – 발표자: TBD
- Visualizing a SQL query – 발표자: TBD
- SQL language – 발표자: TBD

#### 💾 Cache

- Data is cached everywhere – 발표자: TBD
- Why is Redis so fast? – 발표자: TBD
- How can Redis be used? – 발표자: TBD
- Top caching strategies – 발표자: TBD

#### 🏗 Microservice Architecture

- What does a typical microservice architecture look like? – 발표자: TBD
- Microservice Best Practices – 발표자: TBD
- What tech stack is commonly used for microservices? – 발표자: TBD
- Why is Kafka fast? – 발표자: TBD

#### 💳 Payment Systems

- How to learn payment systems? – 발표자: TBD
- Why is the credit card called “the most profitable product in banks”? – 발표자: TBD
- How does VISA work when we swipe a credit card at a merchant’s shop? – 발표자: TBD
- UPI in India (Unified Payments Interface) – 발표자: TBD

#### 🛠 DevOps

- DevOps vs. SRE vs. Platform Engineering – 발표자: TBD
- What is k8s (Kubernetes)? – 발표자: TBD
- Docker vs. Kubernetes. Which one should we use? – 발표자: TBD
- How does Docker work? – 발표자: TBD

#### 🌲 GIT

✅ How Git Commands work – 킨: `1주차`
✅ How does Git Work? – 킨: `1주차`
✅ Git merge vs. Git rebase – 킨: `1주차`

#### ☁️ Cloud Services

- A nice cheat sheet of different cloud services (2023 edition) – 발표자: TBD
- What is cloud native? – 발표자: TBD

#### 🏆 Developer Productivity Tools

- Visualize JSON files – 발표자: TBD
- Automatically turn code into architecture diagrams – 발표자: TBD

#### 🐧 Linux

✅ Linux file system explained – 세미: `1주차`
✅ 18 Most-used Linux Commands You Should Know – 세미: `1주차`

#### 🔐 Security

✅ How does HTTPS work? – 헤이든: `1주차`
✅ Oauth 2.0 Explained With Simple Terms – 헤이든: `1주차`
- Top 4 Forms of Authentication Mechanisms – 발표자: TBD
- Session, cookie, JWT, token, SSO, and OAuth 2.0 - what are they? – 발표자: TBD
- How to store passwords safely in the database and how to validate a password? – 발표자: TBD
- Explaining JSON Web Token (JWT) to a 10-year-old Kid – 발표자: TBD
- How does Google Authenticator work? – 발표자: TBD

#### 📖 Real-World Case Studies

- Netflix's Tech Stack – 발표자: TBD
- Twitter Architecture 2022 – 발표자: TBD
- Evolution of Airbnb’s microservice architecture – 발표자: TBD
- Monorepo vs. Microrepo – 발표자: TBD
- How will you design the Stack Overflow website? – 발표자: TBD
- Why did Amazon Prime Video monitoring move from serverless to monolithic? – 발표자: TBD
- How does Disney Hotstar capture 5 Billion Emojis? – 발표자: TBD
- How Discord Stores Trillions Of Messages – 발표자: TBD
- How do video live streamings work on YouTube, TikTok, or Twitch? – 발표자: TBD

# Oath 2.0
---

## 🔍 OAuth 2.0이란?
- 앱과 서비그사 사용자 정보를 안전하게 공유할 수 있도록 해주는 인증 및 권한 부여 프레임 워크- 비밀번호나 중요한 개인정보를 직접 공유하지 않고도 다양한 애플리케이션과 서비스가 사용자 대신 상호작용 가능

### OAuth 2.0의 주요 구성 요소
OAuth 2.0의 세 가지 주요 역할
1. 사용자 (User)
  - 서비스(ex: Google, FaceBook)에 로그인하고 특정 앱이 자신의 데이터에 접근할 수 있도록 허용하는 사람
2. 서버 (Server, Resource Server)
  - 사용자 데이터를 보관하고 관리하는 서비스 (ex. Google Drive, Facebook API)
3. ID 제공자 (Identity Provider, IDP)
  - 사용자 인증을 담당하는 서비스 (ex. Google, Facebook, Apple)
  - IDP는 로그인 정ㅎ보 확인 -> 인증된 사용자에게 OAuth 토큰 발급

---

## 🔑 OAuth 토큰이 하는 일
- OAuth 2.0 사용하면 OAuth 토큰을 발급받음 -> 토큰: 사용자의 신원 및 권한을 나타내는 *디지털 키* 역할
### 1. 싱글 사인온 (Single Sign-On, SSO)
- 한 번 로그인하면 여러 서비스나 앱을 추가 로그인 없이 사용 가능
- ex. 구글 계정으로 여러 웹사이트에 로그인
### 2. 시스템 간 인증 (Authorisatoin Across Systems)
- OAuth 토큰을 사용하면 여러 시스템에서 권한 공유 가능
- ex. 트위터 계정으로 타사 앱에 트윗 작성
### 3. 사용자 프로필 정보 접근 (Accessing User Profile)
- OAuth 토큰을 사용하면 허용된 범위 내에서만 사용자 정보 접근 가능
- ex. 페이스북 계정으로 로그인할 때, 앱이 사용자 프로필 사진과 이메일만 가져가도록 설정 가능

#[OAuth2](./images/oAuth2.jpg)  

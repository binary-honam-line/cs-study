![Netflix CI/CD 파이프라인 기술 스택](https://github.com/ByteByteGoHq/system-design-101/blob/main/images/netflix-ci-cd.jpg)

# Netflix CI/CD 파이프라인 기술 스택

Netflix는 **CI/CD(Continuous Integration/Continuous Deployment)** 파이프라인을 통해 **자동화된 소프트웨어 개발 및 배포 프로세스**를 운영합니다. 이를 통해 빠르고 안정적인 서비스 제공이 가능합니다.

## **1. 계획 (Plan)**

Netflix는 **JIRA**와 **Confluence**를 활용하여 프로젝트 관리 및 문서화를 수행합니다.

- **JIRA**: 프로젝트 관리 및 일정 계획
- **Confluence**: 팀 협업 및 문서화 지원

## **2. 코드 작성 (Code)**

Netflix는 다양한 프로그래밍 언어를 활용하여 애플리케이션을 개발합니다.

- **주요 백엔드 언어**: Java
- **기타 사용 언어**: Python, Scala, JavaScript, Kotlin
- **프레임워크**: Spring Boot
- **데이터 분석 및 노트북**: Polynote

## **3. 빌드 (Build)**

Netflix는 코드 변경 사항을 효율적으로 빌드하기 위해 다음과 같은 도구를 사용합니다.

- **Gradle**: 기본 빌드 도구
- **Nebula**: Gradle 플러그인을 활용하여 다양한 빌드 요구사항 지원

## **4. 테스트 (Test)**

Netflix는 서비스의 안정성을 보장하기 위해 **Chaos Engineering(혼돈 공학)**을 활용한 테스트를 수행합니다.

- **Chaos Monkey**: 랜덤 장애 시뮬레이션을 수행하여 시스템 내구성 테스트
- **CHAP (ChAP)**: 실시간 트래픽을 활용한 카나리 테스트
- **UP (Automated Test Framework)**: Netflix 내부에서 사용하는 자동화 테스트 프레임워크

## **5. 릴리즈 (Release)**

Netflix는 **Jenkins**와 **Animator**를 활용하여 지속적인 릴리즈를 자동화합니다.

- **Jenkins**: CI/CD 파이프라인에서 지속적 통합 및 배포 지원
- **Animator**: Netflix 내부에서 빌드된 자동화 릴리즈 도구

## **6. 배포 (Deploy)**

Netflix는 **카나리 롤아웃(Canary Rollout) 배포 전략**을 활용하여 안정적인 배포를 수행합니다.

- **Spinnaker**: Netflix가 자체 개발한 멀티클라우드 지속적 배포 도구
- **HashiCorp Packer**: AMI(Amazon Machine Image) 생성 및 패키징

## **7. 모니터링 (Monitor)**

Netflix는 대규모 트래픽을 관리하기 위해 실시간 모니터링 시스템을 구축하고 있습니다.

- **Atlas**: Netflix의 중앙 집중식 메트릭 및 모니터링 플랫폼
- **Kayenta**: A/B 테스트 기반 자동화된 이상 탐지 및 배포 안정성 평가 도구

## **8. 운영 및 사고 대응 (Operate & Incident Management)**

Netflix는 서비스 장애 시 신속하게 대응하기 위한 인시던트 대응 시스템을 운영합니다.

- **PagerDuty**: 장애 발생 시 알림 및 대응 관리
- **Dispatch**: Netflix의 자동화된 인시던트 관리 및 대응 시스템

Netflix의 CI/CD 파이프라인은 **대규모 트래픽을 안정적으로 관리**하고, **빠른 배포와 운영을 가능하게 하는 핵심 요소**입니다. 🚀

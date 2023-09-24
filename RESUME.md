## 이건호 / Software Programmer

### Contact

- 010-0000-0000
- gunho1020@gmail.com
- [articles](https://github.com/daengdaengLee/articles) | [medium](https://medium.com/@daengdaenglee/lists)

### About Me

- 6년 차 웹 프로그래머로 웹 프론트엔드 & 백엔드, 배치 애플리케이션을 개발했습니다.
- JS / TS + Node.js 를 잘 사용합니다. Java + Spring 을 배우고 있습니다.
- 명세와 매뉴얼에 맞게 동작하는 프로그램을 만들려고 합니다. 개발자와 사용자 모두 믿고 쓸 수 있어야 합니다.

#### 기술 스택 전환

- JS / TS + Node.js 로 개발해 왔지만, Java + Spring, Go, Rust 같은 기술로 개발하고 싶습니다.
- 강력하고 통합된 툴체인(빌드툴을 포함하여) 및 개발 환경의 혜택을 누리고 싶습니다. 실제 문제를 해결하기 위한 코드 작성에 더 집중하고 싶습니다.
- 모듈, 패키지, 네임스페이스와 같은 기능을 사용하고 싶습니다. 프로젝트를 더 잘 구조화할 수 있다고 생각합니다.
- 더 Sound 한 타입 시스템의 혜택을 누리고 싶습니다. 유연한 구조의 프로젝트에서 개발자의 실수를 줄여줍니다.

## Work Experience

### 마플코퍼레이션 (2020.01.02 ~ 2023.07.31)

- 웹 풀 스택 프로그래머로 커스텀 상품 제작용 벡터 에디터, 생산 자동화 배치 애플리케이션, PFP NFT 프로젝트 빌더, Web3 커뮤니티 서비스의 인증 및 인가 도메인을 개발, 유지 보수, 운영했습니다.
- 문제를 해결하기 위해 기술의 깊은 밑바닥까지 연구했습니다.
- 단순하고 유연한, 안정적으로 협업할 수 있는 소프트웨어 설계를 고민하고 논의하고 적용했습니다.

#### CIETY (2022.06 ~ 2023.06)

- [homepage](https://www.ciety.xyz/) | [webapp](https://ciety.xyz/login)
- 프로젝트 소개: 웹3 기능을 제공하는 새로운 커뮤니티 빌딩 플랫폼입니다.
- 역할: 백엔드 프로그래머로 인증 및 인가 기능의 DB 설계부터 API 엔드포인트까지 담당하여 개발했습니다.
- 사용한 기술: TS, pnpm, NestJS, Prisma, Jest, Docker, AWS
- 기능: 메타마스크 블록체인 지갑과 이메일로 회원가입, 로그인하는 API와 JWT를 사용해 인증 상태를 검증하고 유지하는 기능을 개발했습니다.
  특히 모바일 앱 환경에서 메타마스크 지갑 앱과 연동할 수 있도록 개발했습니다.
- 기능: 역할, 코인 및 NFT 보유량으로 게시판 입장 및 기능에 대한 조건을 설정하는 기능과 해당 조건을 검사하는 기능을 개발했습니다.
- 개선: 중복 쿼리를 병합하여 API 속도를 평균 160ms에서 평균 60ms로 개선했습니다.
  ([관련 블로그](https://medium.com/@daengdaenglee/prisma-%EC%A1%B0%ED%9A%8C-%EC%B5%9C%EC%A0%81%ED%99%94-e17043266739))
- 테스트: 개발한 API에 대해 GitHub PR 생성 시 자동으로 실행되는 E2E 테스트를 작성하여 기존 API가 정상 동작하는지 확인했습니다.

#### OMNUUM (2022.01 ~ 2022.04)

- [homepage](https://omnuum.io/) | [webapp](https://studio.omnuum.io/)
- 프로젝트 소개: 웹3 PFP NFT 프로젝트를 No Code로 손쉽게 만들 수 있는 플랫폼입니다.
- 역할: 프론트엔드 프로그래머로 NFT PFP 빌더 개발 파트를 리드했습니다.
  데이터 구조, API 인터페이스, 프로젝트 구조를 정하고 서버와 블록체인 네트워크에 API를 요청하는 코드를 개발했습니다.
- 사용한 기술: TS, Yarn, React, RxJS
- 설계: 비즈니스 로직과 React로 작성한 뷰 로직을 분리해 비즈니스 로직 개발이 완료될 때까지 기다리지 않고 뷰 로직 개발을 진행했고
  백엔드 개발팀, 디자인 팀 동료와 유연하게 협업할 수 있었습니다.
- 기능: 낙관적 Lock을 적용해 API로 등록한 메타데이터와 업로드하는 이미지 파일 사이의 정합성을 보장했습니다.
- 기능: 이미지 업로드 요청이 API 서버에 주는 부하를 줄이기 위해 AWS S3의 presigned URL을 발급해 사용했습니다.

#### 제품 제작용 PDF 자동 생성 시스템 (2020.12 ~ 2021.02:2023.06 까지 추가 개발 및 유지보수 진행)

- 프로젝트 소개: 지류 제품 생산에 사용할 출력용 PDF 파일을 매일 생성하는 배치 프로그램입니다.
- 역할: 백엔드 프로그래머로 PDF 파일 생성 기능을 개발, 운영 및 유지보수했습니다.
- 사용한 기술: JS, TS, Playwright, Docker, AWS
- 설계: 외부 자원을 사용하는 코드에 대한 의존성을 주입받아 사용하도록 설계했습니다.
  테스트 환경에서도 Mock 객체나 로컬에서 도커로 실행한 AWS Lambda 서비스를 이용해 PDF 파일을 생성할 수 있습니다.
- 기능: 이미지 바이너리 데이터를 유일하게 관리하고 참조를 통해 여러 번 같은 이미지를 출력하도록 PDF 파일을 생성했습니다.
  파일 크기를 최소화해서 더 적은 리소스로 파일을 생성하고 생산 장비에서 오류나 지연 없이 더 빨리 작업할 수 있게 되었습니다.
  이 기능을 제공하는 라이브러리를 찾지 못해 PDF 스펙을 연구하여 PDF 파일을 생성하는 코드를 직접 작성했습니다.
- 기능: PDF 파일을 생성하는 코드는 Node.js 스트림 API와 async generator 함수를 사용하여 작성했습니다.
  고화질 이미지를 다수 포함한 대용량 PDF 파일을 OMM 에러 없이 안전하게 생성했습니다.
- 기능: 제품 생산을 위한 이미지를 브라우저로만 생성할 수 있어서 Playwright(Headless 브라우저)로 이미지를 생성했습니다.
  AWS Lambda에서 실행해 Playwright가 사용하는 리소스가 배치 프로그램의 전체 기능에 영향을 주지 않도록 격리했습니다.
  커스텀 도커 이미지를 만들어서 AWS Lambda에서 Playwright를 실행하기 위한 의존성을 함께 배포했습니다.

#### 벡터 기반 웹 에디터 (2020.05 ~ 2021-07:2023.06 까지 추가 개발 및 유지보수 진행)

- 프로젝트 소개: SVG 벡터 이미지를 사용해 스티커, 아크릴 키링, 아크릴 스탠드와 같은 커스텀 제품을 디자인할 수 있는 웹 에디터입니다.
- 역할: 프론트엔드 프로그래머로 SVG 이미지를 편집, 저장하고 로드하는 기능을 개발했습니다. 에디터의 줌, 패닝 기능을 개발했습니다.
- 사용한 기술: JS, SVG, FxJS (회사에서 자체 개발한 함수형 라이브러리), Frame (회사에서 자체 개발한 UI 개발 프레임워크)

### BRIQUE (브릭) (2018.03.02 ~ 2019.12.20)

- 웹 프론트엔드 프로그래머로 주로 반도체 공장에서 사용하는 데이터 분석 애플리케이션의 웹 UI를 개발했습니다.
- 프로젝트, 팀, 회사 업무에서 개선할 점을 적극적으로 개선했습니다.

#### BRIQUE Analytics (2018.03 ~ 2019.12)

- 프로젝트 소개: 파이썬 또는 R로 작성한 코드를 노드로 등록하고 웹 UI를 이용해 워크플로우를 만들어 실행할 수 있는 플랫폼입니다.
- 역할: 프론트엔드 프로그래머로 워크플로우를 그리는 UI와 실행 로그를 출력하는 UI를 개발했습니다. 레거시 코드를 주도적으로 개선했습니다.
- 사용한 기술: JS, SVG, React, Redux, Redux-Saga, RxJS, WebSocket
- 개선: IIFE 모듈 패턴과 JQuery를 사용하여 2개 파일(각 5만, 6만 줄)로 구성된 프로젝트를 Webpack, Babel, React를 사용하도록 변경했습니다.
  이후 더 쉽게 목적과 역할에 맞게 모듈 및 파일을 분리할 수 있었고 협업할 때 불필요한 충돌이 줄어들었습니다.
  새로운 기술 도입을 위한 자료 조사, 테스트, 교육을 주도적으로 진행했습니다.

#### Data Prep (2019.07 ~ 2019.08)

- 프로젝트 소개: 테이블 형태의 대용량 데이터를 웹 UI에 표현하고 불필요한 데이터를 제거할 수 있는 프로그램입니다. 위 BRIQUE Analytics의 부가 기능으로 개발했습니다.
- 역할: 프론트엔드 프로그래머로 데이터를 화면에 출력하기 위한 무한 스크롤 테이블 UI를 개발했습니다.
- 사용한 기술: JS, React, react virtualized

#### FDC (2018.08 ~ 2018.09)

- 프로젝트 소개: 반도체 장비에서 수집한 과거 또는 실시간 센서 데이터를 웹 기반 차트 UI로 출력하는 프로그램입니다.
- 역할: 프론트엔드 프로그래머로 대용량 타임 시리즈 데이터를 그리는 차트 UI를 개발했습니다.
- 사용한 기술: JS, React, Dygraphs

## Other Experience

### Side Project

#### Mangrul (2023.09 ~ 현재)

- [repo](https://github.com/daengdaengLee/mangurl) | [webapp](https://mangurl.net/app)
- 프로젝트 소개: 해시 기반 URL 단축 서비스입니다.
- 역할: 개인 프로젝트로 개발, 배포, 운영 모두 직접 하고 있습니다.
- 사용한 기술: Java, Spring MVC, DynamoDB, S3, ECS 등

### Open Source

#### utilitystreams (2023.07 ~ 현재)

- [repo](https://github.com/daengdaengLee/utilitystreams) | [npm](https://www.npmjs.com/package/utilitystreams)
- 프로젝트 소개: Node.js에서 Stream API를 사용할 때 편리하게 쓸 수 있는 스트림 클래스, 함수 모음입니다.
- 역할: 개인 프로젝트로 개발, 배포 모두 직접 하고 있습니다.
- 사용한 기술: TS, Jest
- 기능: 제어하기 어려운 비동기 동작을 처리하는 편의 기능을 제공합니다. (Delay, Debounce, Throttle, Buffer)

#### GlueSQL

- [repo](https://github.com/gluesql/gluesql)
- 기여: https://github.com/gluesql/gluesql/pull/1259

## Skill

### 언어 / 런타임

- Java
- JS / TS / Node.js

### 프레임워크 / 라이브러리

- Web : Spring / NestJS / Express.js
- DB : Prisma / FxSQL
- Test : JUnit / AssertJ / Mockito / Jest
- UI : React
- Utility : RxJS / FxJS / FxTS

### 인프라 / AWS

- Docker
- GitHub Action
- EC2 / ECS / ECR / Lambda / SQS / S3

## Education

### 동국대학교 / 수학교육과 (2011.03.02 ~ 2017.02.16)

- 학점 : 3.9 / 4.5

# RESUME

- updated at : 2023-09-20

## 이건호 / Software Programmer

### Contact

- 010-0000-0000
- gunho1020@gmail.com
- [articles](https://github.com/daengdaengLee/articles) | [medium](https://medium.com/@daengdaenglee/lists)

### About Me

- 6년 차 웹 프로그래머로 웹 프론트엔드 & 백엔드, 배치 애플리케이션을 개발했습니다.
- JS / TS + Node.js 를 잘 사용합니다. Java + Spring, Rust 를 배우고 있습니다.
- 명세와 매뉴얼에 맞게 동작하는 프로그램을 만들려고 합니다. 개발자와 사용자 모두 믿고 쓸 수 있어야 합니다.

## Work Experience

### 마플코퍼레이션 / 웹 풀 스택 프로그래머 (2020.01.02 ~ 2023.07.31)

#### CIETY / 백엔드 프로그래머 (2022.06 ~ 2023.06)

- [homepage](https://www.ciety.xyz/) | [webapp](https://ciety.xyz/login) | [google play](https://play.google.com/store/apps/details?id=com.ciety.xyz.prod&pcampaignid=web_share) | [app store](https://apps.apple.com/us/app/ciety-web3-game-community/id6443814305)
- 웹3 기능을 제공하는 새로운 커뮤니티 빌딩 플랫폼입니다.
- 사용한 기술: TS, pnpm, NestJS, Prisma, Jest, Docker, AWS
- 메타마스크 블록체인 지갑과 이메일로 회원가입, 로그인하는 API와 JWT를 사용해 인증 상태를 검증하고 유지하는 기능을 개발했습니다.
  특히 모바일 앱 환경에서 외부의 메타마스크 지갑 앱을 사용해 인증을 진행하기 위해 API를 단계별로 분리하고 이전 단계 호출을 추적할 수 있도록 설계하고 개발했습니다.
- 역할, 코인 및 NFT 보유량으로 게시판 입장 및 기능에 대한 조건을 설정하는 기능과 해당 조건을 검사하는 기능을 개발했습니다.
  관리자 유저가 직접 원하는 역할을 동적으로 편집할 수 있도록 데이터 구조를 설계하고 관련 API를 개발했습니다.
  게시판 기능을 추가할 계획이 있으므로 게시판 기능에 대한 조건을 DB 테이블로 관리할 수 있도록 설계하고 관련 API를 개발했습니다.
- 파라미터값만 다른 같은 쿼리를 중복해서 실행하는 코드를 병합하고 DB에 요청하는 코드를 모아 동시에 실행해서 API 속도를 평균 160ms에서 평균 60ms로 개선했습니다.
  ([관련 블로그](https://medium.com/@daengdaenglee/prisma-%EC%A1%B0%ED%9A%8C-%EC%B5%9C%EC%A0%81%ED%99%94-e17043266739))
- 개발한 API에 대해 GitHub PR 생성 시 자동으로 실행되는 E2E 테스트를 작성하여 기존 API가 정상 동작하는지 확인했습니다.

#### OMNUUM / 프론트엔드 프로그래머 (2022.01 ~ 2022.04)

- [homepage](https://omnuum.io/) | [webapp](https://studio.omnuum.io/)
- 웹3 PFP NFT 프로젝트를 No Code로 손쉽게 만들 수 있는 플랫폼입니다.
- 사용한 기술: TS, Yarn, React, RxJS
- 속성 이미지를 조합해 프로필 이미지들을 생성하고 메타데이터와 이미지 파일들을 안전하게 서버에 전송하는 코드를 개발했습니다.
  이미지 파일이 많으므로 (기본 10,000장) 메타데이터를 등록하는 요청과 이미지 업로드 요청을 분리했습니다.
  메타데이터와 업로드한 이미지 사이의 정합성을 보장하기 위해 낙관적 Lock을 적용했습니다.
- 이미지 업로드 요청이 API 서버에 주는 부하를 줄이기 위해 AWS S3의 presigned URL을 발급해 사용했습니다.
- NFT PFP 빌더 개발의 주 책임자로 참여하여 비즈니스 로직과 React로 작성한 뷰 로직을 분리하고 RxJS를 사용해 애플리케이션 상태를 전파하도록 설계했습니다.
  같은 인터페이스를 구현한 Mock 객체를 사용해 비즈니스 로직 개발이 완료될 때까지 기다리지 않고 뷰 로직 개발을 진행했고 백엔드 개발팀, 디자인 팀 동료와 유연하게 협업할 수 있었습니다.

#### 제품 제작용 PDF 자동 생성 시스템 / 백엔드 프로그래머 (2020.12 ~ 2021.02:2023.06 까지 추가 개발 및 유지보수 진행)

- 지류 제품 생산에 사용할 출력용 PDF 파일을 매일 생성하는 배치 프로그램입니다.
- 사용한 기술: JS, TS, Playwright, Docker, AWS
- 이미지 바이너리 데이터를 유일하게 관리하고 참조를 통해 여러 번 동일한 이미지를 출력하도록 PDF 파일을 생성했습니다.
  파일 크기를 최소화해서 더 적은 리소스로 파일을 생성하고 생산 장비에서 오류나 지연 없이 더 빨리 작업할 수 있게 되었습니다.
  이 기능을 제공하는 라이브러리를 찾지 못해 PDF 스펙을 연구하여 PDF 파일을 생성하는 코드를 직접 작성했습니다.
- PDF 파일을 생성하는 코드는 Node.js 스트림 API와 async generator 함수를 사용하여 작성했습니다.
  고화질 이미지를 다수 포함한 대용량 PDF 파일을 OMM 에러 없이 안전하게 생성했습니다.
- 제품 생산을 위한 이미지를 브라우저로만 생성할 수 있어서 Playwright(Headless 브라우저)로 이미지를 생성했습니다.
  AWS Lambda에서 실행해 Playwright가 사용하는 리소스가 배치 프로그램의 전체 기능에 영향을 주지 않도록 격리했습니다.
  커스텀 도커 이미지를 만들어서 AWS Lambda에서 Playwright를 실행하기 위한 의존성을 함께 배포했습니다.
- 외부 자원을 사용하는 코드에 대한 의존성을 주입받아 사용하도록 설계했습니다.
  테스트 환경에서도 Mock 객체나 로컬에서 도커로 실행한 AWS Lambda 서비스를 이용해 PDF 파일을 생성할 수 있습니다.
- PDF 파일 생성 기능 및 제품 이미지 생성 기능을 개발하기 위해 PDF 스펙을 연구했고 개발, 배포, 운영, 추가 기능 개발 및 유지보수까지 주 책임자로 참여했습니다.

#### 벡터 기반 웹 에디터 / 프론트엔드 프로그래머 (2020.05 ~ 2021-07:2023.06 까지 추가 개발 및 유지보수 진행)

- SVG 벡터 이미지를 사용해 스티커, 아크릴 키링, 아크릴 스탠드와 같은 커스텀 제품을 디자인할 수 있는 웹 에디터입니다.
- SVG 엘리먼트를 조작해 웹 환경에서 벡터 이미지를 편집(이동, 회전, 크기 변환, 패스 편집)할 수 있는 UI를 개발했습니다.
- 더 편리한 사용을 위해 그룹, 줌, 패닝 기능과 SVG 파일을 로드하는 기능을 개발했습니다.
- 웹 에디터 코어 기능 개발을 위해 SVG 스펙과 웹 API를 연구했으며 개발, 배포, 추가 기능 개발 및 유지보수까지 주 책임자로 참여했습니다.

### BRIQUE (브릭) / 웹 프론트엔드 프로그래머 (2018.03.02 ~ 2019.12.20)

#### BRIQUE Analytics / 프론트엔드 프로그래머 (2018.03 ~ 2019.12)

- 파이썬 또는 R로 작성한 코드를 노드로 등록하고 웹 UI를 이용해 워크플로우를 만들어 실행할 수 있는 플랫폼입니다.
- 스크립트와 실행 옵션을 노드로 등록하고 노드를 연결하여 워크플로우를 구성하는 UI를 개발했습니다. (React, SVG)
- 웹 소켓으로 워크플로우 실행 로그를 받아 출력하는 콘솔 화면 UI를 개발했습니다. (React, WebSocket)
- IIFE 모듈 패턴과 JQuery를 사용하여 2개 파일(각 5만, 6만 줄)로 구성된 프로젝트를 Webpack, Babel, React를 사용하도록 변경했습니다.
  이후 더 쉽게 목적과 역할에 맞게 모듈 및 파일을 분리할 수 있었고 협업할 때 불필요한 충돌이 줄어들었습니다.
  새로운 기술 도입을 위한 자료 조사, 테스트, 교육을 주도적으로 진행했습니다.

#### Data Prep / 프론트엔드 프로그래머 (2019.07 ~ 2019.08)

- 테이블 형태의 대용량 데이터를 웹 UI에 표현하고 불필요한 데이터를 제거할 수 있는 프로그램입니다. 위 BRIQUE Analytics의 부가 기능으로 개발했습니다.
- 대용량 2차원 데이터를 화면에 출력하기 위한 무한 스크롤 테이블 UI를 개발했습니다. (React, react-virtualized)

#### FDC / 프론트엔드 프로그래머 (2018.08 ~ 2018.09)

- 반도체 장비에서 수집한 과거 또는 실시간 센서 데이터를 웹 기반 차트 UI로 출력하는 프로그램입니다.
- 대용량 타임 시리즈 데이터를 그리는 차트 UI를 개발했습니다. (dygraphs.js, React)

## Other Experience

### Side Project

#### Mangrul

- [repo](https://github.com/daengdaengLee/mangurl) | [webapp](https://mangurl.net/app)
- 사용한 기술: Java, Spring MVC, DynamoDB, S3, ECS 등
- 해시 기반 URL 단축 서비스입니다. 원본 URL에 대한 고유한 7자리 해시 코드를 만들어서 단축 URL을 제공합니다.
- 해시 코드는 URL에서 안전하게 사용 가능하도록 Base62 방식으로 인코딩한 문자를 사용합니다.
- 해시 충돌이 발생하면 원본 URL에 salt 값을 더해 다시 단축 알고리즘을 실행합니다.
  아직 사용하지 않은 단축 URL 해시 코드가 충분하다면 충분히 해시 충돌을 해소할 수 있습니다.
- 개인 프로젝트로 개발, 배포, 운영 모두 직접 하고 있습니다.
  AWS 의 VPC, ALB, Route 53, ACM, ECR, ECS, S3 서비스를 이용해 운영 중입니다.

### Open Source

#### utilitystreams

- [repo](https://github.com/daengdaengLee/utilitystreams) | [npm](https://www.npmjs.com/package/utilitystreams)
- 사용한 기술: TS, Jest
- Node.js에서 Stream API를 사용할 때 편리하게 쓸 수 있는 스트림 클래스, 함수 모음입니다.
- 단순하고, 사용하기 쉽게 설계했습니다. 특히 제어하기 어려운 비동기 동작을 처리하는 편의 기능을 제공합니다. (Delay, Debounce, Throttle, Buffer)

## Skill

### 언어

- JS / TS
- Java

### 프레임워크 / 라이브러리

- Web : Spring / NestJS / Express.js
- DB : Prisma / FxSQL
- Test : JUnit / AssertJ / Mockito / Jest
- UI : React
- Utility : RxJS / FxJS / FxTS

### 인프라 / 데브옵스 / AWS

- Docker
- EC2 / ECS / ECR / Lambda / SQS / S3

## Education

### 동국대학교 / 수학교육과 (2011.03 ~ 2017.02)

- 학점 : 3.9 / 4.5

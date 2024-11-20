## 주요 링크

- S3 버킷 웹사이트 엔드포인트: http://myhanghaebucket0.s3-website.ap-northeast-2.amazonaws.com
- CloudFrount 배포 도메인 이름: https://d1t6nufmqe3bvc.cloudfront.net

## 주요 개념

### GitHub Actions과 CI/CD 도구

- Continuous Integration / Continuous Deployment
  코드 변경 시 자동으로 빌드하고 배포하는 과정
- Github Actions
  Gihub에서 제공하는 CI/CD 도구, 레포지토리와 연결하여 설정 가능

### S3와 스토리지

- 스토리지
  디지털 데이터를 저장하는 공간
  클라우드 스토리지는 인터넷 서버를 통해 데이터를 저장하고 관리
- S3
  Amazon Simple Storage Service
  aws가 제공하는 객체 스토리지 서비스
  프론트엔드 개발자는 주로 build 정적 파일(HTML, CSS, JavaScript, 이미지 등)을 저장하고 제공하는데 사용

### CloudFront와 CDN

- CDN
  Content Delivery Network
  전 세계에 분산된 서버 네트워크를 사용하여 사용자에게 더 빠르고 안정적으로 웹 콘텐츠를 제공하는 시스템
  웹사이트의 로딩 속도를 빠르게 하고, 서버의 부하를 줄이므로 사용자 경험 향상으로 이어짐
- CloudFront
  aws가 제공하는 콘텐츠 전송 네트워크 서비스

### 캐시 무효화(Cache Invalidation)

- CDN에 저장된 이전 버전의 캐시 데이터를 새 데이터로 교체하여 변경된 리소스가 즉시 반영되도록 하는 프로세스

### Repository secret과 환경변수

- 환경변수
  프로그램이 실행되는 환경에 따라 동적으로 설정 될 수 있는 값
  민감한 정보를 더 유연하고 안전하게 관리할 수 있음
- Repository secret
  GitHub와 같은 저장소에서 사용하는 암호화된 환경변수
  GitAction과 같은 CI/CD 작업에서 클라우드 서비스에 연결하기 위해 필요한 api 키나 토큰을 안전하게 보호하여 전달 가능

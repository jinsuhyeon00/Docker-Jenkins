Jenkins
![image](https://github.com/jinsuhyeon00/Docker-Jenkins/assets/79950254/ed8212ac-1602-429c-aee5-f621b71073a2)


젠킨스 - 소프트웨어 개발 시 지속적으로 통합(CI : Continuous Integration) 서비스를 제공하는 툴
CI (Continuous Integration) : 여러 개발자들의 코드를 계속해서 통합하는 것
CD (Continuous Delivery) : 개발자들이 코드를 계속 작성하면, 사용자 및 내부 사용자들이 계속 쓸수 있게 만드는 것


젠킨스 설치
![젠킨스](https://github.com/jinsuhyeon00/Docker-Jenkins/assets/79950254/aac3e756-83b2-4014-b41a-8d93939e9546)

gigHub 연결
![깃 연결](https://github.com/jinsuhyeon00/Docker-Jenkins/assets/79950254/8a444881-26b2-4001-b449-aae2cf8a8125)

빌드 및 배포 프로젝트 연결

Pipeline
Pipeline script - 직접적으로 젠킨스 웹 대시보드에서 파이프라인 스크립트를 입력하는 것
* 파이프라인 스크립트는 Jenkinsfile이라고도 하며, Groovy 스크립트로 작성된다.
* 이 방법은 간단한 파이프라인을 정의할 때 유용하지만, 스크립트를 변경할 때마다 Jenkins를 다시 로드해야 하므로 유연성이 떨어진다.

Pipeline script from SCM - 파이프라인 스크립트를 소스 코드 관리(SCM) 시스템(예: Git, Subversion 등)에 저장한 다음 젠킨스에서 해당 스크립트를 가져오는 것
* 일반적으로 Jenkinsfile을 프로젝트 리포지토리에 포함시켜서 사용
* 스크립트 변경이 있을 때 소스 코드 관리 시스템에서 스크립트를 업데이트하면 Jenkins는 자동으로 변경된 스크립트를 가져와 실행할 수 있다.
* 이 방법은 스크립트의 유연한 관리와 버전 관리를 가능하게 한다.

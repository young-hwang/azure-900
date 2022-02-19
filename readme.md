# 1. 핵심 Azure 개념

## 1. 클라우드 컴퓨팅

인터넷을 통한 컴퓨팅 서비스 제공

서버, 스토리지, 데이터베이스, 네트워킹, 소프트웨어, 분석 및 인텔리전스가 포함

신속한 혁신, 유연한 리소스, 규모의 경제성을 제공

다른 사람이 운영하는 데이터 센터에서 컴퓨팅 성능 및 스토리지를 임대하는 방법

클라우드 리소스를 자체 데이터 센터의 리소스 처럼 취급

## 2. 요금이 저렴한 이유

종량제 가격 책정 모델 사용(사용한 만큼 청구)

사용하는 클라우드 서비스에 대해서만 비용 지불

사용이 끝난 리소스는 반환

클라우드 공급자는 사용자 대신 기본 인프라를 유지 관리

어려운 비즈니스 문제를 신속하게 해결하고 사용자에게 최첨단 솔루션 제공

- 운영비용 절감
- 인프라의 효율적 실행
- 비즈니스 요구 사항 변화에 따른 크기 조정

## 3. 클라우드 전환 이유

끊임없이 변화하는 디지털 세계

- 빠른 속도로 사용자에게 새로운 기능을 제공
- 사용자는 자신의 디바이스 및 소프트웨어로 보다 다양하고 포괄적인 활용 기대

더욱 빠르게 서비스 제공하고 위하여 아래의 주문형 액세스 제공

- 거의 제한 없는 컴퓨팅, 스토리지 및 네트워킹 구성 요소 풀
- 애플리케이션을 차별화하는데 도움되는 음성 인식 및 기타 인식 서비스
- 소프트웨어 및 디바이스에서 원격 분석 데이터를 제공하는 분석 서비스

## 4. Azure 란

비즈니스 과제를 해결하도록 돕는 지속적으로 확장 중인 일련의 클라우드 서비스

## 5. Azure 기능

- 미래 대비 : 지속적인 혁신으로 미래의 제품 비전 실현
- 조건부 빌드 : 오픈 소스에 대한 노력과 모든 언어 및 프레임워크 지원을 통해 원하는 방식으로 빌드하고 배포
- 원활한 하이브리드 운영 : 온-프레미스, 클라우드, 에지 등 원하는 위치에서 운영
- 신뢰할 수 있는 클라우드 : 능동적 규정 준수와 보안 전문가 팀의 지원을 통해 보안성 확보

## 6. Azure로 무엇을 할 수 있나?

클라우드는 가상 머신을 실행하기 위한 다른 장소 이상의 의미를 가짐

AI, 기계학습 서비스, 동적으로 확장되는 스토리지 솔루션 등

## 7. Azure 작동 방식

Azure는 private and public cloud plantform으로 개발자와 it 관리자의 빌드, 배포, 애플리케이션 관리를 돕니다.

Azure는 Virtualization 기술을 사용 한다.

Virtualization은 Hypervisor라는 추상화 layer를 사용하여 컴퓨터 하드웨어와 OS의 결합을 분리 시킨다.

Hypervisor는 물리적 컴퓨터의 모든 부분들을 emulate 하고 이것이 가상 머신 cpu가 된다.

제한된 하드웨어의 활용을 최적화 한다.

이는 동시에 여러개의 Virtual Machine을 가동시키고 각각의 Virtual Machine은 Windows, Linux 같은 operating system을 구동 할 수 있다.

Azure는 Virtualization technology 가지고 있고 전 세계 도처의 Microsoft data center의 거대한 스케일을 이용한다.

각각의 데이터 센터는 서버로 가득채워진 많은 랙을 가지며 각각의 서버는 multiple virtual machine을 구동하기 위한 Hypervisor를 포함하고 있다.

network switch는 이러한 서버들에 대하여 연결성을 제공한다.

<img src="https://github.com/young-hwang/azure-900/blob/main/img/1.png" width="50%" />

각각의 랙에 있는 하나의 서버는 Fabric Controller라 불리는 특별한 소프트웨어를 실행한다.

<img src="https://github.com/young-hwang/azure-900/blob/main/img/2.png" width="50%" />

각 Fabric Contorller는 흔히 Orchestrator라고 알려진 또 다른 특별한 소프트웨어와 연결 된다.

<img src="https://github.com/young-hwang/azure-900/blob/main/img/3.png" width="50%" />

Orchestrator는 Azure에서 사용자 요청에 응답하는 것을 포함하여 일어나는 모든 일을 책임진다.

<img src="https://github.com/young-hwang/azure-900/blob/main/img/4.png" width="50%" />

사용자들은 Orchestrator의 web API를 사용하여 요청한다.

web API는 Azure Portal의 사용자 Inteface를 포함한 다양한 툴들로 부터 요청이 되어 질 수 있다.

사용자가 새로운 Virtual Machine을 생성하는 요청을 만들었을 때 Orchestrator packges의 모든 것 들이 필요해진다.

최상의 Server rack을 선택하고 package를 전송과 fabric controller에 요청을 한다.

Fabric Controllers가 virtual machine이 생성되어 졌을 때 사용자는 이것에 접근 할수 있다.

## 8. Azure Portal

Azure Portal은 명령줄 도구의 대안을 제공하는 웹 기반의 통합 콘솔이다.

- 간단한 웹앱에서 복잡한 클라우드 배포까지 모든 것을 구축, 관리 및 모니터링
- 리소스를 편하게 볼수 있는 사용자 지정 대시보드
- 내게 필요한 옵션을 구성하여 최적의 환경 설정

## 9. Azure Marketplace

Azure에서 실행되도록 최적화된 솔루션과 서비스를 제공하는 Microsoft 파트너, 독립 소프트웨어 공급업체, 스타트업을 사용자와 연결해 준다.
모든 솔루션 및 서비스는 Azure에서 실행되도록 인증된 것이다.

## 10. Azure 서비스 둘러보기

가장 일반적으로 사용되는 범주

- Compute
- 웹
- 네트워킹
- IoT(사물 인터넷)
- 스토리지
- 빅 데이터
- 모바일
- AI
- 데이터 베이스
- DevOps

### a. Compute

컴퓨팅 서비스는 회사가 Azure 플랫폼으로 이전하는 주된 이유이다. Azure에서는 애플리케이션 및 서비스를 호스팅하는 다양한 옵션을 제공한다.

|서비스 이름|서비스 기능|
|:--|:--|
|Azure Virtual Machine|Azure에서 호스트된 Windows 또는 Linux VM(가상 머신)|
|Azure Virtual Machine Scale Sets|Azure에서 호스트된 Windows 또는 Linux VM의 스케일링|
|Azure Kubernetes Service|컨테이너화된 서비스를 실행하는 VM을 위한 클러스트 관리|
|Azure Service Fabric|Azure 또는 온-프레미스에서 실행되는 분산 시스템 플랫폼|
|Azure Batch|병렬 및 고성능 컴퓨팅 애플리케이션을 위한 관리 서비스|
|Azure Container Instance|서버 또는 VM을 ***프로비저닝***하지 않고 Azure에서 실행되는 컨테이너화된 앱|
|Azure Functions|이벤트 기반의 서버리스 컴퓨팅 서비스|

### b. 네트워킹

컴퓨팅 리소스를 연결하고 애플리케이션에 대한 액세스를 제공하는 것이 Azure 네트워킹의 주요 기능이다.

Azure의 네트워킹 기능에는 글로벌 Azure 데이터 센터의 서비스 및 기능을 외부 환경에 연결하는 다양한 옵션이 포함되어 있다.

|서비스 이름|서비스 기능|
|:--|:--|
|Azure Virtual Network|수신 VPN(가상 사설망) 연결에 VM을 연결|
|Azure Load Balancer|애플리케이션 또는 서비스 엔드포인트에 대한 인바운드 및 아웃바운드 연결의 균형을 맞춤|
|Azure Application Gateway|애플리케이션 보안을 강화하는 동시에 앱 ***서버 팜*** 제공을 최적화|
|Azure VPN Gateway|고성능 VPN 게이트웨이를 통해 Azure 가상 네트워크에 액세스|
|Azure DNS|매우 빠른 DNS 응답과 매우 높은 도메인 가용성 제공|
|Azure Content Delivery Network|전 세계 고객에게 고대역폭 콘텐츠 제공|
|Azure DDoS Protection|Azure에서 호스트되는 애플리케이션을 DDoS 공격으로 보호|
|Azure Traffic Manager|전 세계 Azure 지역에 네트워크 트래픽 분산|
|Azure ExpressRoute|고대역폭 전용 보안 연결을 통해 Azure 연결|
|Azure Network Watcher|시나리오 기반 분석을 사용하여 네트워크 문제를 모니터링하고 진단|
|Azure Firewall|스케일링 성능에 제한이 없고 보안 수준이 높은 고가용성 방화벽 구현|
|Azure Virtual WAN|로컬 사이트와 원격 사이트를 연결하는 통합 WAN(광역 네트워크) 구축|

### c. Storage

공통 특성
- 중복 및 복제 기능을 갖추고 있어 내구성과 가용성이 뛰어남
- 자동 암호화와 역할 기반 액세스 제어를 통해 보안을 유지
- 스토리지 제한이 없어 확장성이 뛰어남
- 유지 관리 및 사용자에 대한 중요한 문제를 관리
- HTTP 또는 HTTPS를 통해 전 세계 어디에서나 액세스

|서비스 이름|서비스 기능|
|:--|:--|
|Azure Blob Storage|비디오 파일이나 비트맵 같은 대규모 개체를 위한 스토리지 서비스|
|Azure File Storage|파일 서버처럼 액세스하고 관리할 수 있는 파일 공유|
|Azure Queue Storage|애플리케이션 간 메세지 큐에 넣고 안정적으로 전달하기 위한 데이터 저장소|
|Azure Table Storage|비관계형 정형 데이터(정형 NoSQL 데이터)를 클라우드에 저장하여 키/특성 스토어에 스키마 없는 설계 제공|

### d. Mobile

개발자가 iOS, Android 및 Windows 앱용 모바일 백 엔드 서비스를 쉽고 빠르게 만들수 있다.

- 오프라인 데이터 동기화
- 온-프레미스 데이터 연결
- 푸시 알림 브로드캐스트
- 비즈니스 요구 사한과 일치하다록 자동 크기 조정

### e. Database

Azure에서는 다양한 형식과 볼륨의 데이터를 저장하도록 여러 데이터 베이스 서비스 제공

|서비스 이름|서비스 기능|
|:--|:--|
|Azure Cosmos DB|NoSQL 옵션을 지원하는 글로벌 분산형 데이터베이스|
|Azure SQL Database|자동 스케일링과 필수 인텔리전스, 강력한 보안으로 관리되는 관계형 데이터베이스|
|Azure Database for MySQL|고가용성, 보안이 포함된 스케일링 가능한 MySQL 관계형 데이터베이스|
|Azure Database for PostgreSQL|고가용성, 보안이 포함된 스케일링 가능한 PostgreSQL 관계형 데이터베이스|
|Azure Virtual Machines SQL Server|클라우드에서 엔터프라이즈 SQL Server 앱을 호스트하는 서비스|
|Azure Synapse Anyalytics|추가 비용 없이 모든 스케일링 수준에서 필수 보안을 제공하며 완벽히 관리되는 데이터 웨어하우스|
|Azure Database Migration Service|애플리케이션 코드 변경 없이 데이터베이스를 클라우드로 마이그레이션하는 서비스|
|Azure Cache for Redis|자주 사용하는 정적 데이터를 캐시하여 데이터 및 애플리케이션 대기 시간을 줄이는 완전 관리형 서비스|
|Azure Database for MariaDB|고가용성, 보안이 포함된 스케일링 가능한 PostgreSQL 관계형 데이터베이스|

### f. Web

Azure에서는 웹앱 및 HTTP 기반 웹 서비스의 빌드 및 호스트에 대한 지원

|서비스 이름|서비스 기능|
|:--|:--|
|Azure App Service|클라우드 웹 기반 앱을 신속하게 만든다|
|Azure Notification Hubs|백 엔드에서 원하는 플랫폼으로 푸시 알림을 전송|
|Azure API Management|개발자, 파트너 및 직원에게 API를 안전하게 대규모로 게시|
|Azure Cognitive Search|완전 관리형 SaaS(Search as a Service)를 배포|
|Azure App Service의 Web Apps 기능|업무용 웹앱을 대규모로 만들고 배포|
|Azure SignalR Service|실시간 웹 기능을 쉽게 추가|

### g. IoT

여러 서브에서 Azure IoT를 위한 엔드투엔드 솔루션을 지원하고 구동


|서비스 이름|서비스 기능|
|:--|:--|
|IoT Central|대규모 IoT 자산의 연결, 모니터링 및 관리를 도와주는 완전 관리형 글로벌 IoT SaaS(Software as a Service) 솔루션|
|Azure IoT Hub|수백만 개의 IoT 디바이스 간에 안전한 통신 및 모니터링을 제공하는 메시징 허브|
|IoT Edge|데이터 분석 모델을 IoT 디바이스로 직접 푸시할 수 있는 완전 관리형 서비스로, 클라우드 기반 AI 모델 참조 필요 없이 상태 변화에 신속히 대응|

### h. Big Data

대량의 데이터를 말하며 모든 형식과 크기의 데이터에 지원 된다.
대규모 데이터 세트를 처리하기 위해 오픈 소스 클러스터 기술이 개발 되었다.

|서비스 이름|서비스 기능|
|:--|:--|
|Azure Synapse Analytics|대규모 병렬 처리를 활용하여 페타데이터 규모 데이터에서 복잡한 쿼리를 빠르게 실행하는 클라우드 기반 엔터프로이즈 데이터 웨어하우스|
|Azure HDInisght|클라우드의 관리형 Hadoop 클러스터를 사용하여 대규모 데이터를 처리|
|Azure Databricks|Apache Spark 기반의 공동 작업용 분석 서비스를 Azure의 다른 빅 데이터 서비스와 통합|

### i. AI

클라우드 컴퓨팅과 관련된 AI는 광범위한 서비스에 기반하며 이러한 서비스 중에는 기계 학습이 핵심이다.
머신러닝은 컴퓨터에서 기존 데이터를 사용하여 미래 동작, 결과 및 추세를 예측하는 데이터 과학 기술이다.
Machine Learning을 사용하면 컴퓨터에서 명시적으로 프로그래밍하지 않고 학습한다.

일반적인 AI 및 기계 학습 서비스 유형

|서비스 이름|서비스 기능|
|:--|:--|
|Azure Machine Learning Service|기계 학습 모델의 개발, 교육, 테스트, 배포, 관리 및 추적에 사용할 수 있는 클라우드 기반 환경이다. 모델을 자동으로 생성하여 사용자에 맞게 조정 할 수 있다. 로컬 머신의 학습을 시작한 다음, 클라우드로 확장 가능하다.
|Azure ML Studio|미리 빌드된 기계 학습 알고리즘 및 데이터 처리 모듈을 사용하여 기계 학습 솔루션을 빌드, 테스트, 배포 할 수 있는 공동 작업용 시각적 작업 영역이다.|

밀접한 관련이 있는 제품 세트를 Cognitive Services라고 하며 애플리케이션에서 이러한 미리 빌드된 API를 사용하여 복잡한 문제를 해결 한다.

|서비스 이름|서비스 기능|
|:--|:--|
|Vision|이미지 처리 알고리즘을 사용하여 사진 및 동영상을 스마트하게 식별, 캡셔닝, 인덱싱, 조정 한다.|
|Speech|음성을 텍스트로 변환하거나, 음성을 인증에 사용하거나, 앱에 화자 인식을 추가하다.|
|지식 매핑|지능형 추천 및 의미 체계 검색 등의 작업을 해결하기 위해 복잡하 정보와 데이터를 매핑 할 수 있다.|
|Bing Search|Add Bing Search API를 앱에 추가하고 단일 API 호출 기능을 활용하여 수십억 개의 웝 페이지, 이미지, 동영상 및 뉴스를 검색하는 기능을 사용한다.|
|자연어 처리|앱에서 미리 빌드된 스크립트를 사용하여 자연어를 처리하고, 감정을 평가하고, 사용자가 원하는 것을 인식하는 방법을 학습하도록 한다.|

### j. DevOps

DevOps는 사람, 프로세스 및 기술 통합을 통해 소프트웨어 제공을 자동화하여 사용자에게 지속적인 가치를 제공한다. Azure DevOps를 사용하여 애플리케이션에 연속 통합, 제공 및 배포를 제공하는 빌드 및 릴리스 파이프라인을 만들 수 있다. 리포지토리 및 애플리케이션 테스트를 통합하고, 애플리케이션 모니터링을 수행하고, 빌드 아티팩트로 작업할 수 있다. 또한 추적용 백로그 항목으로 작업하고, 인프라 배포를 자동화하고, Jenkins 및 Chef와 같은 광범위한 타사 도구 및 서비스를 통합할 수 있다. 이러한 모든 기능과 그 외 여러 기능은 Azure와 긴밀하게 통합되므로 애플리케이션의 일관적이고 반복 가능한 배포가 가능하여 빌드 및 릴리스 프로세스가 간소화된다.

|서비스 이름|서비스 기능|
|:--|:--|
|Azure DevOps|고성능 파이프라인, 무료 개인 Git 리포지토리, 구성 가능한 Kanban보드, 광범위한 자동화 및 클라우드 기반 부하 테스트와 같은 개발 공동 작업 도구를 사용한다. 이전 Visual Studio Team Service로 알려져 있다.|
|Azure DevTest Labs|배포 파이프라인에서 바로 애플리케이션을 테스트하거나 시연하기 위해 주문형 Windows 및 Linux 환경을 신속하게 만들수 있다.|

## 11. Azure 계정 시작

Azure 서비스를 만들고 사용하려면 Azure 구독이 필요하다. 자체 애플리케이션 및 비즈니스 요구 사항을 해결할 때는 Azure 계정을 만들어 구동을 생성하여야 한다. Azure 계정을 만든 후에는 추가 구독을 무료로 만들 수 있다.

<img src="https://github.com/young-hwang/azure-900/blob/main/img/5.png" width="50%" />

## 12. Azure 계정 만들기

Azure 웹 사이트에서 가입하여 Microsoft에서 직접 또는 Microsoft 담당자, Microsoft 파트너를 통해 Azure 액세스 권한을 구매 할 수 있다.

## 13. Azure 체험 계정이란

- 12개월간 인기 있는 Azure 제품에 대한 무료 액세스
- 처음 30일 동안 사용할 크레딧
- 항상 무료로 제공되는 25개 이상의 제품에 대한 액세스

가입 시 전화번호, 카드번호, Microsoft 또는 Github 계정 필요

## 14. Azure 체험 학생 계정

- 12개월간 특정 Azure 서비스에 비용 없이 액세스
- 처음 12개월 동안 사용할 크레딧
- 특정 소프트웨어 개발자 도구에 비용 없이 액세스

신용카드 없이 가입가능

## 15. Learn 샌드박스

많은 Learn 연습에서는 Azure 계정에 추가되는 임시 구독을 만드는 샌드박스라는 기술을 사용한다. 임시 구독을 통해 Learn 모듈 기간 동안 Azure 리소스를 만들수 있다.

# 2. Azure의 기본 개념 설명

## 1. Public, Private, Hybrid Cloud

클라우드 컴퓨팅의 세 가지 배포 모델은 'Public Cloud', 'Private Cloud', 'Hybrid Cloud'이다. 클라우드에 마이그레이션 할 때는 각 배포 모델의 다른 측면을 고려해야 한다.

|배포 모델|설명|
|:--|:--|
|Public Cloud|서비스는 공용 인터넷을 통해 제공되고 서비스를 구매하려는 누구에게나 제공된다. 서버, 스토리지와 같은 클라우드 리소스는 타사 클라우드 서비스 공급자가 소유하고 운영하며 인터넷을 통해 제공된다.|
|Private Cloud|하나의 기업 또는 조직의 선택된 사용자만 독점적으로 사용하는 컴퓨팅 리소스로 구성된다. 조직의 온사이트(온-프레미스)데이터 센터에 있을 수 있거나 타사 서비스 공급자가 호스트 할 수 있다.|
|Hybrid Cloud|Public Cloud와 Private Cloud간에 데이터 및 애플리케이션을 공유할 수 있도록하여 두 클라우드를 결합하는 컴퓨팅 환경이다.|

## 2. Cloud 모델 비교

### Public Cloud

- 확장 시 자본 지출이 없다.
- 애플리케이션을 신속하게 프로비전 및 프로비전 해제할 수 있다.
- 조직은 사용하는 항목에 대해서만 비용을 지불한다.

### Private Cloud

- 시작 및 유지 관리를 위해 하드웨어 구매해야 한다.
- 조직이 리소스 및 보안을 완전히 제어 할 수 있다.
- 조직이 하드웨어 유지 관리 및 업데이트를 담당한다.

### Hybrid Cloud

- 최고의 유연성을 제공한다.
- 조직이 애플리케이션을 실행할 위치를 결정한다.
- 조직이 보안, 규정 준수 또는 법적 요구 사항을 제어 한다.

## 3. Cloud Computing의 이점

- 고가용성 : 선택한 SLA(서비스 수준 계약)에 따라, 클라우드 기반 앱은 문제가 발생할 경우에도 명백한 가동 중지 시간 없이 지속적인 사용자 환경 제공
- 확장성 : 클라우드 앱을 '수직' 및 '수평'으로 스케일링 할 수 있다.
- 탄력성 : 자동 스케일링을 활용하도록 클라우드 기반 앱을 구성하여 앱에 필요한 리소스를 항상 제공
- 민첩성 : 앱 요구 사항이 변경되면 신속하게 클라우드 기반 리소스를 배포하고 구성
- 지리적 배포 : 전 세계 지역 데이터 센터에 앱과 데이터를 배포 할 수 있으므로 고객이 지역에서 항상 최고의 성능을 유지
- 재해 복구 : 클라우드 기반 뱁업 서비스, 데이터 복제 및 지역 배포를 활용하여 재해가 발생하더라도 데이터를 안전하게 유지

## 4. 자본 비용 및 운영 비용

- CapEx(자본 비용) : 물리적 인프라 비용을 초기에 지출한 다음, 시간이 지남에 따라 초기 비용을 공제한다. 초기 비용은 시간이 지남에 따라 가치가 감소한다.
- OpEx(운영 비영) : 현재 서비스 또는 제품에 대해 지출되어 청구되는 비용. 지출하는 동일 연도에 공제 할 수 있다. 초기 비용은 없으며 서비스 또는 제품을 사용하는 비용을 지불한다.

## 5. Cloud Computing은 사용량 기반 모델

클라우드 서비스 공급자는 사용량 기반 모델로 운영된다.
사용량 기반 모델은 다음과 같은 이점이 있다.

- 선불 비용이 없다.
- 사용자가 최대한 활용하지 못할 수도 있는 값비싼 인프라를 구입하고 관리할 필요가 없다.
- 필요한 경우 추가 리소스의 요금을 지불 할 수 있다.
- 더 이상 필요하지 않은 리소스 사용 요금을 지불하지 않다록 할 수 있다.

## 6. Cloud Service Model

|모델|정의|설명|
|:--|:--|:--|
|IaaS|Infrastructure-as-a-Service|물리적 서버 관리에 가장 가깝다. 클라우드 공급자가 하드웨어를 최신 상태로 유지하지만 운영 체제 유지 관리 및 네트워크 구성은 클라우드 테넌트가 담당한다.|
|PaaS|PaaS|관리형 호스팅 환경이다. 클라우드 공급자가 가상 머신 및 네트워킹 리소스를 관리하고 클라우드 테넌트가 애플리케이션을 관리형 호스팅 환경에 배포한다.|
|SaaS|SaaS|클라우드 공급자는 가상 머신, 네트워킹 리소스, 데이터 스토리지, 애플리케이션 등 애플리케이션 환경의 모든 측면을 관리한다. 클라우드 테넌트는 클라우드 공급자가 관리하는 애플리케이션에 데이터만 제공한다.|

<img src="https://github.com/young-hwang/azure-900/blob/main/img/6.png" width="50%" />

## 7. IaaS

가장 유연한 범주의 클라우드 서비스
애플리케이션을 실행하는 하드웨어를 완벽하게 제어
하드웨어를 구입하는 대신 IaaS를 통해 임대

### 장점

- CapEx 없음 : 초기비용 없음
- 민첩성 : 애플리케이션에 신속하게 액세스, 필요한 경우 프로비저닝 해제
- 관리 : 공유 책임 모델에 적용, 사용자는 프로비저닝 관리 및 유지, 클라우드 공급자는 클라우드 인프라를 관리 및 유지
- 사용량 기반 모델 : OpEx 모델로 사용 및 운영하는 리소스 비용만 지불
- 기술 : 깊은 기술이 없이도 퍼블릭 클라우드를 배포 및 사용
- 클라우드 이점 : 클라우드 공급자의 기술과 전문 지식을 활용하여 워크로드 보안 및 고가용성 보장
- 유연성 : 가장 유연한 서비스, 하드웨어 구성 및 관리를 제어

## 8. PaaS

IaaS와 이점 및 고려 사항이 동일하지만 몇가지 추가 사항 존재

### 장점

- CapEx 없음
- 민첩성 : IaaS보다 민첩성이 뛰어남, 사용자가 애플리케이션 서버 구상 필요 없음
- 사용량 기반 모델
- 기술
- 클라우드 이점
- 생산성 : 클라우드 공급자가 모든 플랫폼 관리를 처리하므로 사용자는 애플리케이션 개발에만 집중, 인터넷을 통해 플랫폼에 액세스하므로 서비스로서의 분산팀을 운영하기 더 쉽다. 보다 쉽게 전 세계에서 사용하도록 설정 할 수 있다.

### 단점

- 플랫폼 제한 사항 : 몇몇 클라우드 플랫폼 제한 사항이 애플리케이션 실행 방식에 영향을 줄 수 있다.

## 9. SaaS

사용자와 최종 사용자 또는 고객을 위해 중앙에서 호스트 및 관리되는 소프트웨어
모든 고객이 한 가지 애플리케이션 버전을 사용하고 월간 또는 연간 구독을 통해 라이선스가 부여 되는 아키텍처를 기반으로 한다.
IaaS와 동일하지만 몇 가지 추가 사항 존재

### 장점

- CapEx 없음
- 민첩성 : 사용자가 직원에게 최신 소프트웨어에 대한 액세스 권한을 빠르고 쉽게 재공
- 종량제 가격 책정 모델 : 사용자는 소프트웨어 사용량과 관계없이 매월 또는 매년 구독 모델에서 소프트웨어 비용 지불
- 기술 : 뛰어난 기술 없이도 SaaS를 배포 및 사용
- 유연성 : 사용자가 어디서든 동일한 애플리케이션 데이터에 액세스

### 단점

- 소프트 웨어 제한 사항 : 소프트웨어 애플리케이션의 몇 가지 제한 사항이 사용자의 작업 방식에 영향, 소프트웨어를 있는 그대로 사용하므로 기능을 직접제어 할 수 없음

## 10. 클라우드 서비스 모델 비교

|IaaS|PaaS|SaaS|
|:--|:--|:--|
|가장 유연한 클라우드 서비스|애플리케이션 개발에 집중|종량제 가격 책정 모델|
|사용자가 애플리케이션을 위한 하드웨어 구성 및 관리|클라우드 공급자가 플랫폼 관리 담당|구독 모델로 비용을 지불|

<img src="https://github.com/young-hwang/azure-900/blob/main/img/7.png" width="50%" />

## 11. 서버리스 컴퓨팅

PaaS와 마찬가지로 서버리스 컴퓨팅을 사용하면 개발자가 인프라를 관리할 필요 없이 빠르게 애플리케이션을 빌드할 수 있다.
서버리스 애플리케이션에서는 클라우드 서비스 공급자가 코드 실행에 필요한 인프라를 자동으로 프로비저닝, 스케일링 및 관리 한다.
서버리스 아키텍처는 스케일링 성능이 뛰어나고 이벤트 기반이므로 특정 기능 또는 트리거가 발생할 때만 리소스를 사용한다.
코드는 여전히 서버에서 실행된다.
“서버리스”라는 이름은 인프라 프로비저닝 및 관리와 관련된 작업이 개발자에게 표시되지 않는다는 점에서 유래한다.
이 방식을 통해 개발자는 비즈니스 논리에 더욱 집중하고 비즈니스 핵심에 더 많은 가치를 제공할 수 있다.
서버리스 컴퓨팅을 통해 팀은 생산성을 향상하고 제품 출시를 단축할 수 있으며 조직은 리소스를 최적화하고 계속해서 혁신에 집중할 수 있다.

# 3. 핵심 Azure 아키텍처 구성 요소 설명

## 1. Azure 구독, 관리 그룹, 리소스 개요

<img src="https://github.com/young-hwang/azure-900/blob/main/img/5.png" width="50%" />

- 리소스 : 가상 머신, 스토리지 또는 SQL 데이터베이스와 같이 사용자가 만든 서비스의 인스턴스
- 리소스 그룹 : 리소스는 리소스 그룹으로 결합. 웹앱, 데이터베이스, 스토리지 계정과 같은 Azure 리소스가 배포되고 관리되는 논리적 컨테이너 역할
- 구독 : 사용자 계정과 해당 사용자 계정에서 만든 리소스를 그룹화. 각 구독에 대해 만들고 사용할 수 있는 리소스의 양에 제한 또는 할당이 있다. 팀 또는 프로젝트에서 만든 리소스 및 그로 인한 비용을 관리할 수 있다.
- 관리 그룹 : 여러 구독에 대한 액세스, 정책 및 규정 준수를 관리하는데 도움. 관리 그룹에 속한 모든 구독은 관리 그룹에 적용된 조건을 자동 상속.

## 2. Azure 지역, 가용성 영역 및 지역쌍

### 1. Azure 지역

지역이란 가까운 곳에 있고 대기 시간이 짧은 네트워크를 통해 연결된 데이터 센터를 하나 이상 포함하고 있는 지리적 영역.
Azure는 각 Azure 지역의 리소스를 지능적으로 할당하고 제어하여 워크로드의 적절한 균형을 유지함.
리소스 배포 할 때 Azure 지역을 선택해야 하는 경우가 자주 있음.

Azure Active Directory, Azure Traffic Manager, Azure DNS는 특정 Azure 지역 선택 필요 없음(글로벌 Azure 서비스)

### 2. 지역이 중요한 이유

사용자가 어디에 있든 사용자와 더욱 가까운 위치에서 애플리케이션을 제공.
글로벌 지역은 향상된 확장성 및 중복성을 제공.
서비스의 데이터 보존을 유지.

### 3. 특수 Azure 지역

규정 준수 또는 법적 목적에 맞게 애플리케이션을 빌드할 때 사용할 수 있는 특수 Azure 지역 존재.

- US DoD 중부, US Gov 버지니아, US Gov 아이오와 등 : 미국 정부 기관 및 파트너를 위한 물리적 및 논리적 네트워크로 격리된 Azure 인스턴스. 선별된 미국인이 운영. 추가 규정 준수 인증서를 포함.
- 중국 동부, 중국 북부 등 : Microsoft 및 21Vianet 간의 고유한 파트너십을 통해 사용. Microsoft에서 데이터 센터를 직접 관리하지 않음.

### 4. Azure 가용성 영역

장애 발생시 정보를 보호 할 수 있도록 서비스와 데이터를 중복시킴. 인프라 호스트 시 자체적으로 중복성 설정하려면 중복된 하드웨어 환경을 구축해야함. 가용성 영역을 통해 앱의 가용성을 높일 수 있음.

### 5. 가용성 영역이란?

Azure 지역 내에서 물리적으로 분리된 데이터 센터. 각 가용성 영역은 독립된 전원, 냉각 및 네트워킹을 갖춘 하나 이상의 데이터 센터로 구성. 가용성 영역은 격리 경계로 설정. 한 영역이 다운되어도 다른 영역은 계속 작동. 고속 프라이빗 광 네트워크로 연결.

### 6. 앱에서 가용성 영역 사용

가용성 영역을 사용하여 중요 업무용 애플리케이션을 실행 할 수 있으며, 한 영역 내에 컴퓨팅, 스토리지, 네트워킹 및 데이터 리소스를 공동 배치하고 다른 영역에 복제하여 애플리케이션 아키텍처에 고가용성을 구현 할 수 있음.(영역 간에 데이터 전송하는 비용 발생)
가용성 영역은 주로 VM, 관리 디스트, 부하 분산 장치 및 SQL 데이터베이스에 주로 사용.

- 영역 서비스 : 특정 영역(VM, 관리 디스크, IP 주소)에 리소스를 고정
- 영역 중복 서비스 : 플랫폼이 영역에서 자동으로 복제(영역 중복 스토리지, SQL 데이터베이스)
- 비지역 서비스 : Azure 지역에서 항상 사용할 수 있으며 영역 전체 중단뿐만 아니라 지역 전체 중단도 복원

### 7. Azure 지역 쌍

가용성 영역은 하나 이상의 데이터 센터를 사용하여 만들어짐. 단일 지역에는 최소 세 개의 영역이 존재. 두 데이터 센터 모두 중단 될 수 있는 대규모 재해 발생 가능성 있음. 이러한 이유로 Azure는 항상 Azure 지역 쌍을 만듬.

### 8. Azure 지역 쌍이란?

각 Azure 지역은 300마일 이상 떨어져 있는 동일한 지리적 위치내의 다른 Azure 지역과 항상 쌍을 이룸.
이 방법을 통해 한 지리적 위치에서 VM 스토리지 같은 리소스를 복제 할 수 있으며, 두 Azure 지역에 동시에 영향을 주는 자연재해, 내전, 정전 또는 물리적 네트워크 중단 등의 이벤트 때문에 서비스가 중단 될 가능성을 줄임.
Azure 지역 쌍의 예로는 미국 동부와 미국 서버 쌍, 동남 아시아와 동아시아 쌍이 있다.
Azure 지역 쌍은 직접 연결되고 Azure 지역 규모의 재해를 피할 수 있도록 충분히 멀리 떨어져 있기 때문에 안정적인 서비스 및 데이터 중복성을 제공하는데 사용 할 수 있음. 일부 서비스는 Azure 지역 쌍을 사용하여 자동 지역 중복 스토리지를 제공.

Azure 지역 쌍의 추가적인 이점
- 광범위한 Azure 중단이 발생하는 경우 해당 지역 쌍에서 호스트되는 애플리케이션에 대해 하나 이상의 지역이 가능한 한 빨리 복원되도록 하기 위해 모든 쌍 중에서 하나의 지역이 우선하도록 지정
- 계획된 Azure 업데이트는 가동 중지 및 애플리케이션 중단 위험을 최소화하기 위해 한 번에 한 Azure 지역 쌍으로 롤아웃.
- 데이터는 세금 및 법률 집행 관할 구역에 사용될 수 있게 동일한 지리적 위치 내에 쌍으로 상

## 3. Azure 리소스 및 Azure Resource Manager

- 리소스 : Azure를 통해 사용 할 수 있는 관리 가능한 항목.(VM, 소토리지 계정, 웹앱, 데이터베이스 등)
- 리소스 그룹 : 리소스를 보관하는 컨테이너. 리소스 그룹은 그룹으로 관리하려는 리소스만 포함.

### 1. Azure 리소스 그룹

Azure 플랫폼의 기본 요소. 리소스의 논리 컨테이너.
모든 리소스는 리소스 그룹에 있어야하고 한 리소스는 단일 리소스 그룹의 멤버이다. 리소스 그룹은 중첩 할 수 없다.

### 2. 논리적 그룹화

리소스 그룹의 용도는 Azure 리소스를 관리하고 구성. 각
사용량, 형식 또는 위차가 비슷한 리소스를 한 리소스 그룹에 배치하면 Azure에서 만드는 리소스에 질서를 부여하고 체계적으로 구성

### 3. 수명 주기

리소스 그룹을 삭제하면 그 안에 리소스도 모두 삭제
리소스 수명 주기 구성 시 실험 후 리소스를 폐기하는 환경에서 유용

### 4. 권한 부여

리소스 그룹은 RBAC(역할 기반 액세스 제어) 권한을 적용하는 범위
리소스 그룹에 RBAC 권한을 적용하면 관리 간편, 액세스 제한

## 4. Azure Resource Manager

Azure용 배포 및 관리 서비스.
Azure 계정에서 리소스 생성, 업데이트, 삭제하는 관리 계층 제공.
Azure Portal에서 사용할 수 있는 모든 기능은 PowerShell, Azure CLI, REST API 및 클라이언트 SDK를 통해서도 사용 가능

### 1. 리소스 관리자를 사용할 경우의 이점

- 스크립트가 아니라 선언적 템플릿을 통해 인프라 관리. Resource Manager Template은 Azure에 무엇을 배포하는지 정의하는 JSON 파일
- 리소스를 개별적으로 처리하는 대신, 솔루션의 모든 리소스를 그룹으로 배포, 관리 및 모니터링
- 개발 수명 주기 내내 솔루션을 다시 배포
- 리소스가 올바른 순서로 배포되도록 리소스 간의 종속성을 정의
- 모든 서비스에 액세스 제어를 적용
- 리소스에 태그를 적용하여 구독의 모든 리소스를 논리적으로 구성
- 동일한 태그를 공유하는 리소스 그룹에 대한 비용을 확인하여 조직의 청구를 명확히 함

## 5. Azure 구독 및 관리 그룹

### 1. Azure 구독

Azure를 사용하려면 Azure 구독 필요.
구독은 Azure 제품 및 서비스에 대한 인증되고 권한이 부여된 액세스 제공
계정에는 서로 다른 청구 모델 보유하고 다른 액세스 관리 정책을 적용하는 하나 또는 여러 개의 구독이 있음.
2가지 유형의 구독 경계를 사용

- 청구 경계 : Azure 사용에 따른 Azure 계정 청구 방식 결정. 다양한 유형의 청구 요구 사항에 따라 여러 개의 구독을 만듬.
- 액세스 제어 경계 : Azure 구독 수준에서 액세스 관리 정책을 적용. 다른 조직 구조를 반영하기 위해 별도의 구독을 만들 수 있음.

### 2. 추가 Azure 구독 만들기

- 환경 : 리소스를 관리할 때 개발 및 테스트, 보안을 위한 별도의 환경을 설정하거나 규정 준수 상의 이유로 데이터 격리 할 수 있음. 이 디자인은 리소스 액세스 제어가 구독 수준에서 발생하기 때문에 유용
- 조직 구조 : 여러 조직 구조를 반영하는 구독.
- 청구 : 청구를 위해 추가 구독을 만들 수 있음. 비용은 구독 수준에서 먼저 집계되므로 사용자의 요구에 따라 비용을 관리하고 추적하는 구독 생성
- 구독 제한 : 구독은 일부 하드 제한에 바인딩

### 3. 요구 사항에 맞게 청구 사용자 지정

구독이 여러 개인 경우 청구서 섹션으로 구성 할 수 있음.
각 청구 섹션은 해당 월에 발생한 요금을 보여 주는 청구서의 폼목.

## 6. Azure 관리 그룹

조직에 구독이 많은 경우 해당 구독에 대한 액세스, 정책 및 규정 준수를 효율적으로 관리하는 방법 필요.
구독을 관리 그룹이라고 하는 컨테이너에 구성하고 거버넌스 조건을 관리 그룹에 적용.
관리 그룹에 속하는 모든 구독은 관리 그룹에 적용되는 조건을 자동으로 상속.

### 1. 관리 그룹 및 구독의 계층 구조

리소스를 통합 정책 및 액세스 관리를 윈한 계층 구조로 구성하는 유연한 관리 그룹 및 구독 구조 만들수 있음

### 2. 관리 그룹에 대한 중요 한 사실

- 단일 디렉터리에서 지원할 수 있는 관리 그룹 수는 10,000개
- 관리 그룹 트리에서 지원할 수 있는 최대 깊이 수준은 6(루트 수준, 구독 수준 제외
- 각 관리 그룹 및 구독은 하나의 부모만 지원
- 각 관리 그룹에는 여러 자식 요소가 있을 수 있음
- 모든 구독 및 관리 그룹은 각 디렉터리의 단일 계층 내에 위치

# 1. Azure 컴퓨팅 서비스 살펴보기

## 1. Azure 컴퓨팅 서비스 개요

클라우드 기반 애플리케이션을 실행하기 위한 주문형 컴퓨팅 서비스.
디스크, 프로세서, 메모리, 네트워킹 및 운영 체제와 같은 컴퓨팅 리소스 제공.

- Azure Virtual Machine
- Azure Container Instances
- Azure App Service
- Azure Functions(Serveless Computing)

### 1. 가상 머신

가상 머신은 물리적 컴퓨터의 소프트웨어 에뮬레이션.
가상 프로세서, 메모리, 스토리지 및 네트워킹 리소스가 포함
운영 체제 호스트하고 소프트웨어 설치하고 실행.

- Azure Virtual Machines : 클라우드 VM을 만들고 사용. IaaS를 다양한 방법으로 제공.
- Azure Virtual Machine Scale Sets : 동일한 VM 세트를 배포 및 관리. 모든 VM은 동일하게 구성 되었으며 가상 머신 확장 집합은 실제 자동 크기 조정을 지원하도록 디자인.
- Container/Kubernetes : 컨테이너를 배포하고 관리하는 데 사용할 수 있는 Azure 컴퓨팅 리소스. 단일 가상 머신 호스트에서 컨테이너화된 애플리케이션의 여러 인스번스를 실행.
- App Service : 모든 플랫폼에서 실행되는 엔터프라이즈급 웹, 모바일 및 API 앱을 신속하게 빌드, 배포 및 스케일링. 완전 관리형 플랫폼. PaaS.
- Functions : 기본 플랫폼이나 인프라가 아닌, 서비스를 실행하는 코드에 관해서만 관심이 있는 경우 적합. Azure Functions는 이벤트, 타이머 또는 다른 Azure 서비스로부터 받은 메시지에 대한 응답으로 작업 수행. 해당 작업을 수초 이내에 빠르게 완료할 수 있을 경우 사용.

## 2. Azure Virtual Machines를 사용하는 경우 결정

- OS에 대한 완전한 제어
- 사용자 지정 소프트웨어 실행
- 사용자 지정 호스팅 구성

미리 구성된 가상 머신 이미지를 선택하면 짧은 시간 안에 가상 머신을 만들고 프로비저닝.
이미지는 가상 머신을 만드는 데 사용되는 템플릿.

### 1. VM을 사용하는 경우의 예시

- 테스트 및 개발 도중
- 클라우드에서 애플리케이션을 실행하는 경우
- 데이터 센터를 클라우드로 확장하는 경우
- 재해 복구 도중
### 2. VM을 사용하는 클라우드로 이동

VM은 물리적 서버에서 클라우드로 이동 할 때 좋음.
물리적 서버의 이미지를 만들고 거의 또는 전혀 변경할 필요 없이 가상 머닌 내에서 호스트
설치된 OS 및 해당 OS를 실행하는 소프트웨어를 업데이트

### 3. Azure에서 VM 스케일링

VM을 함께 그룹화하여 고가용성, 확장성 및 중복성을 제공.

- Azure Virtual Machine Scale Sets
- Azure Batch

### 4. Virtual Machine Scale Sets란

부하 분산된 동일한 VM 그룹을 만들고 관리.
가상 머신 복제 시 웝 사이트 가상 머신의 여러 인스턴스 간에 요청을 라우팅하는 추가 서비스 구성을 자동 수행

### 5. Azure Batch란

수십, 수백 또는 수천 개의 가상 머신으로 스케일링함으로써 대규모 병렬 및 고성능 컴퓨팅(HPC) 일괄 작업을 수행 할 수 있음

Batch 작업 수행

- 컴퓨팅 VM 풀을 시작
- 애플리케이션 및 준비 데이터를 설치
- 사용자의 여러 작업을 포함하는 작업 실행
- 오류를 식별
- 작업을 큐에 다시 놓음
- 작업 완료 시 풀을 스케일 다운

## 3. Azure App Service를 사용하는 경우 결정

인프라를 관리할 필요 없이 원하는 프로그래밍 언어로 웹앱, 백그라운드 작업, 모바일 백 엔드 및 RESTful API를 빌드하고 호스트 가능.
자동 확장과 고가용성 제공.
App Service는 Windows 및 Linux 지원.
GitHub, Azure DevOps 또는 Git 리포지토리에서 자동화된 배포를 사용.
PaaS

### 1. Azure App Service 비용

선택한 App Service 요금제에 따라 요청을 처리하는 동안 앱에서 사용하는 Azure 컴퓨팅 리소스에 대한 요금을 지급
App Service 요금제에 따라 호스트에 사용된 하드웨어 양이 결정.

### 2. App Service 유형

- 웹앱
- API 앱
- WebJobs
- 모바일 앱

웹에 액세스할 수 있는 앱 호스트 시 결정해야 하는 대부분 인프라 관련 사항 처리

- 배포와 관리 기능이 플랫폼에 통합
- 엔드포인트에 보안이 설정
- 높은 트래픽 부하를 처리하기 위해 사이트를 빠르게 스케일링
- 기본 제공 부하 분산 및 Traffic Manager가 고가용성 제공

### 3. 웹앱

ASP.NET, ASP.NET Core, Java, Ruby, Node.js, PHP 또는 Pyhton을 사용하여 웹앱 호스트가 전체 지원.

### 4. API Web

웹 사이트를 호스트하는 것처럼 원하는 언어 프레임워크를 사용하여 REST 기반 웹 API를 빌드할 수 있음.
전체 Swagger 지원과 함께 Azure Marketplace에서 API를 패키지 및 게시하는 기능을 사용 가능.
HTTP, HTTPS 기반 클라이언트에서 사용

### 5. Webjobs

웹앱, API 앱 또는 모바일 앱과 동일한 컨텍스트에서 프로그램 또는 스크립트 실행 가능
프로그램과 스크립트는 트리거를 통해 예약하거나 실행 가능
애플리케이션 로직의 일부로 백그라운드 작업을 실행하는데 사용

### 6. Mobile App

iOS 및 Android 앱의 백 엔드를 빠르게 빌드

- 클라우드 기반 SQL 데이터베이스에 모바일 앱 데이터 저장
- MSA, Google, Twitter 및 Facebook과 같은 일반적인 소셜 공급 기업에 대한 고객을 인증
- 푸시 알림 보냄
- C# 또는 Node.js에서 사용자 지정 백 엔드 논리를 실행

Native iOS/Android, Xamarin 및 React Native 앱을 위한 SDK 지원

## 4. Azure Container Instances/Azure Kubernetes Service를 사용하는 경우 결정

VM은 물리적 하드웨어에 필요한 투자 비용을 줄이는 좋은 방법이나 가상 머신당 단일 운영 체제로 제한
단일 호스트에서 애플리케이션의 여러 인스턴스를 실행하려는 경우 컨테이너 사용이 좋음

### 1. Container란

가상화 환경. 단일 물리적 호스트에서 여러 가상 머신을 실행하는 것과 매우 유사.
단일 물리적 또는 가상 호스트에서 여러 컨테이너를 실행 할 수 있음.
VM과 달리 컨테이너에 대한 운영 체제를 관리하지 않음.
VM은 연결하고 관리할 수 있는 운영 체제의 인스턴스인 것 같지만, 컨테이너는 저용량이며 동적 생성, 스케일 아웃 및 중지를 할 수 있도록 설계.

### 2. 가상 머신과 컨테이너 비교

VM : 하나의 운영 체제만 실행, 서로 다른 런타임 환경이 필요한 여러 응용 프로그램을 제대로 실행하려면 여러 가상 머신 필요.
전처 컴퓨터를 에뮬레이트, 컴퓨터를 시작하거나 스냅숏을 찍는 등의 작업이 느림
Container : 단일 앱과 해당 종속성을 번들로 묶은 다음 컨테이너 호스트에 배포.
컨테이너 호스트는 운영 체제와 인프라를 추상화하여 표준화된 런타임 환경 제공
컨테이너화된 응용 프로그램이 다른 컨테이너화된 앱과 나란히 실행.
운영체제 수준의 가상화는 가상 머신보다 효율적인 이유
컨테이너화된 앱은 크기가 훨씬 더 작은 경향이 있고, 개발 런타임 환경이 프로덕션 환경과 똑같이 보일수 있음.

### 3. 컨테이너 관리

컨테이너는 필요에 따라 애플리케이션 인스턴스를 시작, 중지, 스케일 아웃 할 수 있는 컨테이너 오케스트레이터를 통해 관리
Azure Container Instances / AKS(Azure Kubernetes Service)

Azure Container Instances

가상 머신을 관리하거나 추가 서비스를 채택하지 않고도 Azure에서 컨테이너를 실행하는 가장 빠르고 간단한 방법. PaaS

Azure Kubernetes Service

많은 컨테이너를 자동화, 관리 및 상호 작용하는 작업
분산형 아키텍처와 대량의 컨테이너가 있는 완벽한 컨테이너용 오케스트레이션 서비스

### 4. Kubernetes란

대규모 컨테이너화된 응용 프로그램의 요구를 처리하기 위한 관리 시스템 필요.
컨테이너 기반 워크로드를 관리하는 데 가장 인기 있는 옵션 중 하나가 Kubernetes.
컨테이너 관리 자동화와 확장 가능한 API를 결합 클라우드 네이티브 응용 프로그램 관리.
Kubernetes 클러스터 노드에서 하나 이상의 컨테이너로 구성된 Pod 배치 관리.
Pod 중 하나가 충돌하면 Kubernetes는 해당 Pod의 새인스턴스 생성.
클러스터 노드가 제거되면 Kubernetes에서 영향을 받는 워크로드를 클러스터의 다른 노드로 이동.
Kubernetes Pod는 규모 요구사항에 맞게 더 많거나 적은 처리량을 제공하도록 크기 조정
크기조정은 수평 Pod 크기조정을 통해 수동 또는 자동으로 트리거.
응용 프로그램 업데이트 시 가동 중지 최소화를 위해 지그재그 형태로 배치 및 이전 버전 롤백.
컨테이너 저장소와 네트워킹도 관리.
Kubernetes 영구 저장소는 하나 이상의 컨테이너에 데이터 저장소를 제공 가능.
이 구성을 사용하면 컨테이너에서 응용 프로그램 데이터를 읽고 쓸 수 있으며 여러 Pod 인스턴스 간에 이 데이터를 유지.
Kubernetes에서 실행되는 응용 프로그램에서 데이터 저장 및 검색을 위한 Azure Storage, Azure Cosmos DB 같은 클라우드 기반 저장소 및 데이터 시스템을 사용하는 것이 일반적.
Kubernetes network plugin은 Pod를 인터넷에 공개하고 여러 복제본 간에 트래픽 부하를 분산 네트워크 격리 및 정책 기반 네트워크 보안과 같은 기능 제공, Kubernetes 클러스터의 Pod 간 통신 및 이름 확인 관리.

### 5. 솔루션 컨테이너 사용

마이크로 서비스 아키텍처에서는 솔루션을 더 작고 독립적인 조각으로 분할 가능.

### 6. 마이크로 서비스란

규모가 작고 잘 정의된 범위의 웹 서비스. 다른 서비스와 느슨하게 결합.
하나의 마이크로 서비스를 구축하는게 아닌 각각 단일의 비즈니스 기능을 구현하는 마이크로 서비스의 컬렉션으로 구성된 마이크로 서비스 아키텍처를 채택.
각 서비스는 작은 개발 팀이 관리 할 수 있는 개별 코드베이스.
팀이 전체 응용 프로그램을 다시 빌드 후 재배포 하지 않고도 서비스를 업데이트 가능.
상호 종속성이 없이 각 마이크로 서비스를 완전히 자율적으로 운영.
결함 격리 계층을 제공.

## 5. Azure Functions를 사용하는 경우 결정

Serveless 컴퓨팅은 서버, 인프라 및 운영 체제의 추상화.
서버리스 컴퓨팅을 통해 서버 인프라 관리 및 수요에 따른 리소스 할당 및 할당 해제를 처리.
사용하는 정확한 리소스에 대해서만 요금이 청구.

- 서버의 추상화 : 서버리스 컴퓨팅은 실행하는 서버를 추상화. 서버 인스턴스 명시적으로 예약하지 않음. 플랫폼이 해당 기능을 관리. 각 함수 실행은 다른 컴퓨팅 인스턴스에서 실행.
- 이벤트 기반 크기 조정 : 예정된 이벤트에 응답하는 워크로드에 적합. 이벤트는 다음을 통해 수행되는 트리거(타이머, HTTP(API, 웹후크), 큐 등) 개발자는 함수를 작성하고 함수에는 트리거 및 바인딩에 관한 코드 및 메타데이터 모두 포함. 플랫폼은 자동으로 함수 실행을 예약, 예정된 이벤트의 비율에 따라 컴퓨팅 인스턴스의 수를 조정.
- 마이크로 청구 : 코드가 실행된는 시간에 대해서만 비용을 지불.

### 1. Azure의 서버리스 컴퓨팅

사용자를 대신해 서버 관리 작업이 이미 처리됨.
장점 : 인프라 관리가 없음. 확장성. 사용한 만큼 비용지급.

## 5. Azure Functions를 사용하는 경우 결정

서버리스 컴퓨팅은 서버, 인프라, 운영 체제의 추상화. 
서빈인프라 관리 및 수요에 따른 리소스 할당 및 할당 해제 처리

- 서버의 추상화 : 실행하는 서버 추상화. 서버 인스턴스 명식적 예약하지 않음. 플랫폼에서 관리. 각 함수는 다른 인스턴스에서 실행될 수 있음. 
- 이벤트 기반 크기 조정 : 예정된 이벤트에 응답하는 워크로드에 적합. 
- 마이크로 청구 : 

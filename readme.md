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



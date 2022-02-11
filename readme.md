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

Azure Portal은 명령줄 도구의 대안을 제공하는 

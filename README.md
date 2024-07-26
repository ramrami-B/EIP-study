# 🤓 정보처리기사 실기

# 1. 요구사항 확인

## 1. 소프트웨어 개발 방법론

### 1. 소프트웨어 개발 방법론

1. 소프트웨어 생명주기 모델
    - 소프트웨어 생명주기(SDLC): 시스템의 요구분석부터 유지사항까지 전 공정을 체계화한 절차
    - 순서: 요구사항 분석 → 설계 → 구현 → 테스트 → 유지보수 `요설구테유`
    - 모델 `폭프나반`
        - 폭포수(Waterfall) 모델
        - 프로토타이핑(Prototyping) 모델
        - 나선형(Spiral) 모델
        - 반복적(Iteration) 모델
2. 소프트웨어 개발 방법론
    - 종류: 구조적 방법론, 정보공학 방법론, 객체 지향 방법론, 컴포넌트 기반 방법론, 애자일 방법론, 제품 계열 방법론
    - 애자일(Agile)
        - 개념: 절차 보다는 사람이 중심이 되어 변화에 유연하고 신속하게 적응하면서 효율적으로 시스템을 개발 할 수 있는 방법론
        - 개발 기간이 짧고 신속하며 유동적
        - 유형
            - XP: 기본 원리 - 짝 프로그래밍(Pair Programming), 지속적인 통합(CI), 테스트 기반 개발(TDD), 리팩토링(Refactoring)
            - 린(Lean)
            - 스크럼(Scrum): 백로그(Backlog), 스프린트(Sprint), 스크럼 미팅, 스프린트 회고
3. 객체 지향 분석 방법론
    - 객체 지향(Object Oriented): 실세계의 개체를 속성과 메서드가 결합한 형태의 객체로 표현하는 기법
    - 구성 요소
        - 클래스(Class)
        - 객체(Object)
        - 메서드(Method)
        - 메시지(Message): 객체 간 상호 작용을 위한 수단, 객체에서 객체로 어떤 행위를 하도록 지시
        - 인스턴스(Instance): 클래스에 속한 각각의 객체, 실제로 메모리상에 할당
        - 속성(Property): 객체들이 가지고 있는 데이터 값
    - 기법 `캡상다추정관 (캡숑 다 추정관이네~!)`
        - 캡슐화(Encapsulation): 서로 연관된 데이터와 함수를 묶음, 결합도가 낮아지고 재사용에 용이
        - 상속성(Inheritance): 상위 클래스의 속성과 메서드를 하위 클래스에서 재정의 없이 물려받아 사용
        - 다형성(Polymorphism)
            - 오버로딩(Overloading): 매개변수의 유형과 개수가 다른 같은 이름의 메서드
            - 오버라이딩(Overriding): 상위 클레스에서 정의한 일반 메서드의 구현을 하위 클래스에서 재정의
        - 추상화(Abstraction): 공통 성질을 추출하여 추상 클래스 설정
        - 정보 은닉(Information Hiding): 코드 내부 데이터와 메서드를 숨기고 공개 인터페이스를 통해서만 접근이 가능하도록 함
        - 관계성(Relationship)
    - 원칙 (SOLID)
        - 단일 책임의 원칙(SRP): 하나의 클래스는 하나의 목적, 책임
        - 개방 폐쇄의 원칙(OCP): 확장에는 열려 있고, 변경에는 닫혀 있어야 함
        - 리스코프 치환의 원칙(LSP): 하위 클래스는 어디서나 상위 클래스로 교체 할 수 있다.
        - 인터페이스 분리의 원칙(ISP): 클래스에서 사용하지 않는 인터페이스는 구현하지 말아야 한다.
        - 의존성 역전의 원칙(DIP): 실제 사용 관계는 바뀌지 않으며 추상을 매개로 메시지를 주고 받음으로써 관계를 느슨하게
    - 럼바우 `객동기`
        - 객체(Object) 모델링: = 정보 모델링, 객체를 찾고 객체들 간 관계 정의, 객체 다이어그램
        - 동적(Dynamic) 모델링: 시간의 흐름에 따라 객체들 사이의 동적 행위 표현, 상태 다이어그램
        - 기능(Functional) 모델링: 자료 흐름을 중심으로 처리 과정 표현, 자료 흐름도

### 2. 프로젝트 관리

일단 넘어감

## 2. 현행 시스템 분석

### 1. 현행 시스템파악

1~3. 일단 넘어감

1. 디자인 패턴(Design Pattern): 소프트웨어 설계에서 공통으로 발생하는 문제에 대해 자주 쓰이는 설계 방법을 정리한 패턴
    - 생성형 패턴 `빌프팩추싱`
        - 빌더 Builder: 복잡한 인스턴스를 **조립**하여 만드는 구조, 객체 생성과 구현(표현)을 **분리**한다.
        - 프로토타입 Prototype: 일반적인 **원형**을 만들어 놓고 **복사**한 후 필요한 부분만 수정하여 사용하는 패턴
        - 팩토리메서드 Factory Method: 상위 클래스에서 **객체를 생성하는 인터페이스**를 정의하고 하위 클래스에서 실제 객체 생성, **오버라이딩**
        - 추상 팩토리 Abstract Factory: **서로 관련되거나** 의존적인 객체들의 조합을 만드는 **인터페이스** 제공, **의존성 역전 원칙**
        - 싱글톤 Singleton: **전역 변수를 사용하지 않고** 객체를 하나만 생성하여 **어디서든 참조**할 수 있도록 함
    - 구조 패턴 `ABCDFFP`
        - Adapter 어댑터: **호환되지 않는 인터페이스를 가진 클래스**를 이용할 수 있도록 **중간에서 맞춰줌**
        - Bridge 브릿지: 추상화와 구현을 **분리**하여 각각 독립적으로 **확장**, 구현부에 기능 클래스 **연결**
        - Composite 컴포사이트: 객체 관계를 **트리 구조**로 구성 → **부분-전체 계층**을 표현, **단일 객체와 복합 객체를 동일**하게 취급
        - Decorator 데코레이터: 구현 되어 있는 클래스에 **객체 간의 결합을 통해 동적으로 유연하게 기능 확장**, 상속의 대안으로 사용
        - Facade 퍼사이드: **복잡한 시스템에 단순한 인터페이스** 제공, **결합도를 낮춤**, 통합된 인터페이스
        - Flyweight 플라이트: **클래스의 경량화**의 목적, 여러 개의 가상 인스턴스를 제공하여 **메모리 절감**
        - Proxy 프록시: 실제 객체에 대한 **대리 객체**로 **정보 은닉**의 역할도 수행
    - 행위 패턴 `나머지`
        - Mediator: 객체 수가 많아졌을 때 **중재자**를 두고 **통신 빈도수를 줄임**, 상호 작용의 유연한 변경
        - Interpreter: 분리된 **구문의 해석**을 맡는 클래스를 작성, **여러 형태의 언어 구문 해석**, 문법 캡슐화
        - Iterator: 컬렉션 구현 방법(내부 구조)을 **노출 시키지 않기 위해 반복자를 사용**하여 접근
        - Template Method: **핵심 골격은 유지**하면서(추상클래스) **일부를 서브 클래스로 캡슐화**(하위 클래스에서 구현), 유지보수에 용이
        - Observer: 상태의 변화를 **관찰**하여 의존하는 다른 객체에 **연락이 가고** 내용이 자동 갱신, 일대다 의존 관계
        - State: 객체 **상태를 캡슐화**하여 클래스화, 내부 상태에 따라 행위 내용 변경
        - Visitor:  별도 클레스의 메서드가 **각 클래스를 돌아다니면서** 작업을 수행, 객체의 **구조는 변경하지 않으면서 기능만 따로 추가**하거나 확장할 때 사용
        - Command: 실행될 **기능(요청)을 캡슐화**, 각 **명령**에 따라 서브 클래스가 선택되어 실행, 재사용성 높음
        - Strategy: **알고리즘 군**을 정의하고 같은 알고리즘을 캡슐화 하여 필요할 때 서로 교환, 동적으로 행위를 자유롭게 바꿀 수 있음
        - Memento: 객체의 정보를 **저장**, **Undo 기능**
        - Chain of Responsibility: **한 요청을 2개 이상의 객체**에서 처리
    

### 2. 개발 기술 환경 정의

1. 개발 기술 환경 현행 시스템 분석
    - 운영체제 현행 시스템 분석
        - 운영체제(Operating System): 컴퓨터 시스템이 제공하는 모든 하드웨어, 소프트웨어를 사용 할 수 있도록 해주고, 컴퓨터 사용자와 하드웨어 간의 인터페이스를 담당하는 프로그램
        - 운영체제의 종류 및 특징
            - PC
                - 윈도우(Microsoft): 유지, 관리 비용 장점
                - 유닉스(IBM, HP, SUN): 대용량 처리, 높은 엔터프라이즈급 서버
                - 리눅스(Linus Torvalds): 높은 보안성
            - 모바일
                - 안드로이드(Google): 리눅스 운영체제 위에서 구동, 자바, 코틀린
                - iOS(Apple): 높은 보안성과 고성능 제공
    
    - 네트워크 현행 시스템 분석
        - 네트워크(Network): 컴퓨터 장치들의 노드 간 연결(데이터 링크)을 사용하여 서로에게 데이터를 교환할 수 있도록 하는 기술
        - OSI 7계층 `아파서 티내다, 피ㅠ (APSTNDP)`
            
            
            | 계층 | 설명 | 프로토콜 | 전송 단위 |
            | --- | --- | --- | --- |
            | 응용 계층 (Application Layer) | 사용자와 네트워크 간의 상호 작용 | HTTP, FTP | 데이터 (Data) |
            | 표현 계층 (Presentation Layer) | 데이터의 형식 변환, 암호화/복호화 | JPEG, MPEG | 데이터 (Data) |
            | 세션 계층 (Session Layer) | 연결 접속 및 동기 제어 | SSH, TLS | 데이터 (Data) |
            | 전송 계층 (Transport Layer) |  신뢰성 있는 통신 보장 / 흐름 제어, 오류 제어, 혼잡 제어 등 `흐오혼` | TCP, UD | 세그먼트(Segment) |
            | 네트워크 계층 (Network Layer) | 데이터 전송을 위한 최적화된 경로 제공 | IP, ICMP | 패킷 (Packet) |
            | 데이터 링크 계층 (Data Link Layer) | 인접 시스템 간 데이터 전송 / 전송오류 제어, 동기화, 흐름 제어 등의 전송 기능 / 오류 검출, 재전송 등 기능 | Ethernet(이더넷) | 프레임 (Frame) |
            | 물리 계층 (Physical Layer) | 0과 1 비트 정보를 회선에 보내기 위한 전기적 신호 변환 | RS-232C | 비트 (Bit) |

    - DBMS 현행 시스템 분석
        - DBMS: 데이터베이스라는 데이터의 집합을 만들고, 저장 및 관리할 수 있는 기능들을 제공하는 응용 프로그램
        - 기능: 중복 제어, 접근 통제, 인터페이스 제공, 관계 표현 등
    
    - 미들웨어의  현행 시스템 분석
        - 미들웨어(Middleware): 분산 컴퓨팅 환경에서 응용 프로그램과 프로그램이 운영되는 환경 간에 원만한 통신이 이루어 질 수 있도록 제어해주는 소프트웨어
        - WAS(웹 애플리케이션 서버)

## 3. 요구사항 확인

### 1. 요구사항

1. 요구사항 개념
    - 요구공학(Requirements Engineering): 사용자 요구사항에 대한 도출, 분석, 명세, 확인 및 검증하는 구조화된 활동
    - 분류
        - 기능적 요구사항: 시스템이 제공하는 기능, 서비스에 대한 요구사항 / 특정 입력에 대해 시스템이 어떻게 반응,동작 하는지 / 기능성, 완전성, 일관성
        - 비기능적 요구사항: 기능적 요구사항 외적 요구사항 / 품질이나 제한 조건 / 신뢰성, 사용성, 효율성, 유지보수성, 보안성 등
    - 프로세스 `도분명확`: 도출 → 분석 → 명세 → 확인 및 검증

### 2. 요구사항의 시스템화 타당성 분석

# 2. 화면 설계

## 1. UI 요구사항 확인

### 1. UI 요구사항 확인

- UI(User Interface): 사용자와 시스템 사이에서 의사소통 할 수 있도록 고안된 물리적, 가상의 매개체
- 유형
    - CLI: 정적 텍스트 기반 인터페이스 - 명령어
    - GUI: 그래픽 반응 기반 인터페이스 - 마우스, 키보드
    - NUI: 직관적 사용자 반응 기반 인터페이스 - 터치, 음성
    - OUI: 유기적 상호 작용 기반 인터페이스 - 현실에 존재하는 모든 사물
- UI 설계 원칙 `직유학유`
    - 직관성: 누구나 쉽게 이해, 사용
    - 유효성: 사용자의 목표 달성
    - 학습성: 모두가 쉽게 배우도록
    - 유연성: 사용자의 실수, 오류 방지

### 2. UI 지침

### 3. 스토리보드

### 4. UI 프로토타입 제작 및 검토

## 2. UI 설계

### 1. UI 설계를 위한 UML

- UML(Unified Modeling Langauge): 객체 지향 소프트웨어 개발 과정에서 산출물을 명세화, 시각화, 문서화 할 때 사용되는 모델링 기술과 방법론을 통합해서 만든 표준화된 범용 모델링 언어
- 구성요소 `사관다`
    - 사물(Things): 추상적 개념, 주제를 나타낸다.
    - 관계(Relationships): 사물과 사물을 연결하여 관계를 표현하는 요소
    - 다이어그램(Diagrams): 사물과 관계를 모아 그림으로 표현
- UML 다이어그램
    - 구조적 다이어그램
        - 클래스: 클래스 간 정적인 관계를  표현
        - 객체: 클래스에 속한 객체들(인스턴스)를 특정 시점의 객체와 객체 사이의 관계로 표현
        - 컴포넌트: 시스템을 구성하는 컴포넌트와 그들 사이의 의존 관계를 나타내는 다이어그램
        - 배치: 컴포넌트 사이의 종속성 표현
        - 복합체 구조: 클래스나 컴포넌트가 복합 구조를 갖는 경우 그 내부 구조를 표현하는 다이어그램
        - 패키지: 유스케이스나 클래스 등의 모델 요소들을 그룹화한 패키지들의 관계를 표현한 다이어그램
    - 행위적 다이어그램
        - 유스케이스
        - 시퀀스
        - 커뮤니케이션
        - 상태
        - 활동
        - 타이밍

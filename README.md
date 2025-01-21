# ParkingSite_js

#### 📢 JavaScript, Node.js, MongoDB, Python을 사용하여 사용자 위치 기반 (GPS) 주차장 안내 웹사이트 개발     
🖥️ 개발환경 : JavaScript, Node.js, express, MongoDB, Python3.5, CSS3, Visual Studio Code, 공공데이터API, Naver Maps API      

📜 사용자 위치 기반 주차장 안내 웹사이트    
```
작은 국토 면적에 비해 자동차의 수가 많아 주차 문제가 심각해지고 있다.    
이러한 불편함을 해소하고자 공공데이터를 활용하여 서울시에 있는 주차장 정보를 지도상에 표시하고,    
사용자 위치 기반 또는 장소 검색을 통하여 해당 지역의 주차장을 안내한다.    
주차장 데이터의 요약 정보가 필요한 사용자들을 위한 데이터 분석 및 시각화를 통한 정보를 제공한다.
```

<br>

1. 확장성 있는 네트워크 애플리케이션 개발에 사용되는 Node.js 와 웹 프레임워크인 express로 서버 구축
> Node.js 는 Chrome의 V8엔진을 이용하여 JavaScript로 서버를 구축하고, 서버에서 JavaScript가 작동되도록 해주는 런타임환경이다.     
> Express는 Node.js를 사용하여 쉽게 서버를 구성할 수 있게 만든 클래스와 라이브러리의 집합체인 프레임워크이다.       
> 수많은 개발자들에게 개발 규칙을 강제하여 코드 및 구조의 통일성을 향상할 수 있는 장점이 있고 그 외의 프레임워크로는 Adonis.js, Koa, Sails.js 등이 있다.      
2. Compass 툴을 사용하여 NoSQL 중에서 MongoDB 사용
> 비정형 데이터와 대규모 데이터를 효율적으로 처리하기 위해 더 유연하고 확장 가능한 솔루션인 MongoDB 사용했다.      
> MongoDB는 데이터를 테이블이 아닌 문서 형태로 저장하는 NoSQL(Not Only SQL) 데이터베이스 (Document-Oriented Datebase)이다.      
> 이전의 RDBMS들과는 다른 스키마 유연성과 수평적 확장성을 고려하여 설계된 현대식 데이터베이스이다.
```
📌 MongoDB 특징

1. 스키마 : 어떤 데이터가 어디에 저장되고 어떤 형식과 관계를 정의하는지에 대한 개념 
MongoDB는 데이터베이스 아래에 여러 개의 테이블 대신 컬렉션(Collection)에 JSON(Document) 형태의 데이터를 저장하며,
이를 바이너리 포맷으로 변환한 BSON(Binary JSON)형태로 처리한다.
빠른 데이터 변경과 비정형 데이터 처리, 개발 속도 향상, 다양한 데이터 구조의 통합을 가능하게 하는 유연한 스키마를 확보할 수 있고,
스키마 벨리데이션이라는 기능을 통해 필요한 경우 RDBMS처럼 스키마 제약을 설정할 수도 있다.

2. 복제와 고가용성
RDMS는 외부 어플리케이션에 의존해서 장애 발생 시 스위칭하는데 시간이 걸리고, 정상 작동 여부도 관리자가 확인해야하는 번거로움이 있다.
반면 MongoDB는 Raft 알고리즘을 기반으로 자동 스위칭 기능을 제공해 1초 내외의 지연만 발생하며, 
read/write concern 및 preference 설정을 통해 데이터 일관성과 트래픽 분산도 지원한다.

3. 수평적 확장(샤딩)
MongoDB는 데이터를 여러 서버에 분산 저장하여 수평 확장을 가능하게 한다. 
기존 RDBMS의 파티셔닝 방식과 달리 MongoDB는 샤드 클러스터 구조를 통해 자동으로 데이터를 분산 처리한다. 
이를 통해 대용량 데이터를 효율적으로 처리하며 손쉽게 확장성을 확보할 수 있다.

4. 다양한 인덱싱 기능 지원
MongoDB는 B-Tree 기반의 단일 필드 인덱스를 포함해 복합키, 멀티키, 공간해시, 텍스트 등 다양한 인덱스를 지원하여,
다양한 쿼리에 최적화된 성능을 제공한다.
택시 및 바이크 공유 서비스 등 위치 기반 애플리케이션에서 큰 이점을 제공할 수 있다.
```
3. DB 데이터를 마커 형태로 Naver Maps API를 이용해 지도 위에 표시
> Exploer 11+, Chrome, Safari 5+ 등 PC에서도 모바일에서도 사용 가능 
4. Infowindow로 마커 정보 확인 기능 및 클러스터링 기능 추가
5. GPS로 사용자 현재 위치 자동 설정 기능 추가
6. Kakao 키워드 API를 이용해 질의어 검색 기능 추가로 매칭된 결과 데이터 제공 
7. 공공데이터포털에서 제공하는 서울시 공영주차장 안내 정보 API 활용
8. Python Pandas 데이터 분석 라이브러리를 도입하여 데이터 분석 및 시각화 제공
9. Python Matplotlib의 차트 또는 플롯, 히스토그램 등을 사용하여 전국 데이터 분석과 서울시 구별 주차장 데이터 시각화 제공



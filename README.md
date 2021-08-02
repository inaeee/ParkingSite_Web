# Project_ParkingWebsite
졸업작품으로 출품한 사용자 위치 기반 주차장 웹사이트입니다.

1. 작품 개요   
우리 나라는 작은 국토 면적에 비해 자동차의 수가 매우 많습니다. 
따라서 운전자들은 자신의 주거지나 근무지를 제외한 다른 지역에서 주차할 곳을 찾기가 힘들고 번거롭습니다.
이러한 불편함을 해소하고자 공공데이터를 활용하여 서울시에 있는 주차장의 정보를 제공합니다.

2. 작품 설명   
공공데이터를 활용하여 모은 서울시 주차장들의 위치가 지도 상에 마커로 표시됩니다.
사용자들은 원하는 장소 검색 또는 GPS를 통하여 주차장을 찾고 해당 주차장들의 정보를 얻을 수 있습니다.
주차장 데이터들의 요약 정보가 필요한 사용자들은 분석 데이터들의 시각화를 통해 확인할 수 있습니다.

3. 구현 기능   
    * 확장성 있는 네트워크 애플리케이션 개발에 사용되는 __Node.js__ 와 웹 프레임워크인 __express__ 를 이용하여 서버를 구축하였습니다.
      웹페이지를 구현하기 위해서 객체 기반의 __JavaScript__ 를 사용하였습니다.   
    * __공공데이터포털__ 에서 제공하는 서울시 공영주차장 안내 정보 API를 이용하였습니다.
      해당 데이터는 주차장명, 주소, 주차장 종류, 운영구분, 위도, 경도 등 다양한 정보들이 포함되어 있습니다.
      이러한 정보들 중 프로젝트 구현에 필요한 데이터들만 사용하였습니다.   
    * 유연하게 저장된 데이터들을 조정하고 추가할 수 있도록 __NoSQL__ 중에서 __MongoDB__ 를 사용하였습니다. 속도가 빠른 것이 장점입니다.
      GUI 환경을 통해 MongoDB를 관리하기 위하여 __compass__ 툴을 사용하였습니다.   
    * __Naver Maps API__ 는 JavaScript 형태의 Naver 지도 플랫폼으로써, 웹서비스 또는 애플리케이션에 지도 기능을 구현할 수 있도록 다양한 클래스와 메서드를 제공합니다.
      Exploer 11+, Chrome, Safari 5+ 등 PC에서도 사용이 가능하고 모바일에서도 사용이 가능합니다.
      MongoDB에 입력된 데이터들이 마커 형태로 지도 위에 표시됩니다.   
    * 주황색으로 표시된 마커를 클릭하면 __Infowindow__ 가 보여집니다. 데이터베이스에 넣은 해당 주차장의 정보들을 확인할 수 있습니다.
      사용자는 원하는 지역에 있는 주차장의 위치 뿐만 아니라 기본적인 정보도 함께 얻을 수 있습니다.   
    * 가까운 위치에 주차장이 여러 개가 같이 있다면, __클러스터링__ 을 통하여 하나로 표현되며, 클릭하면 지도가 확대되어 더 자세한 지도로 주차장을 하나씩 확인할 수 있습니다.
      사용자가 현재 있는 위치를 기반으로 주차장의 정보를 알고 싶다면, __현재 위치__ 를 클릭합니다. 그러면 GPS를 통해 사용자가 있는 위치로 지도가 옮겨지며 해당 위치에 빨간색 아이콘이 깜빡입니다.
      이를 토대로 주차장의 정보를 확인할 수 있습니다.   
    * __KAKAO developers__ 에서 __카카오 맵__ 의 기능을 웹과 앱 플랫폼에서 구현할 수 있도록 다양한 메서드와 라이브러리를 통해 제공합니다.
      __키워드로 장소 검색__ 을 통하여 질의어에 매칭된 장소 검색 결과를 제공합니다.   
    * 주차장을 찾고 싶은 장소를 검색하면 해당 장소로 이동하며, 기존 주차장의 마커와 다른 아이콘으로 검색한 장소가 표시됩니다. 이를 토대로 사용자가 원하는 주차장을 찾을 수 있습니다.   
    * __Python__ 을 기반으로 __데이터 분석__ 을 하였습니다.   
      __Pandas__ 는 파이썬에서 사용하는 데이터 분석 라이브러리로, 행과 열로 이루어진 데이터 객체를 만들어 다룰 수 있습니다. 보다 안정적으로 대용량의 데이터들을 처리하는데 매우 편리한 도구입니다.   
      __Matplotlib__ 는 파이썬에서 데이터를 차트나 플롯으로 그려주는 라이브러리 패키지로서 가장 많이 사용되는 데이터 시각화 패키지입니다. 라인플롯, 바차트, 파이차트, 히스토그램 등을 비롯하여 다양한 차트와 플롯 스타일을 지원합니다.
      

## 프로젝트 제목

* 침대 밖은 위험해

## 시연 동영상

[![Watch the video](https://user-images.githubusercontent.com/46912845/148653723-897950c6-861c-4e27-8f1f-7564d091bcd8.jpg)](https://youtu.be/493mAYvdQsk)
* 이미지 클릭시 동영상이 재생 됩니다.


## Pro Makers (김도혁/유수엽/최윤규/권준호/송다영)

* 권준호 : 카메라 모듈 연동 작업 / 마스크 인식 Server API
* 최윤규 : 타이젠 UI 및 소스 머지 작업
* 김도혁 : 온도 센서 연동 및 모듈 구현
* 유수엽 : 온도 센서 하드웨어 분석  
* 송다영 : 기획 및 테스트

## 프로젝트 배경 혹은 목적

  <img src="https://user-images.githubusercontent.com/46912845/148629437-e4f0b754-ce35-453d-b124-c9deccb18b62.jpg" width="70%"></img>    
  <img src="https://user-images.githubusercontent.com/46912845/148629490-a4ebd7ea-0872-496b-a5fa-8dfb277a8cfb.jpg" width="70%"></img>  
  <img src="https://user-images.githubusercontent.com/46912845/148629494-c1907436-c3d5-46f9-a3f6-eef55253b1dd.jpg" width="70%"></img>    
  
  + MLX90614 비접촉 온도센서 연동 성공
  + HC-SR04 (초음파 센서) - 정확한 Timer 10u Sec제어와 Start Time / End Time 방법을 찾지 못하여 다음번에 도전
  + 카메라 연동
    
  <img src="https://user-images.githubusercontent.com/46912845/131221167-89724ca0-befc-4e6a-9ab2-796677422601.png" width="70%"></img>
   + server_restapi는 Upload된 Image의 마스크 유무 판단하여 JOSN형태로 결과 반환


## 파일 리스트


### UI (최윤규)

  + KioskCafeteriaTutorial 예제를 활용한 키오스크 구현
  + https://github.com/Promakers/TopMaker2021/tree/main/KioskCafeteriaTutorial 참조

### server_restapi (권준호)
  + Web API Server
  + Upload된 이미지의 마스크 유무를 판단하여 JSON형태로 결과 반환
  
### Tizen_respapi_test (권준호)
  + 타이젠에서 Res API 이미지 확인 테스트 코드

### MLX90614 비접촉 온도 센서 (김도혁)

  + 아두이노 https://github.com/adafruit/Adafruit-MLX90614-Library 참조하여 타이젠 C# 클래스 제작  

 ## 보드 
 
  * STMP32
  
  <img src="https://user-images.githubusercontent.com/46912845/148635193-c9cab5cb-cbf6-4cb3-8d19-4dd4e7b164d3.jpg" width="50%"></img>  
  
  * STM32용 쉴드 제작 ( 서보 몬터 제어 2개 / 디지털 출력 2개 - 레지저 포인트)
  

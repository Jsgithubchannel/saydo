# 📌 SayDo - AI 기반 음성 Todo 관리 앱
## Say it, Do it!
### AI 음성 인식과 자연어 처리를 활용한 스마트 일정 관리 앱 🚀
-------

### 데모 영상

## 📹 데모 영상
[![Watch the video](https://drive.google.com/file/d/1oWl2Drg9tyym8EBtGoJ4lS3tTDCRxmcd/view?usp=drive_link)

## ✨ 주요 기능

1. AI 음성 인식 및 일정 관리
- 음성 명령을 통해 AI가 사용자의 할 일을 분석
- 일정인지 일반 대화인지 구분하여 처리
- 일정이면 대화 내용에서 날짜/시간을 추출하여 저장

2. 우선순위 및 카테고리 사용자 지정 가능
  
3. UI/UX 디자인 및 사용자 편의성
- 다크 모드 스타일의 Home Screen
- 하단 네비게이션 바와 중앙 마이크 버튼 포함
- 마이크 버튼 클릭 시 반투명한 오버레이와 음성 인식 UI 표시

![Information Architecture drawio](https://github.com/user-attachments/assets/89a62502-2d06-4226-9108-3cc13827e6a5)


## 프로토타입
https://www.figma.com/proto/vz6nCq1vO04dnd6IC6bbE5/SayDo---%EC%9D%8C%EC%84%B1-%EB%B0%8F-%EC%9E%90%EC%97%B0%EC%96%B4-Todo?node-id=0-1&t=dAofrwWDQgKB6saU-1
링크에서 확인 가능합니다.
![스크린샷 2025-03-18 오후 4 50 02](https://github.com/user-attachments/assets/9fb6ebb5-2698-42f1-ac80-79116ac61f47)

## 🛠 추가 구현 예정 기능
1. 구글 캘린더 연동: AI가 자동으로 구글 캘린더에 추가
2. 구글 소셜 로그인

## 회고
#### 1. 학습한 내용 중 가장 유용했던 점  
이번 작업을 통해 **웹과 모바일 환경에서의 소셜 로그인 구현 차이점**을 명확하게 이해할 수 있었다. 
웹에서는 생각보다 간단한(?) API 연동만으로 쉽게 로그인 기능을 추가할 수 있었지만, 
모바일에서는 인증 절차와 플랫폼별 차이(예: iOS와 Android의 차이, OAuth 인증 방식 등)를 더 깊이 고려해야 한다는 점을 배웠다. (모바일보다 웹이 익숙해서 그런 것 같다. )

#### 2. 어려웠던 부분과 해결 방법  
가장 어려웠던 부분은 **모바일에서 소셜 로그인 구현**이었다.  
- 웹에서는 OAuth 인증이 브라우저 기반으로 동작하기 때문에 간단하게 처리할 수 있었지만, 모바일에서는 **OAuth 인증 과정에서 추가적인 설정이 필요**했다.  
- 특히, iOS에서 예상보다 복잡했다.  
- 해결 방법을 찾기 위해 여러 공식 문서를 참고했지만, 설정 과정이 복잡하고 시간이 많이 소요되어 이번에는 도입을 보류했다.  

#### 3. 앞으로 더 학습이 필요한 부분  
- **모바일 소셜 로그인 인증 흐름** (OAuth 2.0, Firebase Authentication 활용)  
- **iOS 및 Android 플랫폼별 차이점** (iOS의 인증 정책, Android의 Activity/Intent 활용 방식)  
- **보안 고려사항** (토큰 저장 방식, Refresh Token 관리, 인증 오류 처리) 

#### 4. 학습한 내용을 실제 프로젝트에 어떻게 적용할 수 있을지  
- 현재 SayDo 프로젝트에는 사용자 인증이 필요하지 않지만, 추후 사용자별 맞춤형 일정 관리 기능을 추가할 경우 소셜 로그인 기능이 필요할 수 있다.  
- OAuth 인증을 보다 쉽게 처리할 수 있는 패키지나 라이브러리를 조사하여 구현 난이도를 줄이는 방법을 고민할 예정이다.  

이번 회고를 통해 모바일 환경에서의 소셜 로그인 구현이 쉽지 않다는 점을 다시 한번 확인했다. 하지만, 차근차근 학습하며 추후 다시 도전할 수 있도록 준비할 계획이다. 🚀

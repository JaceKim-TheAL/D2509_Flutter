# D2509_Flutter
Google에서 개발한 크로스 플랫폼 앱 개발 프레임워크

<img src="./images/flutter.png" width="80%"> 

## INDEX
- [Flutter의 핵심 특징](#-flutter의-핵심-특징)
- [Flutter의 장점 요약](#-flutter의-장점-요약)
- [대표적인 Flutter 앱 사례](#-대표적인-flutter-앱-사례)
- [QNA](#qna)
  - [Q. Flutter가 최초의 크로스 플랫폼 앱 개발 프레임워크인가?](#q-flutter가-최초의-크로스-플랫폼-앱-개발-프레임워크인가)
  - [Q. RN이 성능이 떨어지면 Flutter는 그렇지 않은가?](#q-rn이-성능이-떨어지면-flutter는-그렇지-않은가)

---
Flutter는 Google이 개발한 오픈소스 UI 프레임워크로, 하나의 코드베이스로 iOS, Android, 웹, 데스크톱 앱까지 모두 개발할 수 있는 강력한 도구입니다.

## 🌈 Flutter의 핵심 특징
### 1. 단일 코드베이스, 다중 플랫폼
- 한 번의 코드 작성으로 여러 플랫폼에 앱을 배포할 수 있어요.
- iOS, Android는 물론 웹, Windows, macOS, Linux까지 지원합니다.

### 2. Dart 언어 기반
- Flutter는 Google이 만든 Dart 언어를 사용합니다.
- Dart는 UI 구축에 최적화되어 있고, 정적 타입 언어라서 안정성과 성능이 뛰어나요.

### 3. 위젯 중심 구조
- Flutter의 UI는 모두 위젯으로 구성됩니다.
- StatelessWidget: 상태가 없는 정적인 UI
- StatefulWidget: 사용자 입력 등 상태 변화에 반응하는 UI
- 위젯을 조합해 복잡한 UI도 쉽게 만들 수 있어요.

### 4. 자체 렌더링 엔진
- Flutter는 Skia라는 그래픽 엔진을 사용해 플랫폼 고유 UI에 의존하지 않고 직접 UI를 그립니다.
- 덕분에 일관된 디자인과 고성능을 유지할 수 있어요.

### 5. Hot Reload 기능
- 코드 수정 후 앱을 재시작하지 않고 바로 반영되는 기능으로, 개발 속도를 크게 높여줍니다.

<br/>

[[TOP]](#index)

---
## 🚀 Flutter의 장점 요약
| 장점 | 설명 | 
|-----|------| 
| 빠른 개발     | Hot Reload로 즉시 반영          | 
| 아름다운 UI   | Material & Cupertino 위젯 내장  | 
| 고성능        | 네이티브에 가까운 실행 속도       | 
| 확장성        | 다양한 패키지와 커뮤니티 지원     | 
| 유지보수 효율  | 단일 코드로 여러 플랫폼 관리 가능  | 

<br/>

[[TOP]](#index)

---
## 📱 대표적인 Flutter 앱 사례
- Google Ads
- Alibaba
- eBay
- Reflectly (AI 기반 저널 앱)

Flutter는 특히 스타트업, 크로스 플랫폼 앱, 빠른 MVP 개발에 적합하며, 점점 더 많은 기업들이 채택하고 있다.

<br/>

[[TOP]](#index)

---
## QNA

### Q. Flutter가 최초의 크로스 플랫폼 앱 개발 프레임워크인가?
- 물론 Flutter가 나오기 전에도 한가지 코드베이스로 여러기기에서 작동하는 앱을 만들기 위한 시도는 있었다.
- 그중 처음은 Webview를 활용한 앱(Web APP)이다. 먼저 HTML, CSS, JS로 웹페이지를 만들고 각 플랫폼의 Webview를 활용하는 앱이다. 다만 카메라, 위치, 오디오등의 기기의 네이티브 요소를 활용하는 앱을 만들기 어려웠다.

- 그 다음으로는 2015년 혜성처럼 등장한 React Native(RN)가 있다. 
  - 2015년 이전에도 웹개발에서 쓰이던 React는 RN이 출시할 당시에도 인기있는 프레임워크였고 앱을 제작하고 싶은 많은 웹 개발자들이 RN으로 앱 개발에 입문하게 된다.
  - 다만 RN는 Native, 즉 브라우저가 아닌 네이티브 환경(Android, iOS)에서 돌아긴 했지만 완벽한 네이티브 앱은 아니다. 
  - 따라서 카메라, 오디오등 기기의 HW와 밀접한 관련이 있는 코드를 작성하기 위해서는 bridge를 거쳐야만 했고, 이는 RN으로 개발한 앱의 성능을 떨어뜨리는 원인이 되었다.

### Q. RN이 성능이 떨어지면 Flutter는 그렇지 않은가?
- RN과 다르게 Flutter는 RN의 성능 하락 주범인 bridge가 없고, Dart로 작성한 코드를 AOT 컴파일을 통해 Native단에서 돌아가는 코드로 변환된다. 
- 또한 Skia 라이브러리를 사용해 위젯을 그리기에 대부분의 상황에서 60FPS를 보장한다.

<br/>

[[TOP]](#index)

---
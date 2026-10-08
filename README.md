# 지뢰찾기 안드로이드 앱

게임(1인/2인, 초급·중급·상급, 폭발 연출, 기록 보기)을 안드로이드 앱으로 감싼 프로젝트입니다.
게임 화면은 `app/src/main/assets/index.html` 하나이고, 인터넷 없이도 실행됩니다.
(웹폰트만 인터넷이 없으면 기본 글꼴로 바뀝니다.)

## APK 만드는 방법 1: GitHub에서 자동으로 (설치 프로그램 필요 없음)

1. github.com에서 새 저장소를 만들고, 이 폴더의 모든 파일(`.github` 폴더 포함)을 올립니다.
2. 저장소의 Actions 탭에서 `Build APK`를 선택하고 Run workflow를 누릅니다.
3. 몇 분 뒤 실행 결과 화면 아래 Artifacts에서 `minesweeper-apk`를 내려받아 압축을 풉니다.
4. 안에 있는 `app-debug.apk`를 스마트폰으로 옮겨 설치합니다.
   처음 설치할 때 "출처를 알 수 없는 앱 설치"를 허용해야 합니다.

## APK 만드는 방법 2: 내 컴퓨터에서 Android Studio로

1. Android Studio를 설치하고 이 폴더를 엽니다(Open).
2. 동기화가 끝나면 메뉴 Build > Build Bundle(s) / APK(s) > Build APK(s)를 선택합니다.
3. 알림창의 locate를 눌러 `app-debug.apk`를 찾아 폰에 설치합니다.

## 참고

- 기록은 앱 안에 저장되며 앱 데이터를 지우면 사라집니다.
- 구글 플레이 스토어에 올리려면 별도 서명 키와 개발자 계정이 필요합니다.

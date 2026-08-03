# inLoco 릴리스

로컬 우선 Markdown 메모 앱 inLoco의 정식 배포 저장소입니다.

## 최신 버전 · 4.11.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.11.0/inLoco-Setup-4.11.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.11.0/inLoco-4.11.0-release.apk)

## 릴리스 기록

<!-- INLOCO_RELEASES_START -->
<!-- INLOCO_RELEASE:4.11.0:START -->
### inLoco 4.11.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.11.0/inLoco-Setup-4.11.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.11.0/inLoco-4.11.0-release.apk)

- 최근 vault 점프 리스트로 앱을 시작할 때 로그인 세션 복원이 끝난 뒤 첫 동기화를 실행하도록 수정했습니다.
- 서로 다른 로컬·서버 vault의 동기화 이력이 섞이지 않도록 vault 조합별 데이터베이스로 분리했습니다.
- 세션 복원이 지연되면 만료된 로그인 정보로 동기화를 강행하지 않고 안전하게 건너뛰도록 보강했습니다.
<!-- INLOCO_RELEASE:4.11.0:END -->

<!-- INLOCO_RELEASE:4.10.0:START -->
### inLoco 4.10.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.10.0/inLoco-Setup-4.10.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.10.0/inLoco-4.10.0-release.apk)

- 설정의 테마 색 팔레트에 순백 프리셋을 추가했습니다.
- 순백 프리셋과 라이트 모드를 함께 사용하면 앱 화면과 편집 WebView 배경을 정확한 #FFFFFF로 표시합니다.
- 흰색 테마 스와치를 선택해도 선택 표시가 잘 보이도록 검은색 체크 아이콘을 사용합니다.
<!-- INLOCO_RELEASE:4.10.0:END -->

<!-- INLOCO_RELEASE:4.9.0:START -->
### inLoco 4.9.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.9.0/inLoco-Setup-4.9.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.9.0/inLoco-4.9.0-release.apk)

- 너비 문법이 없는 기존 표는 페이지 본문 너비를 채우는 기본 렌더링을 유지하고, widths 문법을 사용한 표만 열 너비 조절 UI를 표시합니다.
- 너비 조절형 표가 페이지보다 좁을 때 가운데에 배치되며 마지막 열의 오른쪽 경계도 드래그할 수 있습니다.
- 읽기·스플릿 렌더에서 변경한 표 너비와 정렬을 Ctrl+Z로 되돌리고 Ctrl+Shift+Z 또는 Ctrl+Y로 다시 적용할 수 있습니다.
<!-- INLOCO_RELEASE:4.9.0:END -->

<!-- INLOCO_RELEASE:4.8.0:START -->
### inLoco 4.8.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.8.0/inLoco-Setup-4.8.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.8.0/inLoco-4.8.0-release.apk)

- Android에서 현재 화면 해상도가 지원하는 가장 높은 주사율을 앱 창의 선호 주사율로 요청합니다.
- 모바일 목록과 편집 화면의 다시 그리기 영역을 분리해 스크롤·커서 이동 시 불필요한 전체 repaint를 줄였습니다.
- Android profile 빌드에서 읽기·편집·스플릿별 프레임 p95와 120Hz 기준 초과율을 기록하는 성능 계측을 추가했습니다.
<!-- INLOCO_RELEASE:4.8.0:END -->

<!-- INLOCO_RELEASE:4.7.0:START -->
### inLoco 4.7.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.7.0/inLoco-Setup-4.7.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.7.0/inLoco-4.7.0-release.apk)

- `## 제목 {toggle}`과 `- 항목 {toggle}` 문법으로 하위 내용을 접고 펼칠 수 있으며 상태는 원문과 분리해 문서별로 유지합니다.
- 렌더된 표의 헤더 메뉴에서 열 기준 오름차순·내림차순 정렬을 실행하면 본문 행만 안정 정렬해 Markdown 원문에 반영합니다.
- 표 열 경계를 드래그해 너비를 바꿀 수 있고 결과는 기존 `:::wide widths=…` 문법에 저장됩니다.
<!-- INLOCO_RELEASE:4.7.0:END -->

<!-- INLOCO_RELEASE:4.6.0:START -->
### inLoco 4.6.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.6.0/inLoco-Setup-4.6.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.6.0/inLoco-4.6.0-release.apk)

- 일반 저장 시 vault 내부에 `.sync-temp` 폴더를 만들지 않고 같은 폴더의 일회성 임시파일로 안전하게 저장합니다.
- 로컬 전용 vault의 삭제본은 vault 밖 앱 휴지통에 보관해 `.sync-trash`를 만들지 않으며 앱에서 그대로 복원할 수 있습니다.
<!-- INLOCO_RELEASE:4.6.0:END -->

<!-- INLOCO_RELEASE:4.5.0:START -->
### inLoco 4.5.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.5.0/inLoco-Setup-4.5.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.5.0/inLoco-4.5.0-release.apk)

- `:::wide`와 `:::` 사이의 표 또는 블록 수식을 읽기·스플릿 pane 전체 너비로 렌더합니다.
- 읽기·스플릿 화면의 본문 여백에서도 휠 스크롤이 작동하고 세로 스크롤바를 pane 최우측에 표시합니다.
- 스플릿에서 편집기와 렌더 어느 쪽에 커서를 두고 Ctrl+휠을 사용해도 양쪽 배율을 함께 변경합니다.
<!-- INLOCO_RELEASE:4.5.0:END -->

<!-- INLOCO_RELEASE:4.4.0:START -->
### inLoco 4.4.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.4.0/inLoco-Setup-4.4.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.4.0/inLoco-4.4.0-release.apk)

- 점프 리스트로 서버용 vault를 열어도 정규화된 vault 식별자로 기존 서버 연결을 복원하고 시작 동기화를 실행합니다.
- Windows에서 동기화 중 창 닫기 또는 Alt+F4를 누르면 완료를 기다리거나 강제 종료할지 확인합니다.
<!-- INLOCO_RELEASE:4.4.0:END -->

<!-- INLOCO_RELEASE:4.3.0:START -->
### inLoco 4.3.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.3.0/inLoco-Setup-4.3.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.3.0/inLoco-4.3.0-release.apk)

- 표준 `- [ ]` 한글 체크리스트를 일반 불릿보다 먼저 판정해 항상 체크박스로 렌더합니다.
- 스플릿 뷰에서 읽기 모드로 전환해도 오른쪽 렌더 페이지의 스크롤 위치를 유지합니다.
- `**강조**한글`은 본문 글꼴을 그대로 사용하고 굵기만 자연스러운 bold로 표시합니다.
<!-- INLOCO_RELEASE:4.3.0:END -->

<!-- INLOCO_RELEASE:4.2.0:START -->
### inLoco 4.2.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.2.0/inLoco-Setup-4.2.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.2.0/inLoco-4.2.0-release.apk)

- `**강조**한글`처럼 한글과 붙은 강조가 더 선명한 굵기로 표시됩니다.
- 불릿·숫자·중첩·CRLF 체크리스트가 체크박스로 렌더되고 클릭으로 정확히 토글됩니다.
- 숫자 목록 중간 항목을 추가하거나 삭제하면 아래 번호가 자동으로 다시 정렬됩니다.
- PDF 인용구 안의 문단·목록·체크박스·표·수식·코드가 구조를 유지해 출력됩니다.
- 탭이 많아지면 너비를 줄인 뒤 가로 스크롤로 전환되며, drag & drop으로 탭 순서를 바꿀 수 있습니다.
<!-- INLOCO_RELEASE:4.2.0:END -->

<!-- INLOCO_RELEASE:4.1.0:START -->
### inLoco 4.1.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.1.0/inLoco-Setup-4.1.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.1.0/inLoco-4.1.0-release.apk)

- 각 탭이 편집 중인 본문·커서·보기 모드와 읽기·편집·스플릿 스크롤 위치를 독립적으로 유지합니다.
- 탭을 옮기거나 다른 메모를 열 때 미저장 경고 없이 작업 상태를 보존하고, 탭 닫기·vault 전환·앱 종료 시에만 저장 여부를 확인합니다.
<!-- INLOCO_RELEASE:4.1.0:END -->

<!-- INLOCO_RELEASE:4.0.0:START -->
### inLoco 4.0.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.0.0/inLoco-Setup-4.0.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.0.0/inLoco-4.0.0-release.apk)

- 인라인 코드를 주황 계열 색상으로 구분해 본문과 더 쉽게 구별할 수 있습니다.
- 테마 색상 변경이 Windows WebView 편집기의 커서·선택·거터·스크롤바에 즉시 반영됩니다.
- 설정에서 운영체제 기본 맞춤법 검사를 켜거나 끌 수 있습니다.
- 빌드·GitHub Release 업로드·버전별 패치노트가 누적되는 릴리즈 README 갱신을 한 명령으로 수행하는 자동화를 추가했습니다.
<!-- INLOCO_RELEASE:4.0.0:END -->
<!-- INLOCO_RELEASES_END -->

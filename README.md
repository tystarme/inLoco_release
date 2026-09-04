# inLoco 릴리스

로컬 우선 Markdown 메모 앱 inLoco의 정식 배포 저장소입니다.

## 최신 버전 · 4.21.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.21.0/inLoco-Setup-4.21.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.21.0/inLoco-4.21.0-release.apk)

## 릴리스 기록

<!-- INLOCO_RELEASES_START -->
<!-- INLOCO_RELEASE:4.21.0:START -->
### inLoco 4.21.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.21.0/inLoco-Setup-4.21.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.21.0/inLoco-4.21.0-release.apk)

- **PDF 수식이 한 줄 안에서 위아래로 제멋대로 뜨던 문제**를 고쳤습니다. 문장 속 수식을 본문보다 제 깊이의 두 배만큼 띄워 놓고 있었고, 그 양이 수식마다 달라 들쭉날쭉했습니다. 이제 본문 글자와 같은 줄에 정확히 앉습니다.
- **분수가 한 줄을 통째로 차지하던 문제**를 고쳤습니다. 분수 하나가 본문 폭 전체를 먹어 문장이 끊기고 수식 사이가 벌어졌습니다.
- `\bar`·`\overline`의 **윗줄을 글자에 제대로 붙였습니다.** 글꼴의 실제 치수를 재서 글자 잉크 바로 위에 긋습니다(예전에는 글자 상자 꼭대기에 그려 한참 떠 있었습니다).
- 제곱근 기호와 늘어나는 괄호 `( ) [ ] { }`를 **직접 그립니다.** 글리프를 억지로 키우던 방식이라 수식 위아래에 빈 공간이 생기고 획 굵기가 덮개선과 어긋났습니다.
- **수식 문법을 더 알아봅니다.** `\hat` `\vec` `\tilde` `\dot` 같은 악센트, `\mathbf` `\mathbb` `\boldsymbol` 같은 서체 명령, `\displaystyle` 류 스위치, `\textbf` `\mbox`를 지원합니다. 조판에 실패한 수식만 이미지로 물러나므로, 한 문서 안에서 어떤 수식은 글자·어떤 수식은 이미지로 갈리는 일이 줄었습니다.
- `10^{-4}`의 앞선 `-`를 이항 연산자가 아닌 **부호**로 봅니다. 연산자 좌우 여백도 TeX 기준에 맞춰 좁혔습니다(`1 - p`가 두 배로 벌어져 있었습니다).
<!-- INLOCO_RELEASE:4.21.0:END -->

<!-- INLOCO_RELEASE:4.20.2:START -->
### inLoco 4.20.2

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.20.2/inLoco-Setup-4.20.2.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.20.2/inLoco-4.20.2-release.apk)

- **문장 속 수식이 조판되지 않던 문제를 고쳤습니다.** 문단·목록·제목이 수식 설정을 못 받아 문장 안의 `$…$`만 옛 근사 표기로 떨어졌습니다. 이제 블록 수식과 똑같이 조판됩니다.
- `aligned` 여러 줄 수식에 **있지도 않은 중괄호 `{`가 그려지던 문제**를 고쳤습니다. 중괄호는 `cases`에만 붙습니다.
- `\bar`·`\overline`·제곱근의 **윗줄이 글자에서 너무 멀리 떠 있던 것**을 글자에 붙였습니다.
- 인터넷이 없어 글꼴을 받지 못해도 수식을 조판합니다(내장 글꼴로 물러납니다). 예전에는 이 경우 수식이 통째로 근사 표기로 나갔습니다.
<!-- INLOCO_RELEASE:4.20.2:END -->

<!-- INLOCO_RELEASE:4.18.2:START -->
### inLoco 4.18.2

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.18.2/inLoco-Setup-4.18.2.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.18.2/inLoco-4.18.2-release.apk)

- 4.18.1과 **기능은 같습니다.** 같은 `4.18.1` 버전으로 내용이 다른 설치 파일이 두 번 만들어져, 어느 것을 설치했는지 구분할 수 없는 문제가 있었습니다. 구분을 위해 번호만 올린 판입니다.
- `4.18.1`을 설치하셨다면 이 판으로 다시 설치해 주세요.
<!-- INLOCO_RELEASE:4.18.2:END -->

<!-- INLOCO_RELEASE:4.18.1:START -->
### inLoco 4.18.1

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.18.1/inLoco-Setup-4.18.1.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.18.1/inLoco-4.18.1-release.apk)

- **Ctrl+Z로 되돌릴 수 있는 횟수가 줄어들던 문제를 고쳤습니다.** 렌더에서 시작한 편집(체크박스·토글·표)과 편집기 입력이 각각 다른 실행취소 기록에 쌓여, 한쪽을 되돌리면 다른 쪽 기록이 통째로 사라졌습니다. 이제 편집기가 있으면 편집기 기록 하나만 씁니다.
- **접기 경계에 등급이 생겼습니다.** `## ---`처럼 적으면 그 등급 **이하**의 접기만 끊습니다. `## ---`은 `##` 접기만 끊고 바깥 `#` 접기는 그대로 통과합니다. 등급이 셀수록 선이 두껍게 그려집니다.
- 등급이 없던 `---` 두 줄 형태는 없앴습니다(안쪽 구역용 경계가 바깥 접기까지 잘랐습니다). 이제 접기 경계는 `# ---` 계열 한 가지입니다.
<!-- INLOCO_RELEASE:4.18.1:END -->

<!-- INLOCO_RELEASE:4.18.0:START -->
### inLoco 4.18.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.18.0/inLoco-Setup-4.18.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.18.0/inLoco-4.18.0-release.apk)

- **접기 경계**가 생겼습니다. `---`를 두 줄 연속으로 적으면 제목 접기가 거기서 멈춥니다. `# 제목` 하나가 문서 끝까지 삼키는 걸 막을 수 있습니다.
- 접기 경계는 화면·PDF 모두 일반 구분선보다 **굵은 선**으로 그려 한눈에 구분됩니다.
<!-- INLOCO_RELEASE:4.18.0:END -->

<!-- INLOCO_RELEASE:4.17.1:START -->
### inLoco 4.17.1

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.17.1/inLoco-Setup-4.17.1.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.17.1/inLoco-4.17.1-release.apk)

- **체크박스가 사라지던 문제를 고쳤습니다.** 목록 항목 사이에 빈 줄이 하나라도 있으면 그 목록 전체의 체크박스가 그냥 불릿으로 보였습니다.
- **엉뚱한 체크박스가 체크되던 문제를 고쳤습니다.** 중첩된 항목은 렌더러가 자식부터 만들기 때문에 화면 순서와 어긋났고, 접어 둔 토글이 가린 체크박스도 순번을 밀고 있었습니다.
- 체크박스와 토글은 이제 **자동 저장하지 않습니다.** 읽으면서 접었다 폈다 할 때마다 저장·업로드가 돌아 화면이 끊겼습니다. 저장은 Ctrl+S(저장 버튼)에서만 합니다.
<!-- INLOCO_RELEASE:4.17.1:END -->

<!-- INLOCO_RELEASE:4.17.0:START -->
### inLoco 4.17.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.17.0/inLoco-Setup-4.17.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.17.0/inLoco-4.17.0-release.apk)

- **체크박스를 눌러도 파일이 바뀌지 않던 문제를 고쳤습니다.** 편집기 본문과 어긋나 옛 내용이 덮어쓰던 것이 원인이었습니다. 체크 한 번을 Ctrl+Z로 되돌릴 수도 있습니다.
- 토글 문법이 줄 **맨 앞**으로 왔습니다: `## {toggle} 제목`, `- {toggle} 항목`. 접기 버튼도 줄 앞(목록에서는 bullet 옆)에 그려집니다.
- `{toggle:close}` / `{toggle:open}`으로 처음 상태를 정할 수 있고, **버튼을 누르면 원문이 그대로 바뀝니다.** 접어 둔 상태가 파일에 남아 재시작·동기화·다른 기기에서도 유지됩니다.
- 예전 문서의 줄 끝 `{toggle}` 표기도 그대로 동작합니다. 원문을 임의로 옮기지 않습니다.
- PDF에 `{toggle}` 글자가 본문으로 인쇄되던 문제를 고쳤습니다. 접어 둔 내용도 종이에는 모두 펼쳐서 나옵니다.
<!-- INLOCO_RELEASE:4.17.0:END -->

<!-- INLOCO_RELEASE:4.16.0:START -->
### inLoco 4.16.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.16.0/inLoco-Setup-4.16.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.16.0/inLoco-4.16.0-release.apk)

- 노트·폴더를 우클릭해 **탐색기에서 열기**를 고르면 Windows 탐색기가 그 파일을 선택한 채 열립니다. 공백·한글이 든 경로도 정확히 찾아갑니다.
- 시작 화면 설정에 **"닫기 전 열어둔 탭 모두"** 가 생겼습니다. 앱을 다시 켜면 탭 순서와 활성 탭이 그대로 돌아옵니다(그 사이 지워진 노트는 건너뜁니다).
- **Ctrl+Shift+T** 로 방금 닫은 탭을 닫기 전 위치에 되살립니다. 연달아 누르면 계속 거슬러 올라갑니다.
- 노트 이름 변경·폴더 이동·삭제가 저장된 탭 목록에도 바로 반영돼, 다시 켰을 때 없는 경로를 열려고 하지 않습니다.
<!-- INLOCO_RELEASE:4.16.0:END -->

<!-- INLOCO_RELEASE:4.15.1:START -->
### inLoco 4.15.1

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.15.1/inLoco-Setup-4.15.1.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.15.1/inLoco-4.15.1-release.apk)

- 표/수식 바로 윗줄에 속성을 적어 폭을 조절합니다. `widths=1fr,2fr`은 열 너비, `wide`는 그 블록만 전체 폭, `wide widths=2fr,1fr`처럼 한 줄에 같이 쓸 수 있습니다. 단위는 px(화면 고정폭)·mm(PDF에서 실제 크기)·fr(남는 폭을 비율대로), 생략하면 픽셀입니다.
- 비율(fr) 표는 화면과 PDF 모두 폭을 정확히 채우고, 열 경계를 드래그하면 옆 열에서 폭을 가져와 표 전체 크기가 변하지 않습니다. 드래그 결과는 같은 단위로 원문에 저장됩니다.
- PDF 내보내기가 표 열 너비를 반영합니다. 고정폭 합이 페이지를 넘으면 비율을 유지한 채 줄여 열이 잘리지 않습니다.
- PDF에 `:::wide widths=...`와 `:::` 문법이 본문 글자로 인쇄되던 문제를 고쳤습니다.
- 단위 없이 저장된 기존 표(`widths=180,240`)는 그대로 동작하며, 드래그로 저장해도 단위를 임의로 붙이지 않습니다.
<!-- INLOCO_RELEASE:4.15.1:END -->

<!-- INLOCO_RELEASE:4.14.5:START -->
### inLoco 4.14.5

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.14.5/inLoco-Setup-4.14.5.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.14.5/inLoco-4.14.5-release.apk)

- Windows Ctrl+F 검색창을 네이티브 입력으로 교체해 한글 조합과 커서가 뒤집히던 문제를 해결했습니다. 찾아 바꾸기의 '바꿀 내용' 칸도 같은 방식으로 동작합니다.
- 읽기·편집 본문의 기본 글자 크기를 이전 110% 크기로 재기준화했습니다. 배율 표시 100%가 그만큼 크게 보이며, 사용자가 지정한 배율은 그 위에 그대로 적용됩니다.
- 편집 모드 검색이 CRLF 줄바꿈 문서에서 엉뚱한 위치를 잡거나 일부 매치만 강조하던 문제를 고쳤습니다. 파일의 줄바꿈 표기는 저장할 때 그대로 보존합니다.
- Ctrl+F에서 Enter를 계속 눌러도 두 번째 매치에서 멈추던 문제와, 검색을 닫아도 편집기에 강조가 남아 있던 문제를 고쳤습니다.
- 스플릿 모드에서 편집기와 렌더 화면 **양쪽 모두** 검색어를 강조하고, 각 화면이 자기 스크롤로 현재 매치를 보여 줍니다.
- 표 셀에도 본문과 같은 글꼴을 적용하고, 코드는 JetBrains Mono 전용 글꼴로 표시해 코드와 본문을 한눈에 구분할 수 있게 했습니다.
- 인라인 코드(`코드`)와 코드 블록 안의 검색어도 강조합니다. 코드 표기는 그대로 두고 매치 부분의 배경만 칠하며, 검색을 닫으면 강조도 함께 사라집니다.
- 검색창 타이핑이 큰 노트에서 끊기던 문제를 개선하고, 검색창에서 Ctrl+A(전체 선택)로 입력한 검색어를 한 번에 지우거나 복사할 수 있게 했습니다.
<!-- INLOCO_RELEASE:4.14.5:END -->

<!-- INLOCO_RELEASE:4.14.0:START -->
### inLoco 4.14.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.14.0/inLoco-Setup-4.14.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.14.0/inLoco-4.14.0-release.apk)

- 편집 도구 모음의 중복 도움말 버튼을 제거하고 최상단 도움말 버튼으로 접근 경로를 일원화했습니다.
- 읽기·스플릿 화면 본문에 Pretendard를 적용하고 행간을 5% 넓혀 한글과 영문 가독성을 개선했습니다.
- 순백 테마의 모든 Material 역할색을 무채색으로 구성해 배경과 UI에 남아 있던 청색 기운을 제거했습니다.
- Windows 창 제목에 현재 vault명 또는 단일 파일명을 표시해 Alt+Tab과 작업 표시줄 미리보기에서 창을 구분할 수 있게 했습니다.
<!-- INLOCO_RELEASE:4.14.0:END -->

<!-- INLOCO_RELEASE:4.13.0:START -->
### inLoco 4.13.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.13.0/inLoco-Setup-4.13.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.13.0/inLoco-4.13.0-release.apk)

- Ctrl+F에서 t_mech, `본문`, C++, x[y]처럼 기호가 포함된 검색어도 읽기 화면에 정확히 하이라이트되도록 수정했습니다.
- Ctrl+F 검색창의 위젯과 포커스를 안정적으로 유지하고 검색 갱신을 지연·통합해 Windows 한글 조합 중 커서와 자모가 뒤집히는 문제를 개선했습니다.
- 검색어를 모두 지우거나 검색창을 닫았을 때 편집 화면에 이전 하이라이트가 남지 않도록 수정했습니다.
<!-- INLOCO_RELEASE:4.13.0:END -->

<!-- INLOCO_RELEASE:4.12.0:START -->
### inLoco 4.12.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.12.0/inLoco-Setup-4.12.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.12.0/inLoco-4.12.0-release.apk)

- 분량이 큰 문서에서 입력 이벤트 전달과 줄 번호 전체 레이아웃 계산을 지연·통합해 타이핑 지연을 줄였습니다.
- 탭마다 편집기와 실행 취소 기록을 독립적으로 유지해 탭 전환 후에도 Ctrl+Z와 Undo 버튼으로 수정사항을 되돌릴 수 있습니다.
- Undo·Redo 버튼이 Windows WebView의 실제 활성 편집기를 제어하도록 수정했습니다.
<!-- INLOCO_RELEASE:4.12.0:END -->

<!-- INLOCO_RELEASE:4.11.0:START -->
### inLoco 4.11.0

- [Windows Setup](https://github.com/tystarme/inLoco_release/releases/download/v4.11.0/inLoco-Setup-4.11.0.exe)
- [Android APK](https://github.com/tystarme/inLoco_release/releases/download/v4.11.0/inLoco-4.11.0-release.apk)

- 최근 vault 점프 리스트로 앱을 시작할 때 로그인 세션 복원이 끝난 뒤 첫 동기화를 실행하도록 수정했습니다.
- 서로 다른 로컬·서버 vault의 동기화 이력이 섞이지 않도록 vault 조합별 데이터베이스로 분리했습니다.
- 세션 복원이 지연되면 만료된 로그인 정보로 동기화를 강행하지 않고 안전하게 건너뛰도록 보강했습니다.
- 동기화 DB를 사용자 AppData 앱 지원 폴더 아래에 저장해 실행 위치와 관계없이 안전하게 열도록 수정했습니다.
- DB 상위 폴더를 먼저 생성해 점프 리스트 실행 시 발생하던 SQLite code 14 오류를 방지했습니다.
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

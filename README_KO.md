# Pushup Video Pipeline — OAuth 소개 사이트

Google OAuth 동의 화면에 사용할 **공개 정적 사이트**입니다. 영상 자동 업로드 프로그램의 코드 및 설정과는 무관합니다.

## 포함된 파일

- `index.html`: 앱 홈페이지
- `privacy.html`: 개인정보처리방침
- `terms.html`: 이용약관
- `styles.css`: 공통 스타일
- `.nojekyll`: GitHub Pages 정적 게시 설정

## 게시하기: GitHub Pages (별도 공개 저장소)

1. GitHub에 로그인하고 **새 공개 저장소**를 만듭니다. GitHub 사용자명이 `MYNAME`이라면 저장소 이름은 정확히 `MYNAME.github.io`로 지정하는 방식을 권장합니다. 이미 해당 이름의 저장소가 있다면 해당 사이트의 관리 상황에 맞게 별도의 저장소 또는 커스텀 도메인을 사용하세요.
2. **여기에 포함된 웹사이트 파일만** 저장소 최상위에 업로드합니다. 본인의 `personal-video-pipeline` 소스나 토큰, `.pipeline`/`.youtube` 등의 운영 데이터는 절대 업로드하지 마세요.
3. 저장소 **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main, /(root) → Save**를 선택합니다.
4. 사이트 공개 확인: `https://MYNAME.github.io/` 및 `https://MYNAME.github.io/privacy.html` 과 `https://MYNAME.github.io/terms.html`.
5. Google Cloud **Google Auth Platform → 브랜딩**에 세 URL을 입력합니다. **승인된 도메인**에는 Google 화면이 허용하는 실제 호스트명을 사용합니다.
6. 필요한 경우 **Google Search Console**에서 사이트 소유권을 확인합니다. URL 접두어 속성의 HTML 확인 파일을 이 공개 사이트의 루트에 업로드하는 방식을 사용할 수 있습니다. OAuth 검증에서는 도메인 전체 소유권 확인이 요구될 수 있으므로 Search Console 완료만으로 OAuth 승인까지 보장되지는 않습니다.
7. **대상 → 앱 게시**를 진행하고 검증 안내가 있으면 Google 안내에 따릅니다. 프로덕션 전환 뒤에도 기존 만료된 OAuth 토큰은 앱의 공식 재인증 절차로 갱신해야 할 수 있습니다.

## 공개 전에 꼭 확인

- 공개 연락처는 `sahora.bin@gmail.com`으로 기재했습니다. 사용자 제공 Google Cloud 화면에서 확인된 주소이며 **사이트를 공개하면 누구나 볼 수 있습니다**. 원치 않으면 3개 HTML 파일의 이 주소를 원하는 공개 업무용 이메일로 변경하세요.
- 개인정보처리방침에 기재한 데이터의 실제 저장 위치, 삭제 방식, 인증 정보 처리 방법이 현재 코드와 일치하는지 검토하세요. 이 페이지는 기술·정책 검토를 위한 초안이며 자동으로 Google 인증 심사를 통과시킨다는 보장은 없습니다.
- `MYNAME`은 예시입니다. Google Cloud에 예시 URL을 복사하지 말고 **실제 배포된 https 주소**를 입력하세요.
- 메인 프로그램은 전혀 수정하지 않아도 됩니다. 이 사이트는 독립된 공개 저장소에서 운영하세요.

# 설원 스키 대여소

1. ZIP을 풀고 파일들을 GitHub 저장소의 main 브랜치 최상위에 올립니다. index.html, gear.png, snow.jpg, .nojekyll이 같은 위치에 있어야 합니다.
2. 저장소 Settings → Pages에서 Deploy from a branch → main → / (root)를 선택하고 저장합니다.
3. Pages에 표시되는 HTTPS 주소를 열어 회원 로그인과 대여를 확인합니다.

Firebase 콘솔의 ski-device 프로젝트에서 Authentication의 이메일/비밀번호 로그인 방법과 기본 Firestore 데이터베이스를 활성화합니다. Firestore 규칙 탭에서 동봉된 firestore.rules를 검토하고 게시합니다. 이미 동일한 규칙을 게시했다면 이 단계는 건너뛸 수 있습니다. 콘솔 자동 배포는 포함되어 있지 않습니다.

API 키에 웹사이트 제한을 적용했다면 Google Cloud 콘솔의 해당 키 설정에 게시 사이트의 HTTPS 출처(예 https://사용자명.github.io/*)를 추가합니다. 이 앱은 REST 방식으로 이메일/비밀번호 인증을 사용합니다. 회원 로그인과 기록 저장에는 인터넷 연결이 필요하며 오프라인 데모는 브라우저에 기록을 저장합니다. GitHub Pages 주소의 브라우저 저장소는 로컬 파일 주소와 별개입니다.

게시 방법 https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
Firebase 키 설정 https://firebase.google.com/docs/projects/api-keys

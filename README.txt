Crown Envoy 사이트 (정적 사이트: 서버 프로그램이 필요 없어요)
================================================================

모든 파일이 폴더 없이 한 곳에 있어요. 이 파일들을 그대로 GitHub 저장소에 올리면 돼요.

  index.html                 첫 화면 (바로 플레이 / 다운로드 / 버전 목록 / 패치노트 / 도움말)
  versions.json              버전 목록 (새 버전을 낼 때 여기에 한 줄 추가)
  patchnotes.json            패치노트 (새 패치마다 맨 위에 항목 추가)
  CrownEnvoy-v0.1.html       v0.1 게임 파일
  CrownEnvoy-latest.html     최신 버전의 복사본 ("바로 플레이"가 이 파일을 열어요)
  map.jpg, battle-*.jpg      사이트 배경·소개 이미지

[ 올리는 방법: GitHub Pages ]
  1. 저장소 화면에서 Add file > Upload files
  2. 이 폴더의 파일을 모두 골라 끌어다 놓기 (폴더가 아니라 파일들이에요)
  3. Commit changes
  4. Settings > Pages > Deploy from a branch > main / (root) > Save
  5. 주소:  https://내아이디.github.io/저장소이름/

[ 새 버전을 낼 때 ]
  1. 새 게임 파일을 CrownEnvoy-v0.2.html 처럼 올리기
  2. 같은 내용을 CrownEnvoy-latest.html 로도 덮어쓰기
  3. versions.json 맨 위에 새 항목을 추가하고, 이전 최신 항목의 "latest"를 false로, latest 값과 latestFile 을 바꾸기
  4. patchnotes.json 맨 위에 패치노트 추가
  (index.html 안의 FALLBACK 복사본은 파일로 직접 열 때만 쓰이니, 서버에 올릴 땐 json만 고치면 돼요)

[ 알아 둘 점 ]
  - 친구들이 모두 "바로 플레이" 링크로 들어오면 항상 같은 버전이라 서로 맞지 않는 문제가 없어요.
  - 진행 상황(저장된 게임 등)은 접속한 사이트 주소마다 따로 저장돼요.

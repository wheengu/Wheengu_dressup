# 흰구 꾸미기 — GitHub Pages 배포용

이 폴더는 URL로 바로 접속 가능한 정적 웹사이트 배포용 패키지입니다.  
`index.html`이 폴더 최상단에 있으므로, 이 폴더 안의 파일들을 GitHub 저장소의 루트에 올리면 됩니다.

## 포함된 파일 구조

```text
index.html
assets/
main.png
wheen_gu_base_transparent.png
.nojekyll
README.md
```

## GitHub Pages 배포 순서

1. GitHub에서 새 Repository를 만듭니다.
   - 추천 이름: `wheen_gu-dressup`
   - 공개 사이트로 운영하려면 `Public` 권장
2. 이 폴더 안의 파일 전체를 Repository 최상단에 업로드합니다.
   - ZIP 파일 자체를 올리는 것이 아니라, 압축을 푼 뒤 `index.html`, `assets/` 등을 올립니다.
3. Repository의 `Settings`로 이동합니다.
4. `Pages` 메뉴에서 배포 소스를 설정합니다.
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
5. 저장 후 잠시 기다리면 접속 URL이 생성됩니다.

예상 URL 형식:

```text
https://깃허브아이디.github.io/wheen_gu-dressup/
```

## 업데이트 방법

나중에 프로그램을 수정하면, 이 폴더의 파일을 새 버전으로 교체한 뒤 GitHub에 다시 업로드하면 됩니다.  
GitHub Pages는 변경 사항이 반영되기까지 보통 잠깐 시간이 걸릴 수 있습니다.

## 주의사항

- `index.html`은 반드시 저장소의 최상단에 있어야 합니다.
- `assets/` 폴더를 누락하면 배경, 의상, BGM, 효과음이 깨질 수 있습니다.
- `.nojekyll` 파일은 GitHub Pages에서 정적 파일을 그대로 배포하기 위한 안전장치입니다.

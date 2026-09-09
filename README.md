# 안원잘부 콘텐츠 케이스스터디

「안녕하세요원이입니다잘부탁드립니다」 유튜브 채널의 롱폼 29편 전수 케이스스터디.
정적 페이지 하나(`index.html`)와 썸네일 폴더(`thumbnails/`)로만 구성되어 있어
빌드 과정 없이 그대로 호스팅할 수 있습니다.

## GitHub Pages로 공개하는 방법

1. 새 레포지토리를 만들고 이 폴더의 내용을 그대로 올립니다.
   ```
   git init
   git add .
   git commit -m "안원잘부 콘텐츠 케이스스터디"
   git branch -M main
   git remote add origin <레포 주소>
   git push -u origin main
   ```
2. 레포 **Settings → Pages** 로 이동
3. **Source** 를 `Deploy from a branch`, **Branch** 를 `main` / `/ (root)` 로 설정하고 저장
4. 1~2분 뒤 `https://<계정>.github.io/<레포명>/` 로 접속됩니다

> 조직 계정의 Private 레포에서 Pages를 쓰려면 GitHub Enterprise 플랜이 필요합니다.
> Public 레포로 올릴 경우 채널 분석 내용이 외부에 공개되니, 공유 범위를 먼저 확인하세요.
> `index.html` 에는 `noindex` 메타태그를 넣어 검색엔진 수집은 막아두었습니다.

## 구성

```
index.html            리포트 본문 (CSS 인라인, 외부 의존성은 Google Fonts 뿐)
thumbnails/           썸네일 29장 (편번호_videoId.jpg)
안원잘부_콘텐츠_케이스스터디.md   같은 내용의 마크다운 버전
```

## 데이터 기준

- 수집 기준일 2026-09-09 (조회수는 이 시점 값)
- 범위: Shorts 제외 롱폼 29편 전량 (2026-02-05 ~ 2026-09-04)
- 한계와 조사 방법은 리포트 하단에 명시

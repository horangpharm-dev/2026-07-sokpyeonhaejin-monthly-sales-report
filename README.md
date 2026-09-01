# 속편해진내과의원 월간 매출 리포트 (2026년 7월호) — 기간 만료 자동 삭제

이한재 본부장님 제공용. 워터마크(이름·연락처·날짜) 적용.

- `index.html` — 리포트 본문(단독 실행 HTML). 열람 URL은 저장소 Pages 루트.
- `EXPIRES` — 열람 마지막 날(KST). 다음 날 00:00 KST에 `expire` 워크플로가 `index.html`을 안내 페이지(`expired.html`)로 교체한다. 본문에도 같은 날짜의 클라이언트 만료 가드가 있다.
- **즉시 파기**: Actions → expire → Run workflow → force=`true`. 또는 저장소 삭제.
- **기간 연장**: `EXPIRES` 값 수정 후 push. (본문 바닥글의 「열람 기한」 문구와 가드는 `DATA.expires` 재빌드가 필요하다.)
- 공개 저장소인 이유: 무료 플랜의 GitHub Pages는 공개 저장소에서만 동작한다.

# hykim.me — 배포 방법 (GitHub Pages)

1. github.com 로그인 → 오른쪽 위 **+** → **New repository** → Repository name: `hykim-site`, **Public** 선택 → **Create repository**
2. 저장소 화면에서 **Add file → Upload files** → `index.html`(과 `photo.jpg`, `cv.pdf`가 있으면 함께)을 끌어다 놓고 **Commit changes**
3. Settings → Pages → Source: "Deploy from a branch", Branch: `main` / `(root)` → Save
4. Settings → Pages → Custom domain 에 `www.hykim.me` 입력 → Save (`CNAME` 파일 자동 생성)
5. 도메인 등록업체 DNS 설정에서
   - `www`  CNAME  →  `hykim-site.github.io`
   - `@`    A      →  185.199.108.153 / 185.199.109.153 / 185.199.110.153 / 185.199.111.153
   기존 Google Sites 용 레코드는 삭제
6. 반영(최대 24시간) 후 Settings → Pages 에서 "Enforce HTTPS" 체크

## 내용 수정
- 논문 추가: `index.html`의 `<ol class="pubs">` 안에 `<li>` 블록 하나 복사해서 수정
- 워킹페이퍼: `<ul class="wp">` 안의 `<details>` 블록 복사
- 강의: `<ul class="courses">`
- 마지막 업데이트 날짜: 파일 맨 아래 `<footer>`

# 2026 교보생명 내 손으로 뽑는 10대뉴스 — 랜딩페이지

인트라넷 공지의 QR로 접속해 후보 17개를 살펴보는 모바일 페이지입니다. 투표는 이지모아에서 합니다.

## 파일 구성

- `index.html` — 페이지 전체 (후보 데이터는 파일 안의 `CANDIDATES` 목록)
- `assets/thumbs/` — 콘텐츠 카드 썸네일 (`itemNN-N`)
- `assets/penguin.png` — 펭귄 마스코트
- `assets/fonts/` — Paperlogy(오프닝 제목), Pretendard(본문)
- `assets/vendor/three/` — 3D 제목용 three.js 0.160.0

빌드 과정이 없는 정적 사이트입니다. Vercel에서 Framework Preset은 `Other`, Build Command와 Output Directory는 비워 두면 됩니다.

## 수정하는 법

- 후보 제목·설명·링크: `index.html`의 `CANDIDATES` 목록을 고칩니다. 순서가 곧 화면 순서입니다.
- 경품 이미지: `index.html`에서 `prize-ph`를 찾아 주석에 적힌 대로 `<img>` 한 줄로 바꾸고 이미지를 `assets/`에 넣습니다.
- 고친 뒤 GitHub에 올리면 Vercel이 자동으로 다시 배포합니다. 주소(QR)는 바뀌지 않습니다.

## 확인용 주소

- 날짜별 D-N 배지 확인: 주소 끝에 `?today=2026-11-25`
- 인트로 다시 보기 버튼 표시: 주소 끝에 `?review`

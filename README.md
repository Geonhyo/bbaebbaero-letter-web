# 빼빼로 편지

서버 없이 돌아가는 정적 사이트예요. 메시지는 링크 주소(# 뒤)에 담겨요.

## 파일
- `index.html` — 사이트 전체
- `og-image.png` — 카톡/인스타 링크 미리보기 이미지 (1200×630)
- `logo.png`, `icon-512.png` — 로고, 앱 아이콘
- `apple-touch-icon.png`, `favicon.png` — 아이콘

## 배포 (Vercel, 약 5분)
1. 도메인(bbaebbaero.nookin.dev)은 이미 index.html에 들어가 있어요
2. https://vercel.com 가입 → Add New → Project → 이 폴더를 드래그해서 업로드
   (또는 터미널에서 `npx vercel --prod`)
3. 도메인 연결: Vercel 프로젝트 → Settings → Domains 에 bbaebbaero.nookin.dev 입력 → 안내대로 nookin.dev DNS에 CNAME(bbaebbaero → cname.vercel-dns.com) 추가

## 미리보기가 안 바뀔 때
카카오톡은 미리보기를 캐시해요. 이미지 수정 후엔
https://developers.kakao.com/tool/debugger/sharing 에서 URL 넣고 "캐시 초기화".

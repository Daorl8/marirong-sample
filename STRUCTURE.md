# STRUCTURE — 마리롱 (Mari Rong)

포항 동해 수제 디저트 실고객 시안. 단일 HTML 브로슈어 원페이지.

```
/ (배포 루트, CF [assets] directory="./")
├─ index.html          단일 파일 (인라인 CSS/JS, 모바일 우선)
├─ mr-char.webp        마리롱 캐릭터(흰 고양이) — 헤더·히어로·소개·푸터 활용
├─ favicon.png         캐릭터 기반 파비콘 (180px)
├─ og-marirong.jpg     OG 썸네일 1200×630 (휘낭시에, jpg=카톡 호환)
├─ mr-financier.webp   휘낭시에 (메뉴)
├─ mr-macaron.webp     딸기 마카롱 (메뉴)
├─ mr-creamcookie.webp 크림치즈 쿠키 (메뉴)
├─ mr-cookie.webp      초코 아몬드 쿠키 (메뉴)
├─ mr-saltbread.webp   소금빵 (메뉴)
├─ mr-eggtart.webp     에그타르트 (메뉴)
├─ mr-oreo.webp        오레오 디저트 (메뉴)
├─ mr-fruitcup.webp    과일 컵 (메뉴)
├─ wrangler.toml · .assetsignore · CHANGELOG.md · STRUCTURE.md
└─ img/                원본 40장 (배포 제외). ⚠️mr-logo.webp(워드마크 로고) 미사용 orphan → .assetsignore 제외
```

## 섹션 앵커
`#top` 히어로(캐릭터) · `#about` 소개 · `#menu` 메뉴(사진 8종 + 전체 라인업) · `#visit` 영업시간+오시는길 · 푸터

## 디자인 (연보라 + 화이트 큐트)
- **팔레트**: 페이지 `--lav-bg #F5F0FC` · 섹션 `--lav-soft #EADFF8` · 메인 `--lav #CBB4EC`(로고 실측) · **버튼/강조 `--lav-deep #7655BC`(AA 흰글씨 5.5)** · 텍스트 `--lav-text #6B4BA3` · 잉크 플럼 `#3F3556` · 화이트 · 볼핑크 `--pink #F6C3D0` · 핑크버튼/휴무 `--pink-deep #B8476B`(AA 5.06).
- **폰트(시안=CDN)**: 헤딩·브랜드 **Jua**(둥글고 두꺼운 큐트 — Rix다람쥐 유사 요청) + 본문 Pretendard. ⚠️납품 시 서브셋 self-host. Pretendard CDN 무버전.
- **캐릭터 적극 활용**: 헤더 원형 아바타·히어로 큰 마스코트(bob 애니)·소개 옆·푸터. 둥근 카드(24px)·연보라 블롭·소프트 그림자.
- a11y: reveal + 2.4s 타임아웃 + noscript, :focus-visible, reduced-motion 폴백, rAF 스무스 앵커.

## 네이버 실데이터 (반영 완료)
- 주소: 경북 포항시 남구 동해면 일월로 73-1 1층(동해초 정문 앞, 옛주소 도구리 641-10).
- 영업: 화·수·목·금·토 13:00–20:00 / **일·월 정기휴무**. 전화 0507-1371-4761(안심번호; 소개엔 010-3810-4761도 있음).
- **네이버 place ID 1025763123** → 지도 버튼 = 정식 엔트리 링크. **인스타 @mari_rong_** → 예약·인스타 버튼.
- 메뉴(소개 기준): 휘낭시에 6종·쿠키 4종·마카롱 다양·플레인 스콘·꼬끄 후레이크·에그타르트·소금빵.

## ⚠️ 확인/보류
- 가격 미제공 → 무표기 + "인스타 예약" 안내. 아침오픈=인스타 공지 안내.
- og:image·JSON-LD image = 상대경로(jpg). og:url·canonical·절대경로 = 도메인 확정 후 3줄.
- 폰트 CDN(시안) → 납품 시 self-host. 헤드리스 렌더 미실행(브라우저 다운로드 제한).

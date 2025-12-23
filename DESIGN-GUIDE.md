# 🎨 Personal Branding Design Guide

> **분위기**: 모던 & 따뜻한  
> **메인 컬러**: 베이지 & 웜 브라운  
> **용도**: 퍼스널브랜딩 개인 소개앱

---

## 📦 컬러 팔레트

### 메인 컬러
| 이름 | 색상 | HEX | 용도 |
|------|------|-----|------|
| Primary | 🟤 | `#8B7355` | 메인 강조, 버튼 |
| Primary Light | 🟤 | `#A08B70` | 호버 상태 |
| Primary Dark | 🟤 | `#6B5744` | 눌림 상태 |

### 포인트 컬러
| 이름 | 색상 | HEX | 용도 |
|------|------|-----|------|
| Secondary | 🟡 | `#C4A77D` | 골드 포인트 |
| Accent | 🟠 | `#D4A574` | CTA 버튼, 링크 |

### 배경 컬러
| 이름 | 색상 | HEX | 용도 |
|------|------|-----|------|
| Background | ⬜ | `#FAF7F2` | 메인 배경 |
| Card | ⬜ | `#FFFFFF` | 카드 배경 |
| Section | 🟫 | `#F5F0E8` | 섹션 구분 |
| Dark | ⬛ | `#2C2825` | 푸터, 다크 섹션 |

### 텍스트 컬러
| 이름 | 색상 | HEX | 용도 |
|------|------|-----|------|
| Primary | ⬛ | `#2C2825` | 제목 |
| Secondary | 🔘 | `#5C5552` | 본문 |
| Muted | 🔘 | `#9C9590` | 부가 정보 |

---

## ✏️ 폰트

### 한글 (Pretendard)
```css
font-family: 'Pretendard', -apple-system, BlinkMacSystemFont, sans-serif;
```
- **제목**: Semibold (600) ~ Bold (700)
- **본문**: Regular (400) ~ Medium (500)

### 영문 포인트 (Playfair Display)
```css
font-family: 'Playfair Display', Georgia, serif;
```
- 이탤릭으로 세련된 느낌 연출
- 짧은 영문 슬로건에 사용

### 폰트 크기
| 용도 | 크기 | CSS 변수 |
|------|------|----------|
| 히어로 타이틀 | 56px | `--text-5xl` |
| 섹션 타이틀 | 40px | `--text-4xl` |
| 카드 타이틀 | 24px | `--text-2xl` |
| 본문 | 16px | `--text-base` |
| 작은 텍스트 | 14px | `--text-sm` |

---

## 🔘 버튼 스타일

### Primary 버튼 (메인 CTA)
```html
<button class="btn btn-primary">연락하기</button>
```
- 배경: 웜 브라운 (`#8B7355`)
- 텍스트: 크림 화이트
- 호버: 살짝 위로 올라가는 효과 + 그림자

### Secondary 버튼 (보조)
```html
<button class="btn btn-secondary">더 보기</button>
```
- 테두리만 있는 버튼
- 호버 시 배경 채워짐

### 버튼 크기
```html
<button class="btn btn-primary btn-sm">작은 버튼</button>
<button class="btn btn-primary btn-lg">큰 버튼</button>
```

---

## 🃏 카드 스타일

### 기본 카드
```html
<div class="card">
  <h3>카드 제목</h3>
  <p>카드 내용</p>
</div>
```
- 흰 배경
- 부드러운 그림자
- 호버 시 살짝 올라가는 효과

### 테두리 카드
```html
<div class="card card-bordered">
  내용
</div>
```

---

## 📐 레이아웃

### 컨테이너
```html
<div class="container">
  <!-- 최대 1024px, 가운데 정렬 -->
</div>
```

### 섹션
```html
<section class="section">
  <!-- 기본 섹션 -->
</section>

<section class="section section-alt">
  <!-- 배경색 있는 섹션 (베이지) -->
</section>
```

---

## ✨ 애니메이션 & 인터랙션

### 호버 효과
- 버튼: `translateY(-2px)` + 그림자 강화
- 카드: `translateY(-4px)` + 그림자 강화
- 링크: 밑줄 애니메이션

### 트랜지션 속도
| 속도 | 용도 | CSS 변수 |
|------|------|----------|
| 150ms | 빠른 피드백 (링크 색상) | `--transition-fast` |
| 250ms | 기본 (버튼, 카드) | `--transition-base` |
| 400ms | 느린 (페이지 전환) | `--transition-slow` |

---

## 📱 반응형 디자인

### 브레이크포인트
- **모바일**: 768px 이하
- **태블릿**: 769px ~ 1024px
- **데스크톱**: 1025px 이상

### 모바일 조정사항
- 제목 크기 축소
- 그리드 → 단일 컬럼
- 여백 축소

---

## 🎯 프롬프트 예시 (앱 만들 때 사용)

```
퍼스널 브랜딩 랜딩페이지 만들어줘.

design-system.css 파일을 사용해서 스타일링해줘.

페이지 구성:
1. 히어로 섹션: 이름 + 한줄 소개 + 프로필 사진
2. About 섹션: 자기소개 (배경색 있는 섹션)
3. Skills 섹션: 보유 스킬 카드 3개
4. Contact 섹션: 연락처 + CTA 버튼

폰트는 Pretendard 사용하고,
영문 슬로건은 Playfair Display 이탤릭으로 해줘.
```

---

## 🔗 폰트 CDN 링크

```html
<!-- Pretendard -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.9/dist/web/static/pretendard.min.css" />

<!-- Playfair Display (영문 포인트) -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital@1&display=swap" rel="stylesheet">
```

---

**이 디자인 가이드와 `design-system.css`를 함께 사용하세요!** 🚀

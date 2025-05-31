# 🇰🇷 티스토리 & 커스텀 HTML용 다국어 번역 위젯

> Tailwind 기반 Google Translate 연동 UI – 포트폴리오/블로그 최적화

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)

* 한국어 블로그를 누구나 쉽게 읽을 수 있도록, **마치 처음부터 영문 블로그였던 것처럼!**

* **링크 끝부분에 옵션 추가**로 `영어블로그 포트폴리오`로 만들기 (전체 페이지 자동 번역)

* **국기 버튼 UI + 번역 설정 유지 기능 제공**

---

## 📦 설치 방법 (티스토리 예시)

> `<script>` 삽입이 가능한 모든 HTML 플랫폼에서 사용 가능

1. 관리자 → 플러그인 → `[HTML 배너 출력]` 추가
2. 사이드 바로 배치
3. `widget.html` 코드 복붙
4. 필요 시 색상/아이콘/텍스트 커스터마이징

---

## ✨ 주요 기능 요약

* 🏳️ 국기 기반 언어 전환 버튼 제공 (활성 상태 표시 포함)
* 💾 `LocalStorage` 기반 언어 설정 저장 및 유지
* 🌐 `?lang=xx` 파라미터 대응
* 🔁 SPA 호환 – pushState / replaceState 동작 감지
* 🎨 `TailwindCSS` + `CSS 변수` 기반 UI 커스터마이징
* 📦 국기 아이콘 CDN: [flagcdn.com](https://flagcdn.com)

---

## 🌍 이 위젯이 제공하는 경험

* 사용자는 **링크 클릭만으로 자동 번역된 블로그**에 진입할 수 있습니다
* 언어 설정은 LocalStorage에 저장되어, **이후 페이지 이동·새로고침에도 유지**됩니다
* 언어 버튼을 따로 누르지 않아도, **처음부터 끝까지 외국어 블로그처럼** 탐색이 가능합니다
* 사이트 내에서도 언어 패널을 통해 추가적인 조작이 가능합니다.

> 📌 예시: <br/>
> 👉 `https://myblog.tistory.com/?lang=en` <br/>

→ 영어 자동 설정 <br/> → 전반에 걸쳐 유지 <br/> → 영문 포트폴리오 경험 제공 <br/>

---

## 💻 호환 가능한 블로그 플랫폼

> ⚠️ Velog, Brunch, Notion 등 **HTML/JS 삽입이 불가능한 플랫폼에서는 사용 불가**합니다.

* 티스토리 (HTML 배너 플러그인 사용)
* GitHub Pages, Jekyll, Hugo 등 정적 블로그
* WordPress (Self-hosted)
* 기타 HTML 삽입이 가능한 CMS/블로그 환경

---

## 💡 이 위젯만의 장점?

| 기능/특성                | `element.js` 기본 위젯 | `GTranslate` 위젯           | 본 위젯 (Custom Widget) |
| -------------------- | ------------------ | ------------------------- | -------------------- |
| `?lang=xx` 링크 진입 지원  | ❌ 지원 안 함           | ✅ 지원                      | ✅ 지원                 |
| 페이지 이동/새로고침 시 언어 유지  | ❌ 불안정              | ✅ 유지됨                     | ✅ LocalStorage로 유지   |
| 현재 언어 상태 표시          | ❌ 없음               | ❌ 제한적                     | ✅ 버튼 UI로 명확히 표시      |
| UI 커스터마이징            | ❌ 제한적              | ❌ 어려움                     | ✅ Tailwind로 자유롭게 가능  |
| SPA 대응 (pushState 등) | ❌ 미지원              | ❌ 미지원                     | ✅ 대응 가능              |
| 국기 기반 버튼 UI          | ❌ 드롭다운 UI          | ✅ (iframe 기반, 커스터마이징 어려움) | ✅ 자유롭게 구성 가능         |
| 번역 품질 및 신뢰성          | ✅ Google 엔진        | ✅ Google 엔진               | ✅ Google 엔진 (간접 호출)  |

> 본 위젯은 Google Translate의 `element.js` 스크립트를 기반으로 작동하며,
> 공식 문서가 없지만 **간단하게 적용 가능하고 로딩이 빠른** 점이 장점입니다.

> 향후에는 GTranslate 기반 구조로의 확장도 고려 중입니다.

---

## 🚧 알려진 한계

* 네트워크 상태에 따라 초기 번역 적용 시 약간의 지연이 발생할 수 있습니다
* `element.js`는 문서화되지 않은 레거시 스크립트로, 향후 변경될 가능성이 있습니다
* SPA 번역 환경에서 일부 엣지 케이스가 발생할 수 있습니다
    
     – GitHub Issues 또는 PR을 통해 논의해주세요

---

## 🙌 기여 및 PR 환영

* 새로운 언어 버튼 추가
* 접근성 개선
* 타 블로그/플랫폼 대응
* 예쁜 디자인이나 실제 사용 예시 공유

PR과 아이디어 제안은 언제든지 환영합니다 ❤️

---

## 📁 구성 파일

* `index.html` – 실제 삽입 가능한 위젯 코드
* `docs/README.ko.md` – 한국어 문서
* `docs/README.en.md` – 영어 문서

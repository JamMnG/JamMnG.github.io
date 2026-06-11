# 🚀 이재민 | Backend Developer Portfolio

> "안정적인 인프라를 빌드하고, 데이터의 흐름을 최적화하는 백엔드 개발자입니다."

안녕하세요! 백엔드 개발자 이재민의 인터랙티브 포트폴리오 웹사이트입니다.
단순히 서버 로직을 작성하는 것을 넘어, 프론트엔드와 백엔드를 아우르는 높은 이해도를 바탕으로 병목 현상을 해결하고 트래픽을 효율적으로 통제하는 데이터 아키텍처를 고민합니다.

이 포트폴리오 웹사이트는 백엔드 개발자로서의 성과를 보여줌과 동시에, 클라이언트 렌더링 및 UI 상호작용(Interactive)에 대한 이해도를 증명하기 위해 직접 3D 테마로 기획 및 구현되었습니다.

🌐 **포트폴리오 링크:** [본인의 GitHub Pages URL 입력]
📧 **Email:** hally209@naver.com
🎓 **Education:** 신라대학교 컴퓨터공학과 (졸업 예정)

---

## ✨ Portfolio UI/UX Highlights
이 웹사이트 자체도 하나의 프론트엔드 프로젝트로서 구현되었습니다. Vanta.js와 Vanilla JS를 활용하여 역동적인 3D 인터랙션을 제공합니다.

- **3D Topology Background:** `Vanta.js`와 `p5.js`를 활용하여 마우스의 움직임에 반응하는 3D 등고선(Topology) 지형 애니메이션을 구현했습니다.
- **Interactive Car Cursor:** Bruno Simon의 포트폴리오에서 영감을 받아, 마우스 위치에 따라 회전 각도(atan2)와 위치가 계산되어 부드럽게 쫓아오는 장난감 자동차 커스텀 커서를 적용했습니다.
- **3D Tilt Effect & Glassmorphism:** CSS `perspective`와 JS `getBoundingClientRect`를 결합하여 마우스 오버 시 카드가 3D로 기울어지는 물리적 타격감을 주고, 반투명한 유리 질감(backdrop-filter)을 적용했습니다.

---

## 🛠 Tech Stack

### Backend
- Java, Spring Boot
- Python, FastAPI

### Database & Infra
- MySQL, Redis
- AWS, Docker

### Frontend & AI
- JavaScript, Flutter
- OpenAI API, YOLOv8

---

## 💻 Key Projects

### 1. 📚 소셜 독서 노트 (Social Reading)
> 사용자의 읽기 취향을 분석하고 기록을 공유하는 데이터 기반 소셜 플랫폼
- **기간:** 2026.02 ~ 진행 중
- **Tech:** FastAPI, MySQL, Redis, Tailwind CSS
- **Key Achievements:**
  - **API 캐싱 최적화:** 외부 도서 검색 API의 속도 저하를 방지하기 위해 Redis 인메모리 캐싱 도입. **캐시 적중률 72%**, **평균 응답 속도 128ms** 달성.
  - **무중단 자동 저장:** `INSERT ON DUPLICATE KEY UPDATE` (Upsert) 기반으로 DB I/O 부하를 방어하며 실시간 데이터 영속성 보장.
  - **논블로킹(Non-blocking) 아키텍처:** FastAPI의 `BackgroundTasks`를 활용해 무거운 추천 알고리즘 갱신 작업을 백그라운드로 위임하여 서버 지연 방어.

### 2. 🧠 마음온도 (Mental Care AI)
> 비동기 처리 최적화가 적용된 AI 기반 감정 분석 멘탈케어 서비스
- **기간:** 2025.09 ~ 2025.12
- **Tech:** Python, FastAPI, OpenAI API, MySQL
- **Key Achievements:**
  - **비동기 처리로 병목 현상 해결:** 외부 OpenAI API 호출 시 발생하는 대기 시간(I/O Bound) 동안 스레드 블로킹을 막기 위해 `async/await`를 적용, **응답 대기시간 2.5초 단축**.
  - **관심사의 분리(SoC):** 컨트롤러 내 복잡한 AI 호출 로직과 DB 쿼리를 모듈로 분리하여 유지보수성 향상.
  - **Pydantic 데이터 검증:** 클라이언트로부터 들어오는 데이터 타입과 유효성을 자동으로 검증.

### 3. 🛍️ 딩동 (우리 동네 안전 중고거래)
> 접근성 강화 및 데이터 영속성 기술이 적용된 하이퍼로컬 플랫폼
- **기간:** 2025.03 ~ 2025.06
- **Tech:** Flutter, Firebase, Vanilla JS
- **Key Achievements:**
  - **접근성(A11y) 테마 제어:** CSS Custom Properties를 활용해 디지털 소외계층을 위한 큰 글씨 모드를 단일 클래스 토글만으로 구현.
  - **데이터 영속성 확보:** `LocalStorage`를 활용해 브라우저 새로고침 시에도 사용자 테마 설정이 유지되도록 UX 연속성 설계.
  - **프론트엔드 최적화:** 이미지 캐싱 최적화를 통해 **앱 메모리 점유율 40% 감소**.

---

## 🏃‍♂️ How to Run

1. Repository 클론
```bash
git clone [https://github.com/jamming/your-repo-name.git](https://github.com/jamming/your-repo-name.git)

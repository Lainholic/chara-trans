# 🎭 AI Character Card Translator & Editor (CharaTrans)
> **[RisuAI & SillyTavern Universal] AI 캐릭터 카드 다국어 번역 및 메타데이터 에디터**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Platform: Web](https://img.shields.io/badge/Platform-Web%20(Client--side)-brightgreen.svg)]()
[![OpenRouter](https://img.shields.io/badge/OpenRouter-Compatible-38bdf8.svg)]()

100% 브라우저 로컬에서 구동되는 무설치 웹 기반 캐릭터 카드 번역 에디터입니다.  
RisuAI, SillyTavern, Chub.ai의 V2/V3 PNG 카드 메타데이터(`chara`, `ccv3`)를 손상 없이 파싱하고, OpenRouter 및 OpenAI 호환 모델을 통해 검열 없이 전 세계 모든 언어로 자연스럽게 번역하여 다시 정상 PNG 카드로 구워냅니다.

---

## ✨ 핵심 기능 (Key Features)

- 🌐 **글로벌 다국어 양방향 번역 (Multi-Language)**:
  - 🇰🇷 한국어, 🇺🇸 English (해외 수출용 역번역), 🇯🇵 日本語 (라노벨 서브컬처 문체), 🇨🇳 简体中文, 🇹🇼 繁體中文, 🇪🇸 Español, 🇫🇷 Français, 🇩🇪 Deutsch 지원
- 🔄 **실시간 최신 모델 자동 동기화 (Dynamic Model Fetching)**:
  - OpenRouter 및 OpenAI 호환 엔드포인트의 `/models` API를 실시간 조회하여 400개 이상의 최신 모델을 클릭 한 번으로 불러옵니다.
  - 내일 새 모델이 나와도 코드 수정 없이 바로 사용 가능!
- ⚡ **검열 0% (Zero Censorship)**:
  - DeepSeek V3/R1, Llama 3.3, Claude 등 검열 없는 모델을 활용하여 수위 높은 성인향(NSFW), 피폐물, 다크 판타지 카드도 튕김 없이 100% 번역.
- 🎯 **특수 태그 100% 보존**:
  - `{{char}}`, `{{user}}`, `<START>`, 따옴표(`"..."`), 지문 별표(`*...*`) 등 캐릭터 봇 필수 마크업 태그 손상 방지.
- 🖼️ **PNG 바이너리 청크 재주입 (Lossless Injection)**:
  - Base64 디코딩/인코딩 및 CRC32 체크섬 계산을 통해 원본 이미지 화질 손상 없이 새로운 번역 메타데이터를 완벽하게 재삽입.
- 🛡️ **100% 클라이언트 사이드 (Privacy-First)**:
  - 별도의 백엔드 서버가 존재하지 않으며, API 키와 대화 데이터는 사용자의 브라우저에서 지정된 엔드포인트로만 직접 전송됩니다.

---

## 🚀 사용 방법 (Quick Start)

### 1. 실행
- 웹 브라우저에서 `index.html`을 더블클릭하거나, 배포된 웹사이트 주소로 접속합니다.

### 2. API 설정
1. **엔드포인트** 입력 (기본값: OpenRouter `https://openrouter.ai/api/v1`)
2. **API Key** 입력
3. `[🔄 모델 동기화]` 버튼을 눌러 원하는 모델(예: `deepseek/deepseek-chat`) 선택 후 `[💾 설정 저장]` 클릭

### 3. 번역 및 저장
1. 번역하고 싶은 **PNG 캐릭터 카드**를 화면에 드래그 앤 드롭합니다.
2. 상단에서 **목표 언어**(한국어, 영어, 일본어 등)를 선택합니다.
3. `[🔄 전체 번역 시작]`을 누르면 첫인사, 대체 그리팅, 캐릭터 설명, 대화 예시, 성격, 시나리오가 순차적으로 번역됩니다.
4. 번역 결과를 확인 및 수정한 후 `[💾 PNG 카드 저장]`을 누르면 번역된 새로운 카드가 다운로드됩니다!

---

## 💻 호환성 (Compatibility)

- **RisuAI** (V2 / V3 완벽 호환)
- **SillyTavern** (TavernCard Spec 완벽 호환)
- **Chub.ai** / **JanitorAI** / **Agnaistic**

---

## 📄 라이선스 (License)

This project is licensed under the [MIT License](LICENSE).
Anyone can freely use, modify, and distribute this software.

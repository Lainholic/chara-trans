# 🎭 AI Character Card Translator & Editor (CharaTrans)
> **[English | [한국어](#-한국어-안내)]**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Platform: Web](https://img.shields.io/badge/Platform-Web%20(100%25%20Client--side)-brightgreen.svg)]()
[![OpenRouter](https://img.shields.io/badge/OpenRouter-Compatible-38bdf8.svg)]()
[![Spec: V2/V3](https://img.shields.io/badge/TavernCard-V2%2FV3%20Compatible-orange.svg)]()

A lightweight, 100% client-side web application to translate, edit, and localize AI Character Cards (PNG/JSON) for **RisuAI**, **SillyTavern**, and **Chub.ai** with **Zero Censorship** and **Lossless PNG Metadata Re-injection**.

---

## 🌟 Key Features

- 🌐 **Global Multi-Language Translation**:
  - Translate to & from **English**, **Korean (한국어)**, **Japanese (日本語)**, **Simplified/Traditional Chinese (中文)**, **Spanish**, **French**, and **German**.
  - Great for localizing foreign cards, or translating your own Korean/Japanese cards into English for uploading to Chub.ai!
- 🔄 **Real-Time Dynamic Model Syncing**:
  - Connects to OpenRouter or any OpenAI-compatible `/models` API to fetch 400+ live models on the fly. No outdated hardcoded lists—always up to date.
- ⚡ **Zero Censorship (Uncensored Translations)**:
  - Supports **DeepSeek V3/R1**, **Llama 3.3 70B**, **Claude**, and local Ollama models. Seamlessly translates mature (NSFW), dark fantasy, and gritty roleplay cards without refusal filters.
- 🎯 **Strict System Markup & Tag Preservation**:
  - Intelligently preserves `{{char}}`, `{{user}}`, `<START>`, quotes (`"..."`), and action asterisks (`*...*`).
- 🖼️ **Lossless PNG Chunk Parsing & Re-injection**:
  - Directly reads and writes binary `tEXt` chunks (`chara` and `ccv3`) with CRC32 checksum calculation. The original avatar image is preserved at 100% quality.
- 🛡️ **100% Privacy & Client-Side Only**:
  - No backend server. Your API key and card data never leave your browser except to call your designated AI endpoint.

---

## 🚀 Quick Start Guide

### 1. Open the App
- Simply open `index.html` in any modern web browser or visit the deployed web page.

### 2. Configure API Endpoint
1. **Endpoint**: Enter your base URL (Default: `https://openrouter.ai/api/v1`).
2. **API Key**: Enter your OpenRouter or OpenAI-compatible key.
3. Click **`[🔄 Sync Models]`** to fetch the live model list, and pick your preferred model (e.g., `deepseek/deepseek-chat`).
4. Click **`[💾 Save Config]`**.

### 3. Translate & Download
1. **Drag & Drop** any character card (`.png`) or `.json` file into the dropzone.
2. Select your **Target Language** from the toolbar.
3. Click **`[🔄 Translate All]`** to translate greetings, alternate greetings, description, message examples, personality, and scenario.
4. Edit the translations if desired, then click **`[💾 Save PNG Card]`** to download the ready-to-use localized card!

---

## 💻 Compatibility

- **RisuAI** (Fully compatible with V2 / V3 specs)
- **SillyTavern** (TavernCard Spec V2/V3)
- **Chub.ai** / **JanitorAI** / **Agnaistic**

---

<br>

# 🇰🇷 한국어 안내

> **[RisuAI & 실리태번 공용] AI 캐릭터 카드 다국어 번역 및 메타데이터 에디터**

100% 브라우저 로컬에서 구동되는 무설치 웹 기반 캐릭터 카드 번역 에디터입니다.  
RisuAI, SillyTavern, Chub.ai의 V2/V3 PNG 카드 메타데이터(`chara`, `ccv3`)를 손상 없이 파싱하고, OpenRouter 및 OpenAI 호환 모델(DeepSeek 등)을 통해 검열 없이 전 세계 모든 언어로 자연스럽게 번역하여 다시 정상 PNG 카드로 구워냅니다.

### ✨ 한국어 주요 특징
1. **글로벌 다국어 지원**: 영어 카드를 한국어로 번역하거나, 내가 만든 한글 카드를 영어/일본어로 번역하여 해외 사이트에 수출 가능.
2. **실시간 최신 모델 자동 동기화**: 오픈라우터의 최신 모델 목록을 실시간으로 긁어와 드롭다운에 채워주므로 코드 수정 불필요.
3. **검열 0%**: 수위 높은 성인향(NSFW), 피폐물, 다크 판타지 카드도 튕김 없이 100% 번역.
4. **특수 태그 보존**: `{{char}}`, `{{user}}`, `<START>` 등의 마크업 태그 완벽 보존.
5. **PNG 무손실 재주입**: 이미지 화질 손상 없이 번역된 메타데이터를 바이너리 레벨에서 다시 구워내어 RisuAI/실리태번에서 바로 사용 가능.

---

## 📄 License

This project is open-source and licensed under the [MIT License](LICENSE).
Anyone can freely use, modify, and distribute this software.

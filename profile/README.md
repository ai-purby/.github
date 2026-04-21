# 🦊 Purby

> **AI 기반 홈 디바이스 Purby**
> 일상 속 정보와 상호작용을 더 자연스럽게 연결하는 스마트 홈 디스플레이

<p align="center">
  <img src="./assets/purby-hero.png" alt="Purby AI smart home companion concept image" width="100%" />
</p>

---

## ✨ Overview

**Purby**는 시간, 날씨, 일정과 같은 생활형 정보를 한눈에 보여주고,
음성 상호작용을 통해 사용자와 자연스럽게 소통하는 **AI 기반 스마트 홈 디바이스**입니다.

기존의 생활 정보 확인은 스마트폰 앱, 위젯, 포털 검색에 의존하는 경우가 많았습니다.
Purby는 이러한 반복적인 정보 탐색 과정을 줄이고,
사용자 공간 안에서 **항상 켜져 있는 홈 어시스턴트**로 동작하는 것을 목표로 합니다.

단순한 정보 표시 장치를 넘어,
캐릭터 기반 인터페이스와 음성 인터랙션을 통해 **더 친근하고 지속적으로 함께하는 디바이스 경험**을 제공합니다.

---

## 🎯 Project Goals

* 생활형 정보(시간, 날씨, 일정)를 직관적으로 제공
* 음성 명령 기반의 자연스러운 인터랙션 구현
* 캐릭터 중심 UI를 통한 감성적 사용자 경험 제공
* 디바이스 / 서버 / 모바일 간의 유기적인 연동 구조 설계
* 생성형 AI를 실생활 인터페이스로 확장하는 새로운 사용 방식 제안

---

## 🖥️ Main Features

### 1. 홈 화면 정보 제공

* 현재 시간 및 날짜 표시
* 실시간 날씨 및 상태 표시
* 오늘의 일정 요약 제공
* 한 화면에서 모든 핵심 정보 확인 가능

### 2. 음성 기반 상호작용

* 호출어 기반 음성 인식
* 사용자 발화를 STT로 변환
* AI가 의도를 파악하여 적절한 기능 수행
* TTS를 통해 자연스럽게 응답 반환

### 3. 캐릭터 인터페이스

* Purby 캐릭터가 상태에 따라 반응
* 예: Idle / Listening / Thinking / Sleep / Error
* 디바이스를 단순한 화면이 아닌 **살아있는 홈 파트너**처럼 느끼게 설계

### 4. 스마트 홈 디스플레이 경험

* 공부, 일정 확인, 생활 관리에 적합한 상시형 디스플레이
* 모바일 앱과 연동하여 설정 및 일정 관리 가능
* 가정 내 고정형 AI 디바이스로 활용 가능

---

## 🧩 System Architecture

Purby는 크게 **디바이스**, **백엔드 서버**, **모바일/관리 인터페이스**로 구성됩니다.

### Device

* 디스플레이 화면 출력
* 캐릭터 UI 렌더링
* 음성 입력 처리
* 사용자와의 실시간 인터랙션 담당

### Backend Server

* STT / TTS / LLM 연동
* 일정, 날씨, 타이머 등 기능 라우팅
* 사용자 요청 처리 및 응답 생성
* 데이터 저장 및 상태 동기화 관리

### Mobile / Client

* 사용자 설정 관리
* 일정 입력 및 디바이스 연동
* 배경, 알림, 환경설정 제어

---

## ⚙️ Tech Stack

### Frontend / Device UI

* Electron
* React
* Zustand
* Tailwind CSS
* Three.js

### Backend

* FastAPI
* PostgreSQL
* Redis
* Docker / Docker Compose

### AI / Voice

* Wake Word Detection
* STT (Speech-to-Text)
* LLM 기반 Intent Analysis
* TTS (Text-to-Speech)

### Design / 3D

* Blender
* Mixamo

---

## 🔄 Interaction Flow

1. 사용자가 호출어로 Purby를 활성화
2. 디바이스가 음성을 수집하여 서버로 전달
3. 서버가 STT를 통해 텍스트로 변환
4. LLM이 사용자의 의도를 분석
5. 필요한 기능(날씨, 일정, 타이머 등)을 수행
6. 응답 내용을 TTS로 변환
7. Purby가 음성과 화면으로 사용자에게 응답

---

## 📌 Expected Value

* 반복적인 생활 정보 접근을 더 빠르고 자연스럽게 개선
* AI를 생산성 도구가 아닌 **생활형 인터페이스**로 확장
* 캐릭터 UX를 통해 사용자와 디바이스 간 친밀도 형성
* 홈 디스플레이 시장에서 감성적 AI 디바이스 가능성 제시

---

## 🚀 Future Work

* 사용자 맞춤형 메모리 및 장기 컨텍스트 반영
* 공부/집중 모드 등 상황 인식 기능 확장
* 모바일 앱 연동 고도화
* 더 자연스러운 한국어 음성 합성 적용
* 디바이스 하드웨어 완성도 향상
* 캐릭터 애니메이션 및 상태 표현 다양화

---

## 👥 Team

> Purby는 AI, 디바이스, UX를 결합하여
> **생활 속에서 자연스럽게 함께하는 스마트 홈 디바이스**를 만드는 프로젝트입니다.

필요에 따라 팀원 역할, 담당 파트, 시연 영상 링크, 발표 자료 링크 등을 이곳에 추가할 수 있습니다.

---

## 📝 Repository Structure

```bash
Purby/
├── device/         # 디바이스 클라이언트 및 화면 UI
├── server/         # FastAPI 기반 백엔드 서버
├── mobile/         # 모바일 또는 관리용 클라이언트
├── assets/         # 이미지, 캐릭터, 디자인 리소스
├── docs/           # 기획서, 보고서, 발표 자료
└── README.md
```

---

## 💡 One Line Introduction

**Purby는 시간, 날씨, 일정, 음성 상호작용을 하나로 연결한 AI 기반 스마트 홈 디바이스입니다.**

---

## 📷 Preview

상단 대표 이미지는 Purby가 지향하는 스마트홈 디스플레이 경험과 캐릭터 기반 AI 인터랙션을 시각화한 콘셉트 이미지입니다.

추후 홈 화면 캡처, 시스템 아키텍처 다이어그램, 시연 GIF 또는 영상 링크를 함께 추가할 예정입니다.

---

## 📄 License

This project is for academic / prototype purposes.

---

<div align="center">
  <b>Purby</b><br/>
  AI-powered Home Device for Everyday Life
</div>

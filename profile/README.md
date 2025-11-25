# 🧊 대표 프로젝트: CookUs

> 냉장고 재료 기반 레시피 추천 + 식단·영양제 관리 + 데이터 대시보드

CookUs는 사용자의 냉장고 재료를 기반으로 레시피를 추천하고,  
캘린더에 식단과 영양제 섭취를 기록하며, 데이터 대시보드를 통해  
**습관·패턴을 눈에 보이게 만드는 헬스케어 서비스**입니다.

- 냉장고 재료 입력 → 레시피 추천 → 캘린더 기록 → 영양제/식단 리포트
- 요리·섭취 기록을 기반으로 뱃지/리워드를 제공하는 **가볍지만 끈기 있게 이어갈 수 있는 서비스**를 목표로 합니다.
- 프론트, 백엔드, 대시보드, 인프라까지 **모두 직접 설계·구현·배포**했습니다.

<br>

## 👋 건전지팀 (Team GeonJeonJi)

냉장고 재료부터 식습관 데이터까지,  
**사용자의 일상을 조금 더 편하게 만드는 데이터 기반 서비스**를 만드는 팀입니다.  

LG U+ WhyNot Camp 7기에서 시작해,  
기획 → 설계 → 개발 → 배포 → 데이터 분석까지 **엔드투엔드로 직접 경험**한 프로젝트들을 운영하고 있습니다.

<br>


| 홍가연 | 박민상 | 김지영 | 신윤서 | 
|:------:|:------:|:------:|:------:|
| <img width="150" alt="hong" src="https://github.com/user-attachments/assets/9fa60bb2-6686-45f5-8b2f-d95d18834c74" /> | <img width="150" alt="park" src="https://github.com/user-attachments/assets/235c9ffe-99cb-4f7e-9187-3fc6bae16d77" /> | <img width="150" alt="kim" src="https://github.com/user-attachments/assets/cde8666b-9632-44a4-96c6-054f061d8e24" /> | <img width="150" alt="shin" src="https://github.com/user-attachments/assets/aedcdaa7-ef0d-46a4-a3ed-ac6b22aa711e" /> |
| PM · Frontend | 데이터 분석 · DB | 기획 · Backend | 데이터 엔지니어 · DB |

- **홍가연**: 전체 PM, 요구사항 정의, 프론트엔드 구현, 인프라/대시보드 설계
- **박민상**: 백엔드·DB 설계, 쿼리 튜닝, 배포 파이프라인 구축
- **김지영**: 서비스 기획, 화면 설계, 백엔드 주요 기능 구현
- **신윤서**: 데이터 파이프라인·DB 모델링, 기능 개발 및 테스트

<br>

---

## 📂 Repository Overview

이 Organization에는 CookUs 관련 레포지토리가 다음과 같이 구성됩니다.

- **`cookus-frontend`**  
  React + TypeScript 기반 웹 프론트엔드  
  - 냉장고 재료 관리, 레시피 추천 화면
  - 식단 캘린더, 요리 타이머, 뱃지/대시보드 진입 UI

- **`cookus-backend`**  
  FastAPI 기반 백엔드 API 서버  
  - 회원·인증(JWT), 냉장고 재료, 레시피 추천, 캘린더, 영양제, 뱃지 API
  - MariaDB와 연동되는 도메인 모델·쿼리 구현

- **`cookus-dashboard`** (Private)  
  Streamlit 기반 데이터/운영 대시보드  
  - 기간별 요리 횟수, 카테고리별 조리 비율
  - 사용자 기록 기반 통계·모니터링 뷰

- **`CookUs-docs`** (Private)  
  CookUs 최종 산출물 모음  
  - 프로젝트 계획서, 요구사항 정의서, ERD, 시스템 아키텍처, API 명세, 테스트 시나리오 등 문서 저장소

> 각 레포의 설치/실행 방법 및 상세 구조는 해당 레포의 `README.md`를 참고합니다.

<br>

---

## 🚀 서비스 한눈에 보기

- **서비스 목적**
  - 냉장고에 이미 있는 재료를 활용해 “오늘 뭐 먹지?” 고민을 줄이고,
  - 요리 기록과 영양 루틴을 함께 관리하여 **꾸준한 식습관 형성**을 돕는 서비스

- **핵심 기능**
  1. **냉장고 재료 관리**
     - 보유 재료 등록/수정/삭제  
  2. **맞춤 레시피 추천**
     - 사용자의 재료를 기반으로 레시피 후보 추천  
     - 난이도 필터로 “지금 가능한 레시피”만 좁혀서 제공  
  3. **식단 캘린더 & 요리 타이머**
     - 선택한 레시피를 날짜별 캘린더에 기록  
     - 요리 중 타이머 사용, 요리 완료 체크 → 통계 및 뱃지에 반영  
  4. **영양제 루틴 관리**
     - 복용 중인 영양제 등록, 캘린더에서 복용 체크  
     - “오늘의 영양 루틴 완료” 피드백 제공  
  5. **대시보드 & 뱃지**
     - 기간별 요리 횟수, 카테고리 비율 시각화  
     - 첫 요리·연속 기록 등 뱃지로 가벼운 성취감 제공  

> 냉장고 재료 → 레시피 추천 → 식단/영양 루틴 기록 → 대시보드 인사이트까지  
> **사용자의 “요리 습관”을 데이터로 설계한 서비스**입니다.

<br>

---

## 🏗 시스템 아키텍처

<img width="1537" height="1269" alt="CookUs_시스템아키텍처" src="https://github.com/user-attachments/assets/1d1712cb-8251-41d3-a1fc-6187bb357c6c" />

- **EC2 분리 구성**
  - Backend 전용 EC2 1대
  - Frontend + Dashboard용 EC2 1대

- **컨테이너 기반 배포**
  - 서비스별 Docker 이미지 빌드 후, 각자 ECR에 저장
  - EC2에서 이미지 pull → 컨테이너 실행

- **GitHub Actions 기반 CI/CD**
  - main 브랜치 푸시 시 자동 빌드·ECR 푸시
  - 원격 EC2에서 최신 이미지로 재배포  
  → 코드 변경 후 **“git push”만으로 배포**까지 이어지는 파이프라인

<br>

---

## 🛠 공통 기술 스택

**Frontend**  
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=000000)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=FFFFFF)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=FFFFFF)

**Backend**  
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=FFFFFF)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=FFFFFF)
![Uvicorn](https://img.shields.io/badge/Uvicorn-4B8BBE?style=flat-square)

**Database**  
![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=flat-square&logo=mariadb&logoColor=FFFFFF)

**Infra & DevOps**  
![AWS EC2](https://img.shields.io/badge/EC2-FF9900?style=flat-square&logo=amazonec2&logoColor=FFFFFF)
![AWS ECR](https://img.shields.io/badge/ECR-FF9900?style=flat-square&logo=amazonaws&logoColor=FFFFFF)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=FFFFFF)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=FFFFFF)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=FFFFFF)

**Data / Analytics (Dashboard)**  
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=FFFFFF)

<br>

---

## 📑 문서 산출물 (CookUs-docs)

프로젝트 문서는 `CookUs-docs` 레포에 정리되어 있습니다. 예:

- 프로젝트 계획서
- 요구사항 정의서
- ERD 및 스키마 설계서
- 시스템 아키텍처 다이어그램
- API 명세서
- 테스트 시나리오 및 결과

멘토·심사위원·협업자가 “CookUs가 어떤 서비스이고, 어떻게 만들어졌는지”를  
빠르게 이해할 수 있도록 문서 중심으로 정리했습니다.

# Brain Tumor - LLM + RAG Report
# 🧠 뇌종양 분석 및 RAG를 활용한 자동 의학 소견 생성 시스템 구축

## 📅 진행 기간

2024년 10월 10일 ~ 2024년 12월 6일

🚩 프로젝트 개요

이번 프로젝트의 목표는 뇌종양 분야의 의료 영상을 분석하고, 자동으로 전문 의학 소견을 생성하는 시스템을 구축하여 의료진의 진단과 의사 결정을 지원하는 것입니다.

🎯 목적

MRI 촬영 결과 및 상담 데이터를 활용하여 의료진의 소견서 작성 자동화

RAG(제거형 생성기, Retrieval-Augmented Generation) 기술을 통해 실시간으로 최신 의학 정보를 제공

3D Segmentation 기술과 SwinUnetR 모델을 사용해 종양의 위치를 정밀하게 예측

사용하기 쉬운 UI를 제공하여 의료진의 업무 효율성 향상

📂 사용 데이터

임상 데이터(Med42, Hugging Face)

주요 증상과 병력을 추출하여 소견서 자동 생성

ChatGPT를 활용해 가상의 의료 상황 및 데이터를 추가 생성

BraTS 데이터셋(2018, 2020, 2021 버전)

T1, T2, FLAIR, T1ce 4가지 MRI 촬영 기법으로 구성

종양의 위치 및 종류를 시각적으로 확인하고 Segmentation 작업 활용

의학 전문 데이터(PDF, Adams and Victor's Principles of Neurology 8th Edition)

PostgreSQL DB에 저장 후 RAG 기술에 활용

뇌 영역별 구조적 특징, 손상 정보, 종양의 특성 포함

⚙️ 진행 과정

1. 임상 상담 기록 분석 및 소견서 자동화

육하원칙(누가, 무엇을, 언제, 어디서, 왜, 어떻게)에 기반한 모델 설계

Llama3 8B 및 Gemma2 9B 모델을 활용해 텍스트 요약 및 자동화 파이프라인 구축

2. MRI 이미지 Segmentation 작업

3D U-Net 및 SwinUnetR 모델 적용

FLAIR 데이터를 활용해 종양의 위치 및 크기 분석

AAL(AAL atlas) 데이터를 통해 뇌 영역별 종양 위치 출력

3. 데이터 검색 및 요약 시스템 구현

RAG 및 LLM(Ollama의 Gemma2 모델) 기술 활용

PostgreSQL + PGVector를 사용해 고속 검색 및 인덱싱 성능 강화

🚀 결과

FastAPI 기반의 의료진 진단 지원 시스템 구축

MRI Segmentation 결과 및 뇌 영역별 정보 신속 조회 가능

폐쇄망 환경에서도 로컬 LLM을 사용해 데이터 보안 유지

반복적인 문서 작업 부담 감소 및 진단 효율성 극대화

📈 성능

SwinUnetR 모델과 FLAIR 데이터 결합 시 최상의 성능 달성

3D Segmentation 작업의 정확도 및 예측 효율 향상

🛠️ 사용 기술 및 라이브러리

프레임워크: FastAPI

모델: 3D U-Net, SwinUnetR

데이터베이스: PostgreSQL, PGVector

LLM: Ollama (Gemma2 모델)

👨‍👩‍👧‍👦 팀원

( 2 )조 - [누구나 AI] 딥러닝 부트 캠프 10기

📧 문의

이메일: cgygy@naver.com


https://github.com/user-attachments/assets/4831aa1c-cd4e-4905-820a-56040099c75d


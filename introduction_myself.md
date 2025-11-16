# Intro
1. AI 역량을 꾸준히 쌓아옴
2. 어떻게 최신 AI 기술을 학습하고, 쫓아갈지 고민해옴.
3. 훌륭한 엔지니어 인력이 무엇일지 고민하며 성장해옴.

# Skill
## Language
- Base : Python, Javscript, C++
- Infra : Terraform

## AI
- Training Workflow : Kubeflow, MLflow
- Model Versioning : MLflow
- Model Serving : KServe, MLflow
- Training : PyTorch, Keras(TF2.0)
- Data Versioning : DVC

## Computer Vision
- OpenCV

## Infra
- Orchestration of containers
    - Onpresmise : Docker Compose, Kubernetes
    - AWS : ECS, EKS
- CI/CD : Github Actions, Gitlab CI/CD

## Backend
- FastAPI, Express.js

## Frontend
- Web : React + Vite
- Mobile : React Native(Expo)

## Embedded
- AVR, ROS2

# Experience
## 1. ReconLabs <주식회사 리콘랩스>
- 2023.10 - Present
- Position : MLOps Engineer/Development Team

### 1-1. 디자이너 의도 기반 디자인 탐구 AI Assistant Project
- 목표 : Strands, LangGraph 기반 Agent 설계 및 개발
- 기간 : 2025. 03 ~ Present
- 주요 역할
    - 기존 AWS Lambda 에서 AWS Bedrock의 AgentCore Runtime으로 전환
    - 기존 Serverless Message Queue 기반의 AgentCore 기반 배포 아키텍처 설계
        - Consumer : AWS Lambda
        - Agent : AgentCore Runtime
        - MCP : AgentCore MCP
        - Memory : Short-term Memory
- 성과
    - 연구팀의 디자인 탐구 Assistant 배포 속도 기존 1주일에서 1일로 단축
    - 기존 Commit 단위 버저닝에서 AgentCore의 Model 버저닝으로 Agent 관리 효율성 향상

### 1-2. 3D 생성형 모델 서빙 인프라 비용 최적화
- 목표 : 3D 에셋 생성 파이프라인 운영 비용 절감
- 기간 : 2024. 09 ~ 2024. 12
- 주요 역할
    - 기존 Kubeflow Pipeline 환경을 ECS 기반 Container Service로 전환
    - Flux, Hunyuan3D, Step1X-3D 모델을 Triton 기반 API 형태로 서빙 환경 구축
- 성과
    - 일일 운영 비용을 기존 $200에서 $50으로 75% 절감

### 1-3. 3D Asset 생성 엔진 표준화 
- 목표 : 기존 EC2 기반 정적 파이프라인에서 Kubeflow로 전환
- 기간 : 2023. 10 ~ 2024. 09
- 주요 역할
    - Kubeflow 기반 동적 파이프라인으로 아키텍처 재구성
        - 기존 Serverless Message Queue를 바탕으로 Pipeline 아키텍처 설계
            - Controller, Kubeflow Pipeline 간 통신 구현
        - 전처리 - 학습 - 후처리 단계를 컨테이너 모듈 단위로 관리
    - NeRF, Gaussian Splatting 기반 3D 에셋 생성 파이프라인 구축 및 운영
- 성과
    - 온프레미스 GPU 자원 효율 증가 
        - 기존 docker compose를 통한 모델별 GPU 점유에서 자동 GPU 지정으로 온프레미스 자원 사용성 증가

## 2. Arbeon <알비언>
- 2023.01 - 2023.09
- Position : MLOps Developer/AI Team

### 2-1. 모델 서빙 및 API 배포 파이프라인 구축
- 목표 : 개발자가 직접 배포 가능한 모델 서빙 자동화 및 운영 파이프라인 구축
- 기간 : 2023. 06 ~ 2023. 09
- 주요 역할
    - 모델 서빙 FastAPI 추론 서버 코드 작성
    - 모델 배포를 위한 GitLab CI/CD 파이프라인 구성
- 성과
    - DevOps 팀 개입 없이 AI 팀 주도 서빙 및 배포
        - 기존 배포 및 테스트 기간 1일에서 1시간으로 단축
        - 모델 버저닝으로 배포 프로세스 효율성 75% 증가

### 2-2. MLOps 실험 인프라 구축
- 목표 : 분산된 실험 환경 통합 및 재현 가능한 학습 환경 운영
- 기간 : 2023. 01 ~ 2023. 06
- 주요 역할
    - 연구자 실험 환경 통합을 위한 Kubeflow Notebook 환경 제공
    - MLflow 기반 모델 버전 관리 환경 구축
        - Storage : NAS
            - 실험 로그, 모델 및 부산물 저장
    - GPU 리소스 자동 분배 환경 구축
- 성과
    - 온프레미스 GPU 자원 활용 50% 에서 85%로 증가
    - 실험 환경 통합으로 실험 재현성 개선
    - 모델 버저닝으로 배포 프로세스 효율성 75% 증가

## 3. Neubility <주식회사 뉴빌리티>
- 2021.11 - 2022.12
- Position : AI Engineer/Perception Team

### 3-1. MLOps 기본 파이프라인 구축
- 목표 : 지속적인 학습 파이프라인 구축
- 기간 : 2021. 11 ~ 2022. 12
- 주요 역할
    - 수집된 데이터 업로드/추출/라벨링 환경 구축
        - Django 기반 API 서버 구축
            - 수집 데이터 자동 업로드
            - 라벨링 데이터 자동 추출
        - CVAT 기반 라벨링 환경 구축
            - Semi auto labeling 시스템 적용
    - AzureML의 Mlflow 기반 실험 추적 환경 구축
        - 실험 단위 버저닝으로 결과 비교 관리 체계화
    - 분산 학습 시스템 구성
        - Celery 기반 분산 학습 환경 구축
- 성과
    - 지속적 학습 파이프라인으로 계절별 모델 드리프트 현상 해결
        - 계절별 데이터 지속적 학습으로 객체 인식률(객체 분류 정확도) 90% 증가
    - 기존 데이터 가공 프로세스 기간을 1주일에서 1일로 단축

### 3-2. 객체 위치 추정 모듈 개발
- 목표 : 자율주행 로봇의 후방 위험요소 회피
- 기간 : 2022. 09 ~ 2022. 12
- 주요 역할
    - 후방 카메라를 통한 객체 위치 추정 모듈 개발
- 성과
    - 골프장 자율주행 로봇의 후방 위험요소 회피율 99% 달성

## 4. SAMJIN LND <(주)삼진엘앤디>
- 2020.02 - 2021.03
- Position : AI Engineer/Development Team

### 4-1. 카메라 렌즈 AI 먼지 검출 시스템 개발
- 목표 : 마이크로 단위 표면 먼지 세그먼트 검출
- 기간 : 2020. 08 ~ 2021. 03
- 주요 역할
    - 먼지 검출 논문 조사 및 로직 구현
        - Keras(TF 2.0) 기반 DeepLabV3 Network 구현
    - 고객 데이터 확보 및 전처리
    - 추론 코드 컨테이너화
- 성과
    - F1-score 95% 이상 성능 달성 및 납품

### 4-2. ESS 미성형 Computer Vision 기반 검출 시스템 개발
- 목표 : 제품 미성형 검출
- 기간 : 2020. 02 ~ 2020. 08
- 주요 역할
    - 고객 데이터 기반 미성형 검출 실험
        - 미성형 시 해당 부분 반사 정도를 이용한 검출 실험
    - 미성형 검출 로직 개발
        - 반사 부분 Contours 영역 검출 로직 개발
        - 정상 제품들과 Histogram 유사도 검출 로직 개발
    - 추론 코드 컨테이너화
- 성과
    - Accuracy 98% 이상 성능 달성 및 납품

# Education
- Seoul National University of Science and Technology
    - 2014.03 ~ 2020.02
    - Bachelor of Science in Mechanical System Design

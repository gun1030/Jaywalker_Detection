# 🚦 세종 자율주행 관제 데이터 기반 보행자 및 무단횡단 탐지

## 프로젝트 개요
본 프로젝트는 세종시 자율주행 시범운행지구의 CCTV 데이터를 활용하여  
보행자 및 무단횡단 여부를 탐지하는 AI 시스템을 개발하는 것을 목표로 합니다.

- 목적: 보행자 안전 확보 및 스마트시티 구현
- 활용 데이터: CCTV (세종시 자율주행 관제 데이터)


---

## 문제 정의
기존 CCTV 시스템은 단순 모니터링에 그치며,  
보행자의 돌발 상황(무단횡단 등)을 자동으로 감지하지 못합니다.

본 프로젝트에서는  
- 보행자 탐지
- 무단횡단 여부 분류를 동시에 수행하는 AI 모델을 구축합니다.

---

## 모델 및 기술 스택

### 🔹 사용 모델
- YOLOv8 (Object Detection)
- Segmentation 모델을 활용한 도로 영역 분리

### 🔹 데이터 처리
- Bounding Box 기반 라벨링
- 클래스 구성:
  - 0: Jaywalker (무단횡단)
  - 1: Pedestrian (정상 보행자)

### 🔹 개발 환경
- Python
- PyTorch
- Google Colab pro(A100 GPU)

---

## 🖼️ 결과 이미지

### 🔹 Detection 결과 예시

![result image](https://github.com/user-attachments/assets/c6d4719e-f5aa-4b6e-a598-d6751f64c3be)


> 파란 박스: 무단횡단 보행자  
> 민트 박스: 정상 보행자

---

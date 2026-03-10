# Vehicle_license_plate_recognition

> A YOLOv5 and OCR-based license plate recognition pipeline for vehicle number localization and text extraction.

![License Plate Detection](https://github.com/lee-seong-wook/Vehicle-license-plate-recognition/assets/130055880/4f000257-c431-4d82-aa91-cc027468264f)

## Overview
Vehicle_license_plate_recognition은 Colab 환경에서 YOLOv5 번호판 검출 모델과 OCR 후처리를 연결해 번호판 텍스트 추출 흐름을 검증한 프로젝트입니다. 짧은 기간 안에 데이터셋 준비, 검출 모델 실험, OCR 적용을 하나의 워크플로우로 정리하는 데 초점을 두었습니다.

## Project Context
| Item | Details |
| --- | --- |
| Context | Industry-linked project with (주)더브레인에스 |
| Period | 2023.08.20 ~ 2023.08.22 |
| Goal | 차량 번호판 검출과 문자 인식을 결합한 인식 파이프라인 구현 |
| Scope | YOLOv5 학습, 데이터셋 구성, 추론 실험, OCR 적용 |

## My Role
- 단일 참여자로 번호판 검출과 OCR 적용 파이프라인을 직접 정리했습니다.
- Colab 환경에서 YOLOv5 학습과 추론 실험을 구성했습니다.
- Roboflow 데이터셋 활용과 OCR 적용까지 포함해 번호판 인식 흐름을 문서화했습니다.

## Tech Stack
`Python`, `YOLOv5`, `Google Colab`, `Roboflow`, `OpenCV`, `PyTorch`, `Tesseract OCR`, `pytesseract`

## Key Contributions
- YOLOv5 기반 번호판 검출 모델 학습 및 추론 파이프라인 구성
- Roboflow 데이터셋 다운로드와 학습 환경 설정 정리
- 검출 결과 이미지에 대한 OCR 적용 실험
- 짧은 프로젝트 기간 안에 검출과 인식을 연결한 실습형 워크플로우 정리

## Implementation Notes
- `차량_번호판_인식.ipynb`: 데이터셋 다운로드, YOLOv5 학습, 검출, OCR 적용을 포함한 메인 노트북
- 노트북에서는 YOLOv5 저장소를 클론하고 학습 환경을 설치한 뒤, Roboflow 데이터셋을 내려받아 학습을 진행합니다.
- 이후 `pytesseract`와 `tesseract-ocr`를 사용해 번호판 텍스트 추출을 실험합니다.

## How to Run
1. `차량_번호판_인식.ipynb`를 Google Colab에서 엽니다.
2. YOLOv5 환경 설치 셀과 데이터셋 다운로드 셀을 순서대로 실행합니다.
3. 학습 또는 추론 후 OCR 셀을 실행해 텍스트 추출 결과를 확인합니다.

## Workflow Example
![License Plate Workflow Example](https://github.com/lee-seong-wook/Vehicle-license-plate-recognition/assets/130055880/726ec51e-3f6e-4793-89c3-4f48ef2bb538)

<details>
<summary>Participant</summary>

| Name | Role |
| --- | --- |
| 이성욱 | 번호판 검출 및 OCR 파이프라인 구현 |

</details>

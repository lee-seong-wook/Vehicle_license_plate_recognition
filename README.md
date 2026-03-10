# Vehicle_license_plate_recognition

> A YOLOv5 and OCR-based license plate recognition pipeline for vehicle number localization and text extraction.

## Overview
Vehicle_license_plate_recognition은 차량 번호판 영역을 검출한 뒤 OCR로 문자와 숫자를 읽어내는 프로젝트입니다. YOLOv5 기반 검출 모델 학습과 추론 실험을 진행하고, 이후 OCR을 적용해 번호판 텍스트를 추출하는 흐름으로 구성했습니다. 짧은 기간 안에 검출과 인식을 하나의 파이프라인으로 묶는 데 초점을 둔 프로젝트입니다.

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

## Project Gallery
| Detection Result | Additional Example |
| --- | --- |
| ![License Plate Detection](https://github.com/lee-seong-wook/Vehicle-license-plate-recognition/assets/130055880/4f000257-c431-4d82-aa91-cc027468264f) | ![License Plate Example](https://github.com/lee-seong-wook/Vehicle-license-plate-recognition/assets/130055880/726ec51e-3f6e-4793-89c3-4f48ef2bb538) |

<details>
<summary>Participant</summary>

| Name | Photo | Role |
| --- | --- | --- |
| 이성욱 | ![이성욱](https://github.com/lee-seong-wook/Vehicle-license-plate-recognition/assets/130055880/b560398b-4f23-4403-8c55-099213266525.png) | 번호판 검출 및 OCR 파이프라인 구현 |

</details>

# 최재홍 · JaeHong Choe

**Vision AI Engineer** — 반도체 부품 제조 현장의 비전 검사와 판정 자동화

현장 데이터는 불량이 드물고 라벨도 깔끔하지 않습니다. 모델 구조보다 문제를 어떤 단위로 볼지, 무엇을 기준으로 평가할지를 먼저 정하는 편입니다.
요즘은 운영 중에 다시 학습해도 결과가 나빠지지 않게 하는 방법에 관심이 많습니다.

[Email](mailto:jae_apple@naver.com) · [LinkedIn](https://www.linkedin.com/in/jaehong-choe-460831251/) · [Notion](https://www.notion.so/Jay-s-Notion-0ed2c9b6f92b4d35b1fc64cb340449fe)

<br>

## Experience

**MiCo AI** (구 AICESS) · Vision AI Engineer · 2025.09 – 현재

반도체 부품 검사·판정 AI 프로젝트를 문제 정의부터 모델, 평가 기준, 현장 검증까지 맡고 있습니다.

- **반입 부품 불량 판정** — 이미지 단위로 막혀 있던 과제를 제품 단위 MIL로 다시 정의하고, 1차 NG 후보만 VLM이 재판정하도록 구성. Recall을 유지한 채 과검 28~33% 감소, 사람 검토 결과를 LoRA 학습으로 연결 (비공개)
- **MES 처리 판정과 재학습 안전장치** — 입고 이력으로 공정 투입·반송·수리를 판정하는 학습 파이프라인. 늦게 확정되는 라벨에서 미래 정보가 섞이지 않게 하고, 재학습 모델이 특정 고객사에서 나빠지면 교체를 막는 기준 설계 · [repo](https://github.com/JaeHongChoe/industrial-mes-continual-learning)
- **외관 결함 패치 분류** — 원본 해상도 패치 + DINOv3. 실제 불량은 기준 고정 후 마지막 평가에만 사용 · [repo](https://github.com/JaeHongChoe/industrial-visual-qc-dinov3)
- **라인스캔 엠보 검사 엔진** — 장당 약 8억 화소 이미지에서 표면 돌기 수천 개를 전수 검사, 딥러닝 없이 영상처리와 격자 통계로 구성 (PoC 계수 일치율 99.9%) · [repo](https://github.com/JaeHongChoe/industrial-emboss-inspection-linescan)
- **초음파 결함 분할** — 결함 샘플이 거의 없는 환경에서 정상 위주로 학습하는 DRAEM, 가성 결함 합성 · [repo](https://github.com/JaeHongChoe/industrial-draem-anomaly-segmentation)
- **X-ray 구조 계측** — 원형 구조·핀·지그·V홀 자동 검출과 편심 계산, 브라우저 일괄 처리 PoC · [repo](https://github.com/JaeHongChoe/industrial-xray-geometry-measurement)

**아하랩스** · Solution Engineer · 2024.07 – 2025.03

- 2차전지 제조사 대상 파우치형 배터리 품질 모니터링 솔루션 도입·안정화. L3/L4 이중화 네트워크와 Failover 구성
- 실시간 품질 데이터 수집·저장 백엔드 구현, 운영 중 메모리 누수를 찾아 월 1회 PC 재부팅이 필요하던 문제 해소
- 규칙 기반 용접 데이터 이상 감지 로직 라인 배포, 이기종 데이터 통합 PoC

**MMCLab, 한림대학교** · 연구원 · 2021.07 – 2023.03

- **3D 프린팅 포렌식** — 출력물 표면 텍스처로 프린터를 식별하는 멀티모달 네트워크 설계, 장치 식별 정확도 95%. IEEE TMM 게재, 특허 등록 · [repo](https://github.com/juhou/SI3DPpp)
- **의료 영상 데이터 증강** — Pix2Pix로 신장·종양 CT를 생성해 분할 학습에 추가, U-Net IoU 58% → 90% · [repo](https://github.com/JaeHongChoe/SMIAIP)
- **위장관 출혈 예측** — DOAC 복용 환자 데이터로 AutoML 모델 비교·선정, 이후 외부 검증 연구로 SJG 2025 게재

<br>

## Projects

- **자율주행 데브코스** (Programmers, 2023.09 – 2024.02) — YOLOv7 Tiny를 TensorRT로 변환해 1:10 차량에 배포(약 40 FPS), Camera·LiDAR 센서 퓨전 실험 · [object detection](https://github.com/JaeHongChoe/Object_detection-Depth_estimation-project) · [sensor fusion](https://github.com/JaeHongChoe/Camera_3DLiDAR_Object_Detection)

<br>

## Publications & Patent

- I. Kim, J.-U. Hou, **J. H. Choe**, et al. "Validation of a machine learning model for predicting gastrointestinal bleeding in patients with direct oral anticoagulants." *Scandinavian Journal of Gastroenterology*, 60(11), 2025. [[paper]](https://doi.org/10.1080/00365521.2025.2565321)
- B. S. Shim, **J. H. Choe**, J.-U. Hou. "Source Identification of 3D Printer Based on Layered Texture Encoders." *IEEE Transactions on Multimedia*, vol. 25, 2023. [[paper]](https://ieeexplore.ieee.org/document/10005625) [[code]](https://github.com/juhou/SI3DPpp)
- **J.-H. Choe**, S.-L. Lee, Y.-J. Seo, W.-J. Seo, J.-U. Hou. "Generative Adversarial Networks Based Data Augmentation to Address Medical Data Imbalances." *KIPS Conference (ACK)*, 2022. 우수 논문상 [[paper]](http://koreascience.or.kr/article/CFKO202233649535454.page) [[code]](https://github.com/JaeHongChoe/SMIAIP)
- 특허 10-2022-0122680 「3D 프린팅 된 객체의 이미지를 바탕으로 3D 프린터를 식별하는 신경망 기반의 전자 장치」, 2022

<br>

## Awards

- 국방 AI 경진대회 3등 · 국방부·과학기술정보통신부 · 2023.12
- ACK 추계학술대회 우수 논문상 · 한국정보처리학회 · 2022.11
- KB국민은행 소프트웨어 경진대회 장려상 · 2022.11
- 한림대 빅데이터·AI 해커톤 최우수상 · 2022.04
- 한림대 HBC-5 딥러닝 해커톤 1등 · 2021.11

<details>
<summary>그 밖의 대회</summary>

- 교내 Kaggle: 로봇 표면 탐지 1위(2022), 뇌신호 알파벳 분류 1위, 휴먼 액티비티 인식 2위(2021)
- DACON: Computer Vision 이상치 탐지 67/481, 생육 환경 최적화 27/137(2022), 카메라 이미지 품질 향상 110/228(2021)
- Kaggle: Body Morphometry Kidney and Tumor 10/27(2021)
- 21 SW 아이디어 대회 동상

</details>

<br>

## Mentoring

- 교내 Python·딥러닝 멘토 (2022.03 – 2023.03) — 학부생 20명 이상, 멘티 경진대회 수상 2건

<br>

## Skills

- **Modeling** PyTorch · DINOv2/v3 · MIL · DRAEM · U-Net · YOLOv7/v8 · LightGBM · scikit-learn
- **VLM** Qwen-VL · Ollama · ms-swift · LLaMA-Factory · LoRA · few-shot / RAG
- **Vision** OpenCV · NumPy · 형태 분석 · 극좌표 변환 · FFT
- **Deploy** ONNX · TensorRT · Docker · PyScript
- **Lang** Python · C++

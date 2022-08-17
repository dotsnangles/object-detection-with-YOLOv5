# image-detection-with-YOLOv5

### Objectives
- 폐기물 객체 인식 모델을 개발하기 위해 AIHub의 생활 폐기물 데이터를 활용해 YOLOv5를 훈련한다.

### Models and Data
- YOLOv5
- AIHub 생활 폐기물 이미지 일부 / TACO 데이터셋 일부

### Envs and Requirements
- Colab, WSL2, Ubuntu, Conda, WandB
- YOLOv5, PyTorch, OpenCV, Pillow, NumPy, Matplotlib

### Progress
- YOLOv5 모델의 규격에 맞춰 어노테이션을 리포맷
- 이미지 크기 조절, 중앙 배치, 패딩, 제로 센터링
- WandB 로그를 통한 훈련 과정 모니터링
- 추가 데이터 후속 훈련 및 추론
- 카메라 연동을 통해 실제 환경에서 시험

### Result
- 부트캠프 객체 인식 팀 프로젝트 1위

### Retrospective
- YOLOv3 실습 이후 객체 인식 어플리케이션의 기획 및 구현을 시도한 프로젝트
- 객체 인식 모델의 성능 평가 지표인 IOU, mAP에 대해 학습
- 평가 지표의 개념을 토대로 객체 인식 태스크를 이해
- YOLO 시리즈의 Backbone-Neck-Head 구조에 대해 세미나를 진행
- Feature Extraction을 수행하는 Backbone의 중요성이 가장 크다는 것을 배움
- 훈련을 진행하는 과정에서 CUDA out of memory RuntimeError를 처음으로 경험
- Colab 환경에서 훈련이 가능한 체크포인트(YOLOv5m)와 배치 사이즈를 선택
- 최초 훈련 후 추가 데이터로 후속 훈련을 진행했으나 오히려 정확도가 낮아지는 결과가 나옴
- WandB Evaluation Log를 확인해 어노테이션 리포맷의 오류를 발견한 뒤 수정
- 훈련 후 카메라 연동을 통해 모델을 실제 환경에서 시험해봤으나 기대에 못 미치는 결과를 얻음
- 훈련/검증 데이터의 구성에 사용 환경의 맥락이 반영되어 있어야 의도했던 추론 결과를 얻을 수 있음을 배울 수 있었음

### References
- https://github.com/ultralytics/yolov5

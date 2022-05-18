### 생활 폐기물 객체 인식 프로젝트 저장소입니다.

- yolov5
- 데이터셋은 별도 관리합니다.
- 실행 파일: main.ipynb
- train/validation split은 실행 파일에서 가능합니다.
- dataset path와 클래스 설정은 data 폴더의 recyle_detection.yaml에서 가능합니다.
- codesforprep 폴더에 라벨 전처리 관련 프로그램이 모여 있습니다.
- taco dataset 학습 파일은 taco_미니_데이터셋_전이학습_파일.ipynb이며 Kaggle의 YOLOv5 TACO - supercategories를 수정한 것입니다.
- 본 프로젝트의 최종 클래스 분류에 맞춰 기존의 클래스 분류를 간소화했으며 이미지 리사이즈 및 패딩이 추가된 것에 맞춰 bbox값을 수정했습니다.

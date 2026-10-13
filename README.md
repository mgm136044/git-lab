# 로봇제어인공지능 과제 저장소

2026학년도 2학기 "로봇제어인공지능" 수업의 Git 실습과 과제 제출에 쓰는 저장소입니다.

- 학번: 2022136044
- 이름: 민경민
- Hugging Face: [mgm136044](https://huggingface.co/mgm136044)


## 과제

| 과제 | 내용 | 노트북 | 데이터셋 | 상태 |
|---|---|---|---|---|
| 1 | 시연 데이터 수집 및 Hub 업로드 | [assignment_1.ipynb](assignments/assignment_1.ipynb) | [mgm136044/pick-place-cube_20261008_100203](https://huggingface.co/datasets/mgm136044/pick-place-cube_20261008_100203) | 제출 (2026-10-13) |

과제는 모두 5개이며, 나머지 과제도 나오는 대로 `assignments/assignment_N.ipynb`로 올립니다.

과제 1 데이터셋은 SO-101로 테이블 위의 큐브를 집어 회색 패널 영역 안에 놓는 시연 50개입니다(태스크 문장 `Pick and place the cube`, 25fps, overhead·wrist 카메라 2대, 640x480).


## 구성

```text
git-lab/
├── assignments/   과제 노트북 (assignment_N.ipynb)
├── .gitignore
└── README.md
```

녹화 데이터와 체크포인트 같은 큰 파일은 GitHub에 올리지 않습니다. 데이터셋은 Hugging Face Hub에 공개로 올리고, 노트북에는 Hub 주소만 적습니다. `.gitignore`는 `data/`, `output/`, `wandb/`, `*.ckpt`, `__pycache__/`를 추적에서 뺍니다.


## 환경

- Ubuntu 22.04, conda 환경 `lerobot`, Python 3.12
- LeRobot 0.6.0 (`lerobot[all]==0.6.0`)
- 로봇: SO-101 follower / leader


## Git 실습 기록

강의 03의 Git 실습에서 남긴 커밋입니다.

- `6f92790 docs: README 추가`: README 첫 커밋(미션 2)
- `163e310 exp: lr 변경`: 브랜치 실습(미션 4)에서 README에 `lr=0.001시도` 줄 추가. 지금 README에서는 지웠고 내용은 커밋 이력에 남아 있습니다.
- `c7e433f chore: ignore`: `.gitignore` 작성(미션 5)

## 📸 Camera Filter App with OpenCV and MediaPipe

---

## 📁 프로젝트 간략 소개
- **Python**, **OpenCV**, **MediaPipe**를 활용하여 실시간 카메라 필터를 구현.
- 필터를 적용한 이미지를 현재 시간 기반 파일 이름으로 로컬에 저장하는 기능 제공.

---

## 💻 프로젝트 내용

### 🎯 목적
- 실시간 카메라 필터 적용 및 이미지 저장 기능을 통해 사용자 경험 향상.

### 🎣 목표
- a. 다양한 필터를 실시간 카메라 피드에 적용.
- b. 필터가 적용된 이미지를 캡처하여 저장.
- c. 새로운 필터를 쉽게 추가할 수 있도록 구조화된 코드 제공.

---

## 🔄 주요 기능

1. **실시간 필터**:
   - 라이브 카메라 피드에 다양한 필터를 실시간으로 적용.
   - 지원 필터:
     - 얼굴 랜드마크 오버레이
     - 블러 효과
     - 만화 효과
     - 엣지 감지

2. **타임스탬프 기반 이미지 캡처**:
   - 필터가 적용된 이미지를 캡처하고 저장.
   - 저장된 이미지는 현재 시간 기반 파일 이름으로 저장 (예: `capture_20240613_153045.jpg`).

3. **확장 용이성**:
   - `filters.py` 파일에서 필터를 쉽게 추가 또는 수정 가능.

---

## 🖼️ 프로젝트 이미지

### 실시간 모니터링 디스플레이

![Real-Time Monitoring](./output/images/capture.png)

---

## 📊 시스템 아키텍처 다이어그램

### 다이어그램 개요

![System Diagram](./output/images/flowchart.png)

---

## 🛠️ 사용 기술

- **Python**
- **OpenCV**: 실시간 이미지 처리
- **MediaPipe**: 얼굴 검출 및 랜드마크

---

## 📖 설치 및 설정

1. **리포지토리 클론**:
   ```bash
   git clone https://github.com/Kwonsiwoo2/camera_filter_app.git
   cd camera_filter_app
   ```

2. **필요한 라이브러리 설치**:
   ```bash
   pip install opencv-python mediapipe
   ```

---

## 🗂️ 파일 구성

```
project-folder/
|
├── ex.py               # 예제 스크립트 1
├── ex1.py              # 예제 스크립트 2
├── filters.py          # 필터 구현 파일
├── sendver.py          # 추가 스크립트
├── config/             # 설정 파일
├── output/             # 저장된 이미지 출력
├── rsrc/               # 리소스 파일
└── README.md           # 프로젝트 문서화
```

---

## 📖 사용 방법

Python 스크립트를 실행:

```bash
python ex.py
```

**조작 방법**:
- `C` 키를 눌러 이미지를 캡처하고 저장.
- `Q` 키를 눌러 애플리케이션 종료.

저장된 이미지는 `output` 디렉토리에 저장됩니다.

---

## 📝 예제 코드

`filters.py`에서 필터를 적용하는 예제:

```python
import cv2
import mediapipe as mp

def apply_blur(frame):
    return cv2.GaussianBlur(frame, (15, 15), 0)
```

---

## 💡 확장 팁

- `filters.py`에 새로운 필터를 정의하여 쉽게 추가 가능.
- 사용자 정의 필터를 `ex.py` 또는 `ex1.py`에서 가져와 실시간 카메라 피드에 적용.

---

## 🌟 기여 방법

기여를 환영합니다! 문제 제기나 Pull Request를 자유롭게 제출하세요.

---

### 👇 Connect with Me

[![GitHub](https://img.shields.io/badge/GitHub-Profile-blue?logo=github)](https://github.com/Kwonsiwoo2)  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue?logo=linkedin)](https://www.linkedin.com/in/%EC%8B%9C%EC%9A%B0-%EA%B6%8C-064765341/)


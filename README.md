# Python Print Examples — Quick Guide

이 저장소는 Python의 다양한 `print()` 사용법을 담은 예제로 보여주고, VS Code/터미널/Jupyter에서 실행하는 방법을 간단히 정리합니다.


## 파일 목록

### 1) `main_print_v1.py`
- **설명**: 표준 `print()` 활용 종합 예제.
- **동작/기능**:
  - 기본 출력, 여러 값 출력 (`sep`, `end`)
  - f-string / `str.format()` / C 스타일 `%` 포맷
  - 딕셔너리 출력, 멀티라인 출력 (`\n`, 삼중따옴표)
  - 간단한 계산/함수 호출을 포함한 f-string
- **실행 방법**:
  - VS Code: 파일 열고 우측 상단 **Run Python File(▶)**
  - 터미널:
    - Windows: `python main_print_v1.py` (또는 `py main_print_v1.py`)
    - macOS/Linux: `python3 main_print_v1.py`


### 2) `main_print_v2.py`
- **설명**: 콘솔을 보기 좋게 꾸미기 위해 `rich` 라이브러리를 사용하는 예제.
- **동작/기능**:
  - 컬러/스타일 텍스트 출력 (`rich.print`)
  - `Panel`로 박스형 멀티라인 출력
  - `Table`로 딕셔너리/레코드 출력
  - `sep`, `end` 옵션 조합
- **실행 준비**: `pip install rich`
- **실행 방법**:
  - VS Code: 파일 열고 우측 상단 **Run Python File(▶)**
  - 터미널:
    - Windows:
      ```powershell
      pip install rich
      python main_print_v2.py
      ```
    - macOS/Linux:
      ```bash
      pip3 install rich
      python3 main_print_v2.py
      ```


### 3) `main_print_v1.ipynb`
- **설명**: Jupyter Notebook 환경에서 실행 가능한 대화형 파이썬 노트북 파일.
- **동작/기능**:
  - 셀(Cell) 단위 코드 실행 및 출력 결과 실시간 확인
  - 마크다운(Markdown) 셀을 활용한 문서화 및 파이썬 코드 실행
  - 변수 선언, 기본 출력, 여러 값 출력, f-string 실습
- **실행 방법**:
  - VS Code: 파일을 연 후 셀 상단의 **Run All** 클릭 또는 각 셀의 재생 버튼(▶) 클릭
  - Jupyter Notebook / JupyterLab 환경에서 열어 실행


### 4) `requirements.txt`
- **설명**: 프로젝트 실행에 필요한 파이썬 패키지 의존성 목록 파일.
- **동작/기능**:
  - `rich` 라이브러리 및 `ipython`, `ipykernel` 등 Jupyter 실행 관련 패키지 버전명 기록
- **사용 방법**:
  - 터미널에서 다음 명령어로 일괄 설치:
    ```bash
    pip install -r requirements.txt
    ```
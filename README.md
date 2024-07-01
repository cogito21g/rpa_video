# RPA Video with Python

이미지와 스크립트를 가지고 텍스트 파일과 영상 파일을 자동화하여 생성하는 프로그램입니다.


## 설치 방법

이 프로젝트를 로컬 환경에서 실행하려면, 다음 단계를 따라주세요

1. 이 저장소를 클론합니다.
   ```bash
   git clone https://github.com/cogito21g/rpa_video.git
   ```
2. 프로젝트 디렉토리로 이동합니다.
   ```bash
   cd rpa_video
   ```
3. 필요한 패키지를 설치합니다.
```
pip install moviepy              # moviepy 1.0.3
pip install gTTS                 # gTTS 2.5.1
pip install SpeechRecognition    # SpeechRecognition 3.10.4
pip install pydub                # pydub 0.25.1
pip install pillow               # pillow 10.4.0
```
4. `main.py` 파일 실행합니다.
   ```
   python main.py
   ```


## 사용 기술
- python 3.10


## 프로젝트 구조

```
project/
├── rpa_video/
│   │── __init__.py
│   │── change_format.py
│   │── create_video.py
│   │── speech_to_text.py
│   └──text_to_speech.py
├── main.py
├── .gitignore
├── README.md
└── LICENSE
```

- rpa_video/: 
   - chage_format.py: 
   - create_video.py: 
   - speech_to_text.py: 
   - text_to_speech.py: 
- main.py: 프로그램을 실행하는 entrypoint입니다.
- README.md: 프로젝트에 대한 설명과 설치 방법을 설명합니다.


## 규칙

#### 코딩 컨벤션

1. **파일 및 디렉토리 구조**
   - 파일명은 소문자와 하이픈(-)을 사용합니다. 예: `index.html`, `style.css`, `script.js`
   - 디렉토리명은 소문자와 하이픈(-)을 사용합니다.

2. **주석**
   - 한줄 주석은 #을 사용합니다.
   - 여러줄 주석은 """ ~ """을 사용합니다.
   - docstring은 """ ~ """을 사용합니다.

3. **python**
   - 들여쓰기는 4칸을 사용합니다.
   - 변수명과 함수명은 소문자와 밑줄(_)을 사용합니다.
   - 클래스는 CamelCase를 사용합니다.
   - 클래스와 최상위함수는 두줄을 띄웁니다.
   - 클래스내의 메서드는 한줄을 띄웁니다.
   - 모듈과 패키지는 내장모듈, 서드파티, 사용자정의 모듈 순서로 작성합니다.
   - docstring 작성시 설명과 인자, 반환값, 사용예시를 작성합니다.


#### git commit message 규칙

1. **커밋 메시지 구조**
- 제목: 50자 이내로 간결하게 작성
- 본문: 선택 사항, 변경 사항에 대한 자세한 설명
- 꼬리말: 이슈 트래킹 번호 (선택 사항)

2. **타입**
- `feat`: 새로운 기능 추가
- `fix`: 버그 수정
- `docs`: 문서 수정
- `style`: 코드 포맷팅, 세미콜론 누락 등 코드 변경이 없는 경우
- `refactor`: 코드 리팩토링 (기능 변경 없이 코드 구조 개선)
- `test`: 테스트 추가, 테스트 리팩토링
- `chore`: 빌드 업무, 패키지 매니저 설정 등

3. **예시**

```
feat: Create Video

- create audio using scripts
- create video using images and audio_file

Resolves: #123
```


#### 규칙 설정
- 모든 기능 추가는 새로운 브랜치에서 작업합니다.
- 커밋 메시지는 명확하고 간결하게 작성합니다.
- 주요 변경 사항마다 PR(pull request)를 생성하고, 코드 리뷰를 받습니다.


## 기여 방법

1. 이 저장소를 포크합니다.
2. 새로운 브랜치를 생성합니다.
   ```bash
   git checkout -b feature/새로운기능
   ```
3. 변경 사항을 커밋합니다.
   ```bash
   git commit -m 'Add 새로운 기능'
   ```
4. 브랜치에 푸시합니다.
   ```bash
   git push origin feature/새로운기능
   ```
5. 풀 리퀘스트를 생성합니다.


## 라이센스

이 프로젝트는 MIT 라이센스를 따릅니다. 자세한 내용은 `[LICENSE](./LICENSE)` 파일을 참고하세요.

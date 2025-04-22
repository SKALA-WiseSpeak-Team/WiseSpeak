# 🎓 WiseSpeak
## 📚 프로젝트 소개
### RAG 기술 기반 글로벌 지능형 학습 시스템

✔️ PDF 문서에서 정보를 추출하여 각 페이지 별로 오디오 강의 생성

✔️ 실시간 질문이 가능한 챗봇 기능을 통합한 인터랙티브 학습 플랫폼

---

## Service Target
![서비스타깃](https://github.com/user-attachments/assets/9d49d004-4f41-4697-8e29-ca753e84e9bd)

---

## 사용자 기능 흐름도
![사용자기능흐름도](https://github.com/user-attachments/assets/f0ac5d46-469a-420c-800d-2c424a32e403)

---

## 프로젝트 아키텍처
![프로젝트 아키텍처](https://github.com/user-attachments/assets/7420eead-e4d5-4d32-9f22-3442ad95ead2)

---

## 데이터 흐름도
![데이터 흐름도](https://github.com/user-attachments/assets/1e9e422c-4211-4bb4-9a6f-767723589892)

## 🚀 실행 매뉴얼
### 1. Repository Clone
```bash
git clone https://github.com/SKALA-WiseSpeak-Team/WiseSpeak.git
```

### 2. Submodule 최신화
```bash
git submodule update --init --recursive
```

### 3. Backend 서버 실행

#### 디렉토리 이동
레포지토리 root 디렉토리 기준
```bash
cd WiseSpeak-AI
```

#### 환경 설정
```bash
# 가상환경 생성 및 활성화
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

# 패키지 설치
pip install -r requirements.txt
```

#### API 키 설정 방법
##### `.env` 파일 사용 
프로젝트 app 디렉토리에 `.env.example` 파일을 참고하여 .env로 생성하고 API 키를 저장하세요.

#### 실행 방법
```bash
# 백엔드 서버 실행
python run.py
```

서버가 시작되면 `http://localhost:8000`에서 접속할 수 있습니다.
API 문서는 `http://localhost:8000/docs`에서 확인할 수 있습니다.

### 4. Frontend 서버 실행

#### 디렉토리 이동
레포지토리 root 디렉토리 기준
```bash
cd WiseSpeak-Vue
```

#### 필수 조건
- Node.js 16.x 이상
- npm 8.x 이상 또는 yarn 1.22.x 이상

#### env 설정
```
# /client/.env
VITE_API_BASE_URL="your server API URL"

# /server/.env
# TTS모델 사용을 위한 API key
OPENAI_API_KEY = "your OpenAI API Key"
```

#### 환경 설치
```bash
# 의존성 설치
npm install
# 또는
yarn install

# 클라이언트 디렉토리로 이동하여 의존성 설치
cd client
npm install
# 또는
yarn install

# server 디렉토리로 이동하여 의존성 설치
cd ../server
npm install
# 또는
yarn install
```

#### 실행 방법
```bash
# 개발 서버 실행
npm run dev
# 또는
yarn dev
```

# 인공지능 시인 🎭

OpenAI GPT-4o-mini를 활용한 한국어 시 생성 웹 애플리케이션입니다.

## 📝 프로젝트 소개

사용자가 입력한 주제를 바탕으로 AI가 아름다운 한국어 시를 자동으로 작성해주는 Streamlit 기반 웹 애플리케이션입니다.

## ✨ 주요 기능

- 🔑 OpenAI API 키 입력 및 관리
- 📖 주제 기반 시 자동 생성
- 🎨 직관적인 웹 인터페이스
- ⚡ 실시간 시 생성 및 표시

## 🛠️ 기술 스택

- **Python 3.x**
- **Streamlit** - 웹 인터페이스
- **LangChain** - LLM 체인 관리
- **OpenAI GPT-4o-mini** - 시 생성 모델

## 📦 설치 방법

### 1. 저장소 클론 (또는 파일 다운로드)

```bash
git clone <repository-url>
cd <project-directory>
```

### 2. 가상환경 생성 (권장)

```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### 3. 필요한 패키지 설치

```bash
pip install -r requirements.txt
```

추가로 Streamlit이 requirements.txt에 없다면 설치:

```bash
pip install streamlit
```

## 🚀 실행 방법

```bash
streamlit run app.py
```

브라우저가 자동으로 열리며 `http://localhost:8501`에서 애플리케이션에 접근할 수 있습니다.

## 📖 사용 방법

1. **API 키 입력**
   - 사이드바에서 OpenAI API 키를 입력합니다
   - API 키는 [OpenAI Platform](https://platform.openai.com/api-keys)에서 발급받을 수 있습니다

2. **주제 입력**
   - 메인 화면에서 시의 주제를 입력합니다
   - 예: "봄날의 햇살", "그리운 사람", "바다" 등

3. **시 생성**
   - "시 작성 요청하기" 버튼을 클릭합니다
   - AI가 입력한 주제를 바탕으로 시를 생성합니다

## 📋 주요 의존성

- `langchain==1.0.5` - LLM 체인 구성
- `langchain-openai==1.0.2` - OpenAI 통합
- `openai==2.7.2` - OpenAI API 클라이언트
- `streamlit` - 웹 인터페이스

전체 의존성은 `requirements.txt` 파일을 참조하세요.

## ⚙️ 구성 요소

### app.py

메인 애플리케이션 파일로 다음 기능을 포함합니다:

- Streamlit UI 구성
- OpenAI API 키 관리
- LangChain 체인 생성 및 실행
- 시 생성 및 결과 표시
- 에러 핸들링

## ⚠️ 주의사항

- OpenAI API 키가 필요합니다 (유료 서비스)
- API 사용량에 따라 비용이 발생할 수 있습니다
- 안정적인 인터넷 연결이 필요합니다

## 🔒 보안

- API 키는 세션에만 저장되며 파일로 저장되지 않습니다
- API 키 입력 필드는 `type="password"`로 설정되어 있습니다
- 민감한 정보를 Git에 커밋하지 마세요

## 🐛 문제 해결

### API 키 오류
- OpenAI API 키가 올바른지 확인하세요
- API 키가 `sk-`로 시작하는지 확인하세요
- OpenAI 계정에 충분한 크레딧이 있는지 확인하세요

### 패키지 설치 오류
```bash
pip install --upgrade pip
pip install -r requirements.txt --force-reinstall
```

## 📄 라이선스

이 프로젝트의 라이선스는 프로젝트 소유자가 지정합니다.

## 🤝 기여

버그 리포트, 기능 제안, 풀 리퀘스트를 환영합니다!

---

**Made with ❤️ using Streamlit and OpenAI**
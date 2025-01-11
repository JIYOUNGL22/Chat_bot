## 핵심 기능:

1. 데이터 수집 및 크롤링
2. 수집된 데이터의 전처리
3. LangChain을 활용한 데이터 연결
4. RAG(문서 검색 및 생성) 추가
5. GPT API 기반 LLM 활용
6. Gradio를 통한 사용자 인터페이스 구축

**대상 사용자:**
데이터 분석 전문가, IT 기업 채용 담당자

---

### 프로젝트 단계

### 1. 데이터 수집(크롤링)

- **목표:** 특정 주제에 대한 데이터를 인터넷에서 자동으로 수집
- **세부 계획:**
    - 주제 정의: 챗봇의 목적에 맞는 데이터(예: 고객 FAQ, 기술 문서 등).
    - 크롤링 도구: Make를 활용하여 데이터 수집 자동화.
    - 저장 방식: 수집 데이터를 CSV, JSON 등 구조화된 형태로 저장.

### 2. 데이터 전처리(평문처리)

- **목표:** 수집된 데이터를 분석과 모델 학습에 적합한 형태로 변환.
- **세부 계획:**
    - 텍스트 정규화: 불필요한 기호 제거, 대소문자 변환.
    - 토큰화 및 중복 제거: 텍스트 데이터 정리.
    - 언어 및 주제 분류: 주요 키워드 기반 클러스터링.
    - 데이터 검증: 품질 평가 및 불완전 데이터 삭제.

### 3. LangChain 사용

- **목표:** 수집 및 정리된 데이터를 LLM과 효과적으로 연결.
- **세부 계획:**
    - LangChain 환경 설정.
    - 메모리 모듈 구현: 데이터 세션 관리.
    - 커스터마이징: API 호출, 문맥 제공 로직 설계.

### 4. RAG(문서 검색 및 생성) 추가

- **목표:** 검색 기반의 문서 생성 기능으로 챗봇 성능 향상.
- **세부 계획:**
    - RAG 구현: OpenAI와 호환되는 오픈소스 도구 탐색 및 적용.
    - 데이터베이스 연결: FAQ, 문서 등과 통합.
    - 검색 및 생성 로직 최적화: 사용자 입력에 맞는 고품질 응답 제공.

### 5. LLM 활용(GPT API)

- **목표:** LLM을 활용해 챗봇의 자연어 이해와 생성 능력 강화.
- **세부 계획:**
    - OpenAI API 활용 준비: 인증키 생성, 호출 로직 작성.
    - 프롬프트 엔지니어링: 적절한 질문 생성 및 응답 최적화.
    - 성능 평가: 응답 품질, 속도 및 정확성 테스트.

### 6. Gradio 챗봇 구축

- **목표:** 사용자 친화적인 웹 기반 인터페이스 제공.
- **세부 계획:**
    - Gradio 설치 및 설정.
    - 입력/출력 레이아웃 디자인: 간단하고 직관적인 UI.
    - 백엔드 연결: GPT API, LangChain 및 RAG 연동.
    - 배포: 챗봇을 웹 호스팅 서비스에 배포.

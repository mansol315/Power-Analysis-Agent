# ⚡ 전력 분석 AI 에이전트 '라온 (Raon)'
**라온(Raon)** 은 거대언어모델(LLM)을 활용하여 국내 전력 수요 데이터(CSV) 분석과 전문적인 전력 정책 문서(PDF) 조회를 통합적으로 수행하는 지능형 분석 에이전트입니다. 

사용자의 질문 의도에 따라 스스로 판단하여 파이썬 코드를 실행하거나 관련 문서를 검색하여 최적의 답변을 제공합니다. 

## 🌟 주요 기능 (Key Features)
### 1. 지능형 라우터 (Intelligent Router)
사용자의 자연어 질문을 분석하여 **데이터 분석(Data)**이 필요한지, **문서 기반 설명(Document)**이 필요한지 스스로 판단하여 적절한 모듈로 연결합니다. 

### 2. 데이터 분석가 (Data Analyst)

Code Interpreter: 질문에 적합한 Python 코드를 실시간으로 생성하고 실행합니다. 

시각화: 전력 수요 추이, 기온과의 상관관계 등을 그래프(Matplotlib)로 즉시 시각화하여 제공합니다. 

수치 분석: 특정 날짜의 전력량 비교, 월간 최대 수요일 조회 등 정밀한 데이터 분석을 수행합니다. 


### 3. 문서 전문가 (Document Expert - RAG)

지식 베이스: '제11차 전력수급기본계획' 및 '전력 수요 분석 보고서' 등 전문 문서를 학습한 벡터 DB(Chroma)를 활용합니다. 


RAG 기술: 사용자의 질문과 가장 유사한 문서 내용을 검색하여, 근거 기반의 답변을 생성합니다. 


정적 지식 결합: 2019~2024년 EDA(탐색적 데이터 분석) 결과를 사전 지식으로 활용하여 답변의 정확도를 높였습니다. 

## 📁 프로젝트 구조 (Project Structure)

app.py: Streamlit 기반의 웹 대화형 인터페이스 

total.ipynb: 에이전트 핵심 로직 개발 및 테스트를 위한 Jupyter Notebook 

data/: 분석에 사용된 전력 수요 CSV 파일 및 정책 PDF 문서들 

.gitignore: 보안을 위해 API 키(.env) 및 로컬 DB 등을 제외하는 설정 

## 🛠️ 기술 스택 (Tech Stack)

언어: Python 


LLM: OpenAI GPT-4o, GPT-4o-mini 


프레임워크: LangChain, Streamlit 


데이터베이스: Chroma (Vector DB) 


라이브러리: Pandas, Matplotlib, python-dotenv

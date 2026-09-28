<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=auto&height=200&section=header&text=Hello,%20I'm%20Keunwoo!&fontSize=70&animation=fadeIn&fontAlignY=38&desc=AI%20Researcher%20&%20Data%20Analyst&descAlignY=55&descAlign=50" width="100%" />
</div>

<br>

## 🧑‍💻 About Me
**"데이터 속에서 의미를 찾아내는 연구자, 김근우입니다."**

원광대학교 차세대 정보처리 연구실(Next-Generation Information Processing Lab)에서 학부 연구생으로 활동하며, 자연어 처리(NLP)와 빅데이터 분석을 연구했습니다. 텍스트 데이터에서 가치를 추출하는 모델링과, 이를 실제 서비스로 연결하는 풀스택 구현에 흥미를 가지고 있습니다.

- 🎓 **Education:** 원광대학교 인공지능융합학과 & 콘텐츠미디어SW융합전공 (복수전공)
- 🔬 **Role:** Undergraduate Researcher @ Next-Gen Info Processing Lab
- 💡 **Interests:** NLP (NER, LLM), Full-stack Service Dev, Server Security
- 🌱 **Learning:** Information Processing Engineer(SQL, Encryption), 42 Seoul (Peer Learning)

<br>

## 🛠 Tech Stack

### 🧠 AI & Data Analytics
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white"/> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=PyTorch&logoColor=white"/> <img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=HuggingFace&logoColor=black"/> <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white"/> <img src="https://img.shields.io/badge/Scikit_Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white"/>

### 💻 Backend & Server
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=FastAPI&logoColor=white"/> <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white"/> <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white"/> <img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white"/> <img src="https://img.shields.io/badge/Apache_Cassandra-1287B1?style=flat-square&logo=apachecassandra&logoColor=white"/> <img src="https://img.shields.io/badge/Ubuntu-E95420?style=flat-square&logo=Ubuntu&logoColor=white"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=Docker&logoColor=white"/> <img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=Cloudflare&logoColor=white"/>

### 🎮 Content & Web
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=TypeScript&logoColor=white"/> <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=React&logoColor=black"/> <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=JavaScript&logoColor=black"/> <img src="https://img.shields.io/badge/Leaflet-199900?style=flat-square&logo=Leaflet&logoColor=white"/> <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=Streamlit&logoColor=white"/> <img src="https://img.shields.io/badge/Ren'Py-FF7F7F?style=flat-square&logo=Ren'Py&logoColor=white"/>

<br>

## 🚀 Key Projects

### 1. 💼 AI Job Agent (취준 워크스페이스)
> **Description:** 채용 공고(URL·이미지·PDF)를 개인 LLM 키로 파싱해 표로 정리하고, 자소서·서류함·JD 근거 챗까지 한곳에서 관리하는 스마트 구직 지원 웹 서비스  
> **Live:** [jobagent.cloud](https://jobagent.cloud)
- **Tech:** Next.js, React, TypeScript, Supabase (Auth/Postgres/Storage), BYOK LLM (OpenAI 호환·Anthropic·Google), PM2, Cloudflare Tunnel
- **Key Features:**
  - **공고 자동 추출:** HTML·통이미지 포스터·`data/*.js` JD까지 대응해 회사·직무·마감·자격·전형을 표로 저장
  - **BYOK 보안:** 분석·자소서·챗 비용은 사용자 키로만 청구. 키는 AES-256-GCM으로 서버에서만 복호화
  - **서류함 + 마크다운 편집기:** 자소서 버전 관리, 공고 맥락 기반 AI 초안, PDF/DOCX 텍스트 가져오기
  - **도구형 AI 챗:** 저장된 JD(`get_job`)만 근거로 상담·상태 변경. 없는 내용은 추정하지 않음
- [👉 **GitHub Repo**](https://github.com/KeunwooKim/AI_job_agent) · [🌐 **Demo**](https://jobagent.cloud)

### 2. 🗺️ New Disaster (도심 재난 위치 판별·알림 서비스)
> **Description:** 긴급재난문자·실종·기상특보·산사태 등 공공 발령을 수집하고, 지명을 행정구역·지오코딩 중심으로 판별해 지도에 표시하는 재난 알림 서비스
- **Tech:** Next.js, React, TypeScript, Leaflet, SQLite, Hugging Face Inference, Python (학습/전처리)
- **Key Features:**
  - **다중 공공 데이터 수집:** 행안부 긴급재난문자, 경찰청 안전Dream 실종, 기상청 특보·지진·태풍, 산림청 산사태 예측
  - **위치 판별 파이프라인:** 발신 기관 → 법정동 사전 → 도로명 지오코딩 → (부족 시) NER/LLM 보완. 오탐(동사 활용·교차로명 등) 규칙 필터
  - **유형 분류:** 키워드 우선순위로 호우·폭염·강풍·축산 방역 등을 부여하고, 오분류를 줄이는 예외 규칙 적용
  - **지도 UI:** 시·군 단위 특보는 행정구역 색칠, 지점 특정 건은 마커. 기간 조회 지원
- [👉 **GitHub Repo**](https://github.com/KeunwooKim/New_disaster)

### 3. 🚨 Disaster Service (재난 정보 수집 및 실시간 알림 시스템)
> **Description:** 공공 데이터 포털 및 재난 문자 데이터를 수집·가공하여 실시간 알림을 제공하는 백엔드 시스템
- **Tech:** Python, FastAPI, Cassandra, KoBERT(NER), FCM
- **Key Features:**
  - **NER 모델링:** 비정형 재난 문자에서 발생 위치 및 재난 유형 자동 추출 (KoBERT Fine-tuning)
  - **데이터 파이프라인:** 기상청/행안부 데이터 크롤링 및 실시간 DB 적재
  - **API & Push:** FastAPI 기반 서버 구축 및 FCM을 통한 모바일 앱 푸시 알림 전송
- [👉 **GitHub Repo Link**](https://github.com/KeunwooKim/Disaster_service)

### 4. 🐾 Seoul Pet Infrastructure Dashboard (서울시 반려동물 인프라 분석)
> **Description:** 서울시 반려동물 등록 현황과 관련 인프라(병원, 편의시설)의 불균형을 분석하는 인터랙티브 대시보드
- **Tech:** Python, Streamlit, Pydeck, Plotly, Pandas
- **Key Features:**
  - **3D 시각화:** Pydeck을 활용한 자치구별 인구/반려동물 밀도 3D 지도 구현
  - **데이터 분석 (EDA):** 등록 수 대비 인프라 부족 지역 산출 및 불균형 지표 시각화
  - **시설 탐색:** 사용자 위치 기반 반려동물 동반 가능 시설 검색 기능 제공
- [👉 **GitHub Repo Link**](https://github.com/KeunwooKim/Pets_infra)

<br>

## 📈 GitHub Stats
<div align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=KeunwooKim&layout=compact&theme=radical" height="150px" alt="Top Langs"/>
</div>

<br>

## 📫 Contact
- **Email:** andy_0613@naver.com

<br>
<img src="https://capsule-render.vercel.app/api?type=waving&color=BDBDC8&height=100&section=footer" />

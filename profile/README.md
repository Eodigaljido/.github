### 어디갈지도 - 이동 계획 도우미

<div align="center">
  <h1> 어디갈지도 - 이동 계획 도우미</h1>
  <p>🔍 장소 기록부터 약속 동선 계획까지 한 번에 해결하는 스마트 지도 서비스 🔍</p>
</div>

<br/>

<div align="center">
  <img src="./assets/EodigaljidoIcon.png" alt="EodigaljidoIcon" style="border-radius: 10px; width: 200px;" />
</div>

<br/>

<div align="center">
  <a href="https://example.co.kr/">홈페이지</a>
  &nbsp; | &nbsp;
  <a href="http://localhost:8080/swagger-ui/index.html">Swagger</a>
  &nbsp; | &nbsp;
  <a href="https://season-poison-a39.notion.site/Project-1134ef984a1880afa035f50350278481?pvs=4">Notion</a>
</div>

---

## ✍️ 프로젝트 개요
- **프로젝트명:** 어디갈지도
- **프로젝트 기간:** 2026.3 ~
- **프로젝트 형태:** 교내 캡스톤 프로젝트
- **목표:** 메신저/지도/채팅이 뒤섞인 불편한 여행 계획 경험을 하나의 앱으로 통합하여 그룹 여행 계획의 편의성 증대
- **주요 타겟 사용자:** 20 ~ 30세+ / 친구, 연인, 소모임 단위 여행자 (3~8명 내외 그룹)

---

## ✍️ 프로젝트 소개

### 프로젝트 배경

친구들과 여행을 계획할 때 기존 프로세스는 다음과 같은 문제점이 있었습니다:

1. **분산된 도구 사용으로 인한 불편함:**
   - 카카오톡, 디스코드 등 메신저로 의견을 조율하면서, 동시에 지도를 별도로 열어 경로를 공유해야 함.
   - 채팅과 지도가 분리되어 있어 대화 중 언급된 장소를 지도에 반영하는 과정이 번거롭고 누락이 잦음.

2. **실시간 공동 편집의 부재:**
   - 여행 경로를 한 사람이 단독으로 작성한 뒤 공유하는 방식으로, 여러 명이 동시에 의견을 반영하기 어려움.
   - 경로 수정 시 변경 사항을 다시 공유해야 하는 반복 작업 발생.

3. **여행 중 위치 파악의 어려움:**
   - 그룹 이동 시 일행의 현재 위치를 실시간으로 확인할 수 있는 통합 수단이 없음.
   - 별도의 위치 공유 앱을 추가로 사용해야 하는 불편함.

**어디갈지도**는 위 문제를 해결하기 위해 지도 기반 실시간 멀티 편집, 채팅·지도 양방향 연동, 실시간 위치 공유를 하나의 앱에서 제공하는 그룹 여행 루트 플래너입니다.

---

### 문제점 해결

- **여행 계획 통합:** 메신저와 지도를 오가는 번거로움을 없애고, 채팅과 지도 편집을 한 화면에서 동시에 처리.
- **실시간 공동 편집:** 그룹 내 누구나 동시에 경로를 추가·수정할 수 있으며, 변경 이력과 편집 중인 사용자를 실시간으로 시각화.
- **맞춤 루트 추천:** 온보딩 성향 설문을 기반으로 사용자 취향에 맞는 샘플 루트를 즉시 제안하여 계획 시작의 진입 장벽 완화.

---

## 🚀 프로젝트 목표

1. **여행 계획 편의성 향상:**
   - 분산된 메신저와 지도 서비스를 하나의 앱으로 통합하여 그룹 여행 계획에 소요되는 시간과 혼선 최소화.
   - 실시간 멀티 편집으로 모든 구성원이 동등하게 여행 계획에 참여 가능.

2. **사용자 경험 강화:**
   - 지도/리스트/채팅이 한 화면에 통합된 직관적인 인터페이스 제공.
   - 성향 설문 기반 추천 루트로 처음 사용자도 빠르게 여행 계획을 시작할 수 있도록 지원.
<!-- ---
---

## 📌 주요 기능

### **0. 회원가입 | 로그인**

#### **회원가입**

- 이메일 | 이름 | 사번 | 부서 | 비밀번호

<div align="center">
<img src="./assets/회원가입.gif" alt="회원가입" style="border-radius: 10px; width: 700px;"/>
</div>

#### **로그인**

- 이메일 | 비밀번호
- 로그인시 다음과 같이 이동
    - 일반 사용자 ⇒ 채팅 페이지
    - 관리자 ⇒ 관리자 페이지

<div align="center">
<img src="./assets/로그인.gif" alt="로그인" style="border-radius: 10px; width: 700px;"/>
</div>

### **1. 자연어 이해를 통한 질문 응답**

- **기능 설명:** 사용자가 자연어로 질문을 입력하면, LLM이 질문의 문맥과 의미를 분석하여 적합한 답변을 제공합니다.

- 채팅 화면은 아래와 같습니다. 

<div align="center">
<img src="./assets/채팅1.png" alt="채팅1" style="border-radius: 10px; width: 700px;"/>
</div>

- 실제 채팅이 진행되는 화면입니다.


<div align="center">
<img src="./assets/채팅1.gif" alt="채팅1" style="border-radius: 10px; width: 700px;"/>
</div>


- **기술 요소:**
    - **RAG(Retrieval-Augmented Generation):** 유사도 기반 검색을 통해 관련 규정 데이터를 추출한 후, 답변에 포함.
    - **LLM 모델:** 한국어 성능에 최적화된 Llama-VARCO-8B 모델 사용.


---

### **2. 규정 업데이트 자동화**

- **기능 설명:** 관리자 페이지를 통해 신규 규정 작성 및 기존 규정 수정 시, 벡터 데이터베이스(Faiss)가 자동으로 갱신됩니다.

- **주요 과정:**
    1. 관리자가 규정을 입력하거나 수정. (파일 혹은 직접 입력을 통한 업로드)
    2. 변경 사항이 JSON 포맷으로 변환.
    3. 벡터 데이터베이스(Faiss)를 재구성하여 최신 데이터 반영.
        

- 코로나와 관련된 내용입니다. 

<div align="center">
<img src="./assets/코로나등록1.gif" alt="코로나등록1" style="border-radius: 10px; width: 700px;"/>
</div>

- 육아 휴직과 관련된 내용입니다.

<div align="center">
<img src="./assets/육아휴직.gif" alt="육아휴직" style="border-radius: 10px; width: 700px;"/>
</div>

---

### **3. 사용자 레벨 기반 정보 접근 제어**

- **기능 설명:** 직원의 레벨(1,2,3)에 따라 정보 접근 권한을 제한합니다. 정보의 레벨 이하인 직원만 해당 정보에 접근할 수 있습니다.
- **예시:**
    - 레벨 1의 직원은 답변 레벨 1이하인 규정만 접근 및 답변 형성 가능
    - 레벨 2의 직원은 답변 레벨 1, 2인 정보만 접근 및 답변 형성 가능
    - 직원의 레벨보다 높은 정보에 대해 질문할 경우,

<div align="center">
<img src="./assets/사용자레벨.PNG" alt="User Level" style="border-radius: 10px; width: 700px;"/>
</div>

---

### **4. 피드백 기능**

- **기능 설명:** 사용자가 응답 품질에 대해 긍정/부정 피드백을 남길 수 있으며, 이를 통해 챗봇 학습 데이터 개선에 활용할 수 있습니다.
- **주요 기능:**
    - 응답 정확성 평가.
    - 추가 학습 데이터로 활용 가능.


### 5. 관리자 기능

- **기능 설명**:

#### 회원 정보 변경

<div align="center">
<img src="./assets/회원관리.png" alt="회원관리" style="border-radius: 10px; width: 700px;"/>
</div>

- 관리자는 회원 관리 페이지에 접속할 수 있습니다. 

<div align="center">
<img src="./assets/회원관리모달.PNG" alt="회원관리모달" style="border-radius: 10px; width: 700px;"/>
</div>
- 변경 버튼을 누르면 변경 모달 창을 확인할 수 있습니다.
- 회원의 답변 레벨을 변경할 수 있습니다.
    - 답변 레벨 1 ~ 3
- 회원의 권한을 변경할 수 있습니다.
    - USER: 일반 회원
    - USER_WRITE: 규정 작성이 가능한 회원
    - ADMIN: 관리자 회원

#### 피드백 관리

<div align="center">
<img src="./assets/피드백관리.PNG" alt="피드백관리" style="border-radius: 10px; width: 700px;"/>
</div>


- 회원이 작성한 sembot 답변 피드백을 확인할 수 있습니다.


#### 카테고리 관리

<div align="center">
<img src="./assets/카테고리관리.png" alt="카테고리관리" style="border-radius: 10px; width: 700px;"/>
</div>

- 규정 카테고리를 추가, 삭제할 수 있습니다.

---

## 🧑‍💻 팀원 소개

| **이름**    | **역할**        | 
|:-----------:|:---------------:|
| 변지환      | 팀장 & FE/BE    | 
| 김광현      | FE/BE           |
| 김상혁      | AI              | 
| 김준호      | AI              | 
| 이서빈      | BE/FE           | 
| 한수한      | FE/AI/Infra        | 

---

## ⚙️ 기술 스택

<table>
  <thead>
    <tr>
      <th>분류</th>
      <th>기술 스택</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>프론트엔드</td>
      <td>
        <img src="https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=white"/>
        <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white"/>
        <img src="https://img.shields.io/badge/TailwindCSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white"/>
        <img src="https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white"/>
      </td>
    </tr>
    <tr>
      <td>백엔드</td>
      <td>
        <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=spring-boot&logoColor=white"/>
        <img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white"/>
        <img src="https://img.shields.io/badge/Java-007396?style=flat&logo=openjdk&logoColor=white"/>
        <img src="https://img.shields.io/badge/Gradle-02303A?style=flat&logo=gradle&logoColor=white"/>
      </td>
    </tr>
    <tr>
      <td>데이터베이스</td>
      <td>
        <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white"/>
        <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white"/>
        <img src="https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white"/>
      </td>
    </tr>
    <tr>
      <td>인프라</td>
      <td>
        <img src="https://img.shields.io/badge/AWS_EC2-FF9900?style=flat&logo=amazon-ec2&logoColor=white"/>
        <img src="https://img.shields.io/badge/Ubuntu-20.04-E95420?style=flat&logo=ubuntu&logoColor=white"/>
        <img src="https://img.shields.io/badge/Nginx-1.18.0-009639?style=flat&logo=nginx&logoColor=white"/>
        <img src="https://img.shields.io/badge/Tomcat-F8DC75?style=flat&logo=apache-tomcat&logoColor=black"/>
      </td>
    </tr>
  </tbody>
</table>


---

## 📂 문서 자료

- [포팅 메뉴얼](https://github.com/SSAFY-Sembot/Sembot/blob/develop/exec/%ED%8F%AC%ED%8C%85%EB%A7%A4%EB%89%B4%EC%96%BC.md)
- [사용자 가이드](https://github.com/SSAFY-Sembot/Sembot/blob/develop/exec/%EC%82%AC%EC%9A%A9%EC%9E%90_%EA%B0%80%EC%9D%B4%EB%93%9C.pdf)
- [발표 자료](https://github.com/SSAFY-Sembot/Sembot/blob/develop/exec/%EC%B5%9C%EC%A2%85_%EB%B0%9C%ED%91%9C%EC%9E%90%EB%A3%8C.pdf)

--- -->

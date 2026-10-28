<div align="center">

# 다시, 시흥 (Dasi Siheung)
### "시흥의 유휴 공간에 새로운 숨결을 불어넣다"
**도심 속 비어있는 상가와 창작자·소상공인을 잇는 단기 공간 공유 및 로컬 활성화 플랫폼**

<br/>

[![Team](https://img.shields.io/badge/Team-김예지와%20아이들-FF6B6B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/TUK-Mobile-Programming-1-2)
[![Android](https://img.shields.io/badge/Android-Jetpack%20Compose-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://github.com/TUK-Mobile-Programming-1-2/dasi-siheung-android)
[![Backend](https://img.shields.io/badge/Backend-Spring%20Boot%203.5-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)](https://github.com/TUK-Mobile-Programming-1-2/dasi-siheung-backend)
[![GIS](https://img.shields.io/badge/GIS-PostGIS%20Spatial-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)](https://github.com/TUK-Mobile-Programming-1-2/dasi-siheung-backend)
[![Web](https://img.shields.io/badge/Admin%20Web-React%2019%20%7C%20TS-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://github.com/TUK-Mobile-Programming-1-2/dasi-siheung-web)
[![Design](https://img.shields.io/badge/Design-Figma%20System-F24E1E?style=for-the-badge&logo=figma&logoColor=white)](https://github.com/TUK-Mobile-Programming-1-2/dasi-siheung-docs)
[![QA](https://img.shields.io/badge/QA-Quality%20Assurance-0A84FF?style=for-the-badge&logo=checkmarx&logoColor=white)](https://github.com/TUK-Mobile-Programming-1-2/dasi-siheung-docs)

<br/>

</div>

---

## 배경 및 프로젝트 비전

> **"비어있는 상가는 늘어나지만, 청년 창업가와 예술가들은 오프라인 공간을 찾지 못하고 있습니다."**

원도심과 신도시 상권의 장기 공실 문제는 지역 상권 침체로 이어지고 있으며, 반대로 청년 창작자·소상공인은 높은 임대료와 장기 계약의 문턱에 가로막혀 오프라인 실험을 망설이고 있습니다.

**'다시, 시흥'**은 이러한 사회적 단절을 해소하기 위해 탄생한 **시흥형 유휴 공간 재생 & 단기 대여 플랫폼**입니다. 방치된 공실 상가를 팝업스토어, 단기 전시, 플리마켓, 원데이 클래스, 커뮤니티 모임 등 다채로운 로컬 활동의 장으로 전환하여, 공간 호스트에게는 유휴 자산의 가치 재창출을, 창작자에게는 합리적이고 유연한 도전의 기회를 제공합니다.

<br/>

### 4대 핵심 가치 및 솔루션

1. **정밀 GIS 기반 유휴 상가 탐색 (Spatial Discovery)**  
   - PostGIS 기반 공간 데이터 엔진을 적용하여 시흥 관내 유휴 상가의 위치, 수용 인원, 비품 현황, 대여 가능 기간을 지도 위에서 실시간으로 정밀 탐색합니다.
2. **원스톱 단기 대여 및 투명한 조건 조율 (Agile Booking)**  
   - 복잡한 임대차 계약서 대신 모바일 기반의 간편 신청서를 통해 사용 목적과 희망 일정을 전달하고, 호스트와 게스트 간 1:1 대화로 조건을 신속히 협의합니다.
3. **2단계 신뢰 검수 시스템 (Two-Tier Trust Engine)**  
   - **1차 관리자 검수(Admin Web)**: 사업자등록증 및 부동산 권한 증빙 서류를 검증하여 허위 매물 원천 차단  
   - **2차 호스트 승인**: 공간 소유자가 실제 이용 목적과 일정을 확인 후 최종 승인하며, 겹치는 날짜의 동시 점유를 시스템적으로 방어
4. **로컬 창작자 네트워킹 '동네생활' (Creator Community)**  
   - 시흥 청년 예술가와 소상공인이 모여 공동 팝업 팀을 모집하고, 집기·비품을 품앗이하며 지역 문화를 꽃피우는 소통 생태계를 구축합니다.

<br/>

### 서비스 흐름도 (Workflow Architecture)

```
 ┌────────────────┐          공간 등록 & 권한 서류 제출          ┌───────────────────────────┐
 │  공간 제공자   │ ─────────────────────────────────────────► │        관리자 웹          │
 │  (Host/Owner)  │ ◄───────────────────────────────────────── │     (Admin Console)       │
 └───────┬────────┘           1차 자격 검수 완료 & 승인         └───────────────────────────┘
         │                                                                    ▲
         │ 2차 신청서 검토                                                    │
         │ 및 최종 점유 확정                                                  │ 권한/공간 무결성
         ▼                                                                    │ 실시간 모니터링
 ┌────────────────┐                 단기 대여 신청 & 조건 조율                │
 │  창작자·이용자 │ ──────────────────────────────────────────────────────────┘
 │ (Guest/Creator)│
 └────────────────┘
```

---

## Members

<div align="center">

| <img src="https://github.com/sonyudam91-droid.png" width="90" height="90" alt="손유담"/><br/>**손유담** | <img src="https://github.com/dldnwls07.png" width="90" height="90" alt="이우진"/><br/>**이우진** | <img src="https://github.com/identicons/yeji.png" width="90" height="90" alt="김예지"/><br/>**김예지** | <img src="https://github.com/Jongwoo0101.png" width="90" height="90" alt="원종우"/><br/>**원종우** | <img src="https://github.com/identicons/wonhee.png" width="90" height="90" alt="윤원희"/><br/>**윤원희** |
| :---: | :---: | :---: | :---: | :---: |
| **UI/UX Designer** | **Frontend Lead (App & Web)** | **Team Leader / Android** | **Backend & Cloud Lead** | **QA Engineer** |
| [@sonyudam91-droid](https://github.com/sonyudam91-droid) | [@dldnwls07](https://github.com/dldnwls07) | [@YejiKim](https://github.com) | [@Jongwoo0101](https://github.com/Jongwoo0101) | [yoh40401@gmail.com](mailto:yoh40401@gmail.com) |
| Figma 디자인 시스템 & 화면 설계 | `:core-ui`, 제공자 & 어드민 웹 | 이용자 탐색/신청 & 공통 셸 | PostGIS 공간 도메인 & CI/CD | 시나리오 인수 검증 & 품질 보증 |

</div>

<br/>

> **팀 김예지와 아이들**은 기획·디자인부터 클라이언트, 백엔드, 품질 검증까지 하나의 유기적인 파이프라인으로 협업하는 5인 팀입니다.  
> 
> - **손유담 (UI/UX Designer)**: Figma 기반으로 직관적인 사용자 화면 플로우와 일관된 디자인 시스템 전반을 설계했습니다.  
> - **이우진 (Frontend Lead)**: 모바일 공통 디자인 시스템(`:core-ui`), 제공자 플로우, 관리자 웹 콘솔을 구축하고 프론트엔드 TDD를 총괄합니다.  
> - **김예지 (Team Leader & Android)**: 창작자 중심의 핵심 탐색·신청 여정과 공통 바텀 네비게이션 셸을 구현하며 프로젝트 전반을 이끕니다.  
> - **원종우 (Backend Lead)**: PostGIS 기반 공간 데이터 엔진, 무상태 보안 체계 및 CI/CD 자동화로 견고한 백엔드 시스템을 책임집니다.  
> - **윤원희 (QA Engineer)**: 사용자 시나리오 기반 인수 테스트와 기능 검증을 전담하여 프로덕트의 완성도와 품질을 보증합니다.

---

## Repositories & Tech Architecture

| Repository | Description | Key Tech Stack |
| :--- | :--- | :--- |
| [**dasi-siheung-android**](https://github.com/TUK-Mobile-Programming-1-2/dasi-siheung-android) | 공통·이용자·제공자 멀티모듈 Android 앱 | Kotlin, Compose, Material 3, Hilt, Coroutines, Flow |
| [**dasi-siheung-backend**](https://github.com/TUK-Mobile-Programming-1-2/dasi-siheung-backend) | PostGIS 공간 도메인 & 보안 RESTful API | Java 21, Spring Boot 3.5, PostGIS, JPA, Spring Security |
| [**dasi-siheung-web**](https://github.com/TUK-Mobile-Programming-1-2/dasi-siheung-web) | 공간 검수, 호스트 승인 및 플랫폼 운영 관리자 콘솔 | React 19, TypeScript, Vite, TailwindCSS, Vitest |
| [**dasi-siheung-infra**](https://github.com/TUK-Mobile-Programming-1-2/dasi-siheung-infra) | 무중단 배포, 컨테이너 환경 및 CI/CD 파이프라인 | Docker, GitHub Actions, CloudType |
| [**dasi-siheung-docs**](https://github.com/TUK-Mobile-Programming-1-2/dasi-siheung-docs) | 기획 정본, API 스펙, Figma 디자인 시스템 및 QA 가이드 | Markdown, Figma, Notion |

---

## Tech Stack

<div align="center">

### Design & QA
[![Figma](https://img.shields.io/badge/Figma-Design%20System-F24E1E?style=flat-square&logo=figma&logoColor=white)](https://www.figma.com/)
[![QA](https://img.shields.io/badge/QA-Scenario%20Testing-0A84FF?style=flat-square&logo=checkmarx&logoColor=white)](https://github.com/TUK-Mobile-Programming-1-2/dasi-siheung-docs)
[![Notion](https://img.shields.io/badge/Notion-Product%20Docs-000000?style=flat-square&logo=notion&logoColor=white)](https://www.notion.so/)

### Client & App
[![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)](https://kotlinlang.org/)
[![Android Studio](https://img.shields.io/badge/Android%20Studio-3DDC84?style=flat-square&logo=androidstudio&logoColor=white)](https://developer.android.com/studio)
[![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white)](https://developer.android.com/jetpack/compose)
[![Material 3](https://img.shields.io/badge/Material%20Design%203-757575?style=flat-square&logo=materialdesign&logoColor=white)](https://m3.material.io/)
[![Hilt](https://img.shields.io/badge/Hilt-Google-brightgreen?style=flat-square)](https://developer.android.com/training/dependency-injection/hilt-android)
[![Coroutines](https://img.shields.io/badge/Kotlin-Coroutines%20%26%20Flow-7F52FF?style=flat-square)](https://kotlinlang.org/docs/coroutines-overview.html)

### Backend & DB
[![Java 21](https://img.shields.io/badge/Java%2021%20LTS-ED8B00?style=flat-square&logo=openjdk&logoColor=white)](https://openjdk.org/)
[![Spring Boot 3.5](https://img.shields.io/badge/Spring%20Boot%203.5-6DB33F?style=flat-square&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![PostGIS](https://img.shields.io/badge/Spatial%20DB-PostGIS-4169E1?style=flat-square&logo=postgresql&logoColor=white)](https://postgis.net/)
[![Spring Security](https://img.shields.io/badge/Spring%20Security-Stateless-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)](https://spring.io/projects/spring-security)
[![Swagger](https://img.shields.io/badge/API%20Docs-OpenAPI3%20%26%20REST%20Docs-85EA2D?style=flat-square&logo=swagger&logoColor=black)](https://swagger.io/)

### Web & Admin
[![React 19](https://img.shields.io/badge/React%2019-61DAFB?style=flat-square&logo=react&logoColor=black)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev/)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Vitest](https://img.shields.io/badge/Vitest-Unit%20%26%20Integration-FCC72B?style=flat-square&logo=vitest&logoColor=black)](https://vitest.dev/)

### DevOps & CI/CD
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com/)
[![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-CI%2FCD-2088FF?style=flat-square&logo=githubactions&logoColor=white)](https://github.com/features/actions)
[![CloudType](https://img.shields.io/badge/Cloud-CloudType-0052CC?style=flat-square)](https://cloudtype.io/)

</div>

---

<div align="center">

<sub>Copyright © 2026 <b>팀 김예지와 아이들 (TUK-Mobile-Programming-1-2)</b>. All rights reserved.</sub>

</div>

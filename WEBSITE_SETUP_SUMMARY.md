# 웹사이트 완성 요약

## 완료된 작업

귀하의 CV와 SOP를 바탕으로 개인 학술 웹사이트를 완성했습니다.

### 1. 기본 설정 업데이트 (_config.yml)
- 이름: Jihwan Oh
- 이메일: ojh011016@kaist.ac.kr
- 소속: KAIST
- GitHub: jihwan01
- 웹사이트 URL: https://jihwan01.github.io

### 2. 메인 페이지 (_pages/about.md)
- 연구 관심사 및 철학 소개
- 현재 진행 중인 연구 하이라이트
- 학력 정보
- ISPASS 2025 발표 경험

### 3. CV 페이지 (_pages/cv.md)
- 학력: KAIST 전기및전자공학부, 전산학부 복수전공
- 연구 경험:
  * Georgia Tech & KAIST: Multi-GPU 성능 최적화
  * KAIST: PIM 아키텍처 최적화
- 기술 스킬:
  * Hardware Architecture
  * Performance Analysis & Profiling
  * Frameworks & Tools
  * Programming Languages
- 논문 발표: ISPASS 2025

### 4. 연구 페이지 (새로 생성: _pages/research.md)
- 연구 철학 및 방법론
- 현재 진행 중인 프로젝트 상세 설명:
  * Multi-GPU Performance Optimization
  * Processing-In-Memory (PIM) Architecture Optimization
- 연구 관심사 및 미래 방향

### 5. Publications (_publications/)
- ISPASS 2025 논문 추가
- 기존 샘플 논문들 삭제

### 6. Navigation 업데이트
- Publications
- CV
- Research
- 불필요한 섹션 제거 (Talks, Teaching, Portfolio, Blog Posts, Guide)

### 7. 샘플 컨텐츠 정리
- 샘플 포트폴리오 파일 삭제
- 샘플 talks 파일 삭제
- 샘플 teaching 파일 삭제
- 샘플 블로그 포스트 삭제

### 8. README.md 업데이트
- 개인 정보로 업데이트
- 연구 분야 소개
- 연락처 정보

## 로컬 테스트

웹사이트는 현재 로컬에서 실행 중입니다:
- URL: http://127.0.0.1:4001/

브라우저에서 위 주소로 접속하여 웹사이트를 확인할 수 있습니다.

## GitHub에 배포하기

웹사이트를 GitHub Pages에 배포하려면 다음 명령어를 실행하세요:

```bash
cd /Users/jh/jihwan01.github.io
git add .
git commit -m "Update personal website with CV and research information"
git push origin master
```

몇 분 후 https://jihwan01.github.io 에서 웹사이트를 확인할 수 있습니다.

## 추가 개선 사항

향후 다음과 같은 내용을 추가할 수 있습니다:

1. **프로필 사진**: `images/profile.png` 파일을 본인 사진으로 교체
2. **CV PDF**: `files/` 폴더에 CV PDF 파일 업로드
3. **논문 PDF**: 논문이 공개 가능한 경우 `files/` 폴더에 업로드
4. **추가 논문**: 새로운 논문이 발표되면 `_publications/` 폴더에 추가
5. **Google Scholar**: Google Scholar 프로필이 있다면 `_config.yml`에 링크 추가
6. **LinkedIn**: LinkedIn 프로필이 있다면 `_config.yml`에 추가

## 파일 구조

```
jihwan01.github.io/
├── _config.yml              # 사이트 설정 (개인 정보 업데이트 완료)
├── _data/
│   └── navigation.yml       # 네비게이션 메뉴 (업데이트 완료)
├── _pages/
│   ├── about.md            # 메인 페이지 (업데이트 완료)
│   ├── cv.md               # CV 페이지 (업데이트 완료)
│   └── research.md         # 연구 페이지 (새로 생성)
├── _publications/
│   └── 2025-01-ispass-multi-gpu.md  # ISPASS 2025 논문
└── README.md               # 프로젝트 설명 (업데이트 완료)
```

## 연락처

질문이나 추가 수정이 필요하면 언제든지 알려주세요!

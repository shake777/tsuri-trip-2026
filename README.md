# 北九州 釣りいこか倶楽部 — 여행 계획 사이트

키타큐슈 바다낚시 여행을 위한 회원 전용 페이지입니다.
회원 의견 수집, 일정 투표, 토론 게시판, D-DAY 카운트다운을 제공합니다.

## 주요 기능

- 여행 정보 (클럽 소개, 7가지 낚시 방법, 시즌 캘린더, 호텔/식당 비교)
- DAY 1~4 상세 일정 타임라인
- 4종 투표 (여행 일정, 낚시 방법, 숙박 호텔, 식당/메뉴)
- 회원 토론 게시판 (스레드 + 댓글)
- 회원 활동 통계
- 데이터 내보내기/가져오기 (JSON 기반)

## GitHub Pages 배포 방법

### 1단계: GitHub 계정 준비
- 이미 계정이 있다면 [github.com](https://github.com) 로그인
- 없다면 [github.com/signup](https://github.com/signup)에서 무료 가입

### 2단계: 새 저장소(Repository) 만들기
1. 우측 상단 `+` 아이콘 → **New repository** 클릭
2. Repository name: 원하는 이름 (예: `tsuri-trip-2026`)
3. **Public** 선택 (Private은 GitHub Pages 무료 사용 불가)
4. **Add a README file** 체크
5. **Create repository** 클릭

### 3단계: index.html 업로드
1. 저장소 메인 페이지에서 **Add file** → **Upload files** 클릭
2. `index.html` 파일을 드래그&드롭
3. 하단 **Commit changes** 클릭

### 4단계: GitHub Pages 활성화
1. 저장소 상단 **Settings** 탭 클릭
2. 왼쪽 메뉴 **Pages** 선택
3. **Source** 섹션:
   - Branch: `main`
   - Folder: `/ (root)`
4. **Save** 클릭
5. 1~2분 후 페이지 상단에 `Your site is live at https://(사용자명).github.io/(저장소명)/` URL 표시

### 5단계: URL 공유
- 위에서 생성된 URL을 카카오톡·메일로 공유
- 각 회원은 자기 이름을 입력하고 사이트 이용

## 데이터 통합 방법

이 사이트는 **localStorage** 기반이라 회원별 데이터가 각자 브라우저에 따로 저장됩니다.
의견을 통합하려면:

1. 각 회원이 **회원** 탭에서 "📥 모든 데이터 내보내기" 클릭 → JSON 파일 다운로드
2. JSON 파일을 단톡방·메일로 대표(예: DAYOU 님)에게 전송
3. 대표가 자신의 페이지에서 "📤 데이터 가져오기"로 각 JSON을 합침
4. 합쳐진 결과를 보고 최종 결정

## 실시간 데이터 공유가 필요하다면

Firebase Realtime Database 같은 백엔드와 연결하면 모든 회원이 동시에 같은 데이터를 볼 수 있습니다.
필요하시면 별도 개조 작업을 진행할 수 있습니다.

## 라이선스 및 출처

- 클럽 정보 출처: [tsuri-ikoka.com/general](https://tsuri-ikoka.com/general)
- 본 사이트는 회원 간 여행 계획 공유 목적의 비공식 자료입니다.

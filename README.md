# seran-portfolio
브랜치 규칙
브랜치 구조
main      → 배포용(항상 안정)
└─ stage  → main 머지 전 통합 테스트
   └─ 작업 브랜치들 (기능 단위)

브랜치 네이밍

기본 형식: feature/ui-YYMMDD, feature/data-YYMMDD, setting-YYMMDD 등

예시

feature/ui-251104 (UI 작업)

feature/about-251105 (About 섹션)

setting-251103 (환경 세팅)

필요 시 bugfix/…, hotfix/…도 사용 가능

커밋 규칙
형식
[행동][YYMMDD]-간단 설명


행동(Action): create | update | delete | enhance | connect

날짜: YYMMDD (예: 2025-11-03 → 251103)

설명: 1줄 요약 (한국어 OK)

예시
[update][251103]-개발환경셋팅
[create][251104]-Home 섹션 기본 레이아웃 생성
[enhance][251105]-프로젝트 카드 hover 인터랙션 개선
[delete][251105]-사용하지 않는 테스트 이미지 제거
[connect][251106]-EmailJS 연결 및 폼 검증 추가

커밋 원칙

한 커밋 = 하나의 목적(파일 여러 개 수정 OK, 주제가 1개면 됨)

설명은 간결하고 결과 중심(왜/무엇을)

대량 포맷팅/자동정리는 별도 커밋로 분리(update 또는 enhance)

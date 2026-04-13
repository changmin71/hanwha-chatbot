# 한화생명 보험 상담 AI 챗봇

Claude Sonnet API 기반의 보험 상담 챗봇 웹앱입니다.

## 기능

- **고객 상담 모드** — 친절한 AI 상담사가 보험상품 안내, 맞춤 추천, FAQ 응답
- **사내 업무 모드** — 간결한 사내 어시스턴트가 인수심사 기준, 청구/민원 프로세스 검색
- **7단계 맞춤 추천** — 연령/성별/가족/생활상황/건강/기존보험/예산 분석 후 포트폴리오 추천
- **상품 비교** — 사망보장, 건강보장, 저축 상품 비교표
- **자연어 대화** — Claude Sonnet이 상품 데이터 기반으로 자유 질의 응답

## 실행 방법

```bash
# 1. API 키 설정
echo "ANTHROPIC_API_KEY=your-key-here" > .env.local

# 2. 서버 실행
ruby server.rb

# 3. 브라우저에서 열기
open http://localhost:8080
```

## 기술 스택

- Frontend: Vanilla HTML/CSS/JS (빌드 도구 없음)
- Backend: Ruby WEBrick
- AI: Claude Sonnet API (Anthropic)
- Data: products.json (한화생명 8개 보험상품)

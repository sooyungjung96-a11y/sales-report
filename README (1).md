# 매출 분석 리포트

EBS 상품별 세부매출 데이터를 업로드하면 자동으로 분석 리포트와 AI 액션플랜을 생성하는 웹앱입니다.

## GitHub Pages 배포 방법

### 1단계 — GitHub 레포 만들기
1. github.com 접속 → 우상단 `+` → `New repository`
2. Repository name: `sales-report` (또는 원하는 이름)
3. **Public** 선택 (Pages 무료 사용 조건)
4. `Create repository` 클릭

### 2단계 — 파일 올리기
```bash
# 이 폴더에서 실행
git init
git add .
git commit -m "첫 배포"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/sales-report.git
git push -u origin main
```

### 3단계 — GitHub Pages 켜기
1. 레포 페이지 → `Settings` 탭
2. 왼쪽 메뉴 `Pages` 클릭
3. Source: `Deploy from a branch`
4. Branch: `main` / `/ (root)` 선택 → `Save`
5. 1~2분 후 `https://YOUR_USERNAME.github.io/sales-report` 접속 완료!

## 사용 방법

1. 링크 열기
2. Anthropic API 키 입력 (없으면 샘플로 먼저 체험 가능)
3. `상품별_세부매출_다운로드-YYYYMMDD.xls` 업로드
4. 자동 분석 완료!

## 분석 기능

- 📈 매출 개요 — 일별/월별 추이, 상위 상품
- 💳 신규 / 자동결제 — 실제 시트 데이터 기반 분석
- 📅 전년대비 (YoY) — 총매출/신규/자동결제 각각 비교
- ↩ 해지 / 환불 — 3종 구분 추이 분석
- 🏷 상품 상세 — 상품별 총매출/신규/자동결제 비교
- 🎯 액션플랜 — 데이터 기반 우선순위 액션 + AI 심층 분석

## 주의사항

- API 키는 사용자 브라우저에서만 사용되며 외부로 전송되지 않습니다
- 내부 사용 용도로, API 키를 코드에 하드코딩하지 마세요

# JMW 임직원 MALL

JMW 임직원 대상 직원구매 전용 웹 대시보드. 기존 [JMW Gear Spec Navigator]의 제품 데이터/UI 엔진을 참고해 별도 쇼핑몰형 화면으로 신규 구축.

## 현재 상태

- **버전**: V2.0
- **상태**: 목업(Mockup) 단계 — 모든 제품/가격/이미지/KPI 데이터는 더미(dummy) 데이터입니다.
- 실제 로우데이터(품목/계열/모델명/품번/직원가/URL) 및 제품 이미지(자사몰·프로페셔널 사이트 캡쳐본, 품번 기준 JPG) 취합 완료 후 `data/`, `assets/`에 반영 예정입니다.

## 구조

```
jmw_employee_mall/
├── index.html      # 대시보드 본체 (단일 파일, HTML+CSS+JS)
├── assets/         # 제품 이미지 (품번 기준 JPG) — 취합 완료 후 추가 예정
├── data/           # 제품 로우데이터 JSON — 취합 완료 후 추가 예정
└── README.md
```

## 주요 기능 (V2.0 기준)

- 카테고리별 TOP4 홈 화면 (DRYER / STYLER / HAIR CARE / ACCESSORY / HOME APPLIANCE)
- 카테고리 전체보기, 키워드 검색
- 장바구니(세션스토리지 기반, 로그인 없이 탭 단위로 유지·초기화)
- 제품 비교 (최대 6개, 가격+사양 비교)
- 직원구매 현황 대시보드 (기간 필터, 월별 매출 추이, 전년 대비, 채널/생산분류 도넛, 카테고리·TOP10 금액 비교)
- 영업지원팀 담당자 Google Chat 연결 (우측 하단)
- 우클릭/복사 방지 (클라이언트 단 저지 수준)

## 배포 (GitHub Pages)

1. 이 저장소를 GitHub에 생성 후 파일 업로드
2. Settings → Pages → Branch: `main` / `root` 선택
3. `https://<계정>.github.io/jmw_employee_mall/` 로 접속 가능

## 버전 관리 규칙

- 마이너 업데이트: `V2.0` → `V2.1`
- 메이저 업데이트: `V2.x` → `V3.0`
- 버전은 `index.html` 하단 푸터 및 파일 내 `APP_VERSION` 상수에 반영

## 문의

구매 및 업데이트 문의: **JMW 영업지원팀**

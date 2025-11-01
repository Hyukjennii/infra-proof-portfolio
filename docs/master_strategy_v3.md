# 🎯 Master Strategy v3: 인프라 실무 역량 증빙 프로젝트

---

## 1️⃣ 프로젝트 개요
본 프로젝트는 회사 데이터를 사용하지 않고,  
**개인 VM 환경에서 인프라 실무 역량을 객관적·정량적으로 증빙**하기 위한 실험형 포트폴리오이다.

주요 목표:
- 백업, 복구, 네트워크, 자동화 등 핵심 인프라 영역을 재현
- 운영 안정성 및 복원력 향상을 정량적으로 검증
- 상용 백업 환경(Zconverter, NetWorker)과 유사한 구조를 **무료 오픈소스(Bareos 등)** 로 구현
- 모든 실험과 분석은 **가명화·비식별화** 처리로 보안 문제 완전 회피

---

## 2️⃣ 현재 상태
- **직무:** 서버 인프라 관리자  
- **학력:** 방통대 통계데이터학과 1학기 재학  
- **목표:** 2027 상반기 내 실무 포트폴리오 완성 → 데이터 인프라/MLOps로의 기술 확장 기반 마련  

---

## 3️⃣ 기술 역량 구분

| 구분 | 목적 | 주요 기술 | 검증 결과물 |
|------|------|------------|---------------|
| **인프라 운영** | 시스템 안정성 및 효율적 자원 관리 | Linux, Shell, Cron, Bareos | 로그·리포트 |
| **자동화** | 점검·백업·알림 절차 자동화 | Shell, Python, GitHub Actions | 자동화 리포트 |
| **복구 및 장애 대응** | 복원 절차 표준화 및 실시간 복구 검증 | Bareos, rsync, netem | Fault Recovery Report |
| **모니터링/분석** | 로그 기반 성능 측정 및 통계 분석 | Python, Pandas, Matplotlib | Backup Summary Report |

---

## 4️⃣ 프로젝트 구조

infra-proof-portfolio/
├── infra_ops/
│ ├── scripts/ # 자동화 스크립트
│ │ ├── check_disk.sh # 디스크 점검
│ │ ├── check_network.sh # 네트워크 진단
│ │ ├── alert_notify.sh # 경보 데모
│ │ └── cron_jobs.txt # 점검 스케줄 예시
│ ├── reports/ # 리포트 및 분석 결과
│ │ ├── backup_summary.md # 백업 성공률 리포트
│ │ ├── fault_recovery.md # 장애 복원 절차 및 검증
│ │ └── operation_efficiency.md # 자동화 효율 분석
│ ├── data/
│ │ ├── backup_sim.log # 백업 로그 샘플
│ │ └── parsed_backup.csv # 분석용 변환 데이터
│ └── notebooks/
│ └── backup_trend.ipynb # 시각화 노트북
├── docs/
│ ├── master_strategy_v3.md # 본 문서 (전략 백서)
│ ├── backup_policy.md # 백업 정책 및 주기
│ ├── recovery_workflow.md # 복구 절차 문서
│ └── efficiency_standard.md # 운영 효율화 기준
└── README.md # 핵심 개요 / 진척도 / 링크

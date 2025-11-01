# 🚀 infra-proof-portfolio
> **인프라 실무 역량 증빙 프로젝트**  
> 회사 데이터를 쓰지 않고 개인 VM 환경에서 **백업·복구·네트워크·자동화** 역량을 정량적으로 입증합니다.

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](#)
[![Last Update](https://img.shields.io/badge/updated-this_week-blue.svg)](#)
[![Progress](https://img.shields.io/badge/progress-70%25-yellow.svg)](#)
[![License: MIT](https://img.shields.io/badge/license-MIT-lightgrey.svg)](#)

---

## 🔎 프로젝트 개요
이 저장소는 인프라 운영을 **재현·측정·리포트**하기 위한 실험형 포트폴리오입니다.  
- **백업 안정성**: 성공률/소요시간 로그 기반 분석  
- **장애 복원력**: 네트워크 지연/손실 주입 후 복구 절차 검증  
- **운영 효율화**: 수동 점검 대비 **자동화 전환 효과** 수치화

> 📘 전체 전략 백서(최신) → [docs/master_strategy_v3.md](docs/master_strategy_v3.md)

---

## 🧭 범위(인프라 전용 v3)
- OS/서버 운영 자동화 (Linux, Shell, Cron)
- 백업/복구 체계 (rsync, Bareos)
- 네트워크 장애 시뮬레이션 (`tc netem`)
- 로그 수집·통계·시각화 (Python, Pandas, Matplotlib)
- 문서/리포트 자동화 (Markdown → PDF)

※ **데이터 파이프라인(Kafka/Spark/Airflow 등)은 본 저장소 대상 아님.**  
향후 커리어 전환 전략은 별도 문서(`career_transition_plan.md`)로 관리 예정.

---

## 🧩 폴더 구조
infra-proof-portfolio/
├── infra_ops/ # 인프라 운영·자동화·복구 실험
│ ├── scripts/ # check_disk.sh, check_network.sh, alert_notify.sh, cron_jobs.txt
│ ├── reports/ # backup_summary.md, fault_recovery.md, operation_efficiency.md
│ ├── data/ # backup_sim.log, parsed_backup.csv
│ └── notebooks/ # backup_trend.ipynb (시각화)
├── docs/
│ ├── master_strategy_v3.md # 인프라 전용 전략 백서(최신)
│ ├── backup_policy.md # 백업 정책/보존 주기
│ ├── recovery_workflow.md # 복구 표준 절차
│ └── efficiency_standard.md # 운영 효율화 기준
└── README.md # 현재 파일

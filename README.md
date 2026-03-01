# 🇰🇷 Korean On-Chain Repo System Design & Economic Validation

### Smart Contract-Based Intraday Atomic DvP with Monte Carlo Simulation

16th DB Finance & Economics Competition  
Team: NODIT  
Category: Securities & Asset Management  

---

## 📌 Overview

This study proposes a **Korean On-chain Repo system** built on a permissioned blockchain architecture and quantitatively validates its economic impact.

Core methodologies include:

- Atomic Delivery-versus-Payment (DvP) via smart contracts
- KOFR-based interest rate modeling using the CIR model
- 10,000-run Monte Carlo simulation
- Integrated Total Economic Benefit (TEB) framework

---

## 🎯 Key Findings

- ✅ Up to **91.7% reduction in settlement risk**
- ✅ Approx. **KRW 3 trillion annual economic benefit**
- ✅ 12x reduction in Potential Exposure (T+1 → T+0)
- ✅ Haircut optimization improves collateral efficiency
- ✅ Liquidity buffer cost reduction under Basel III LCR

---

## 🧮 Total Economic Benefit Model

\[
TEB = Π(liquidity) + Π(haircut) + Π(buffer)
\]

Monte Carlo (10,000 runs) results:

- Mean: KRW 3.03 trillion
- 5th percentile: KRW 1.93 trillion
- Conservative scenario: KRW 1.23 trillion

---

## 🏗 System Architecture

Proposed architecture:

- Hyperledger Besu (IBFT 2.0)
- EVM-compatible Solidity smart contracts
- KSD central node
- BOK KOFR Oracle
- FSS regulatory monitoring node

Core contracts:

- AtomicRepoContract
- CollateralManager
- SettlementFinality

---

## 🔬 Methodology

- 1,044 KOFR historical observations
- OLS-estimated CIR parameters
- Basel III CRE22 haircut standards
- RiskMetrics √Δt exposure model
- Lognormal, Gamma, Normal probabilistic modeling

---

## 🌍 Differentiation from Global Platforms

| Feature | Global Platforms | This Study |
|----------|----------------|------------|
| Haircut | Static | Dynamic intraday |
| Regulatory Node | No | Yes (FSS) |
| Rate Benchmark | SOFR | KOFR + CIR |
| Economic Quantification | Not provided | TEB + Monte Carlo |

---

## 📈 Policy Implications

- Legal recognition of blockchain settlement finality
- Amendment of Capital Markets Act (Article 294)
- Smart contract enforceability clarification
- Centralized CSD-based on-chain infrastructure

---

## 🚀 Conclusion

This research demonstrates that blockchain-enabled repo markets can:

- Significantly reduce systemic risk
- Improve capital efficiency
- Establish a sovereign digital financial infrastructure

The proposed Korean on-chain repo model provides both technological feasibility and robust quantitative economic justification.

# 🇰🇷 한국형 온체인 레포(On-chain Repo) 시스템 설계 및 경제적 유효성 검증

### 스마트 컨트랙트 기반 일중 DvP 결제와 몬테카를로 시뮬레이션 분석

제16회 DB 금융·경제 공모전 출품작  
팀명: NODIT  
분야: 증권∙자산운용  

---

## 📌 연구 개요

본 연구는 전통적 레포(Repo) 시장의 구조적 비효율을 개선하기 위해  
**블록체인 기반 온체인 레포(On-chain Repo) 시스템**을 설계하고,  
그 경제적 유효성을 정량적으로 검증하였다.

핵심 접근 방법:

- 스마트 컨트랙트 기반 **Atomic DvP (Delivery versus Payment)**
- KOFR 기반 금리 모델링 (CIR 모형 적용)
- 10,000회 몬테카를로 시뮬레이션
- 총 경제적 편익(TEB) 통합 모델 구축

---

## 🎯 핵심 결과

- ✅ 결제 리스크 최대 **91.7% 감소**
- ✅ 연간 평균 **약 3조 원 경제적 편익**
- ✅ T+1 → T+0 전환 시 Potential Exposure 12배 감소
- ✅ 헤어컷 최적화를 통한 담보 효율성 개선
- ✅ LCR 유동성 버퍼 절감 효과

---

## 🧮 총 경제적 편익 (TEB) 모델

TEB는 3개 채널로 구성된다:

1️⃣ 유동성 조기 회수 수익  
2️⃣ 헤어컷 최적화에 따른 담보 해방 효과  
3️⃣ 일중 유동성 버퍼 기회비용 절감  

\[
TEB = Π(liquidity) + Π(haircut) + Π(buffer)
\]

몬테카를로 10,000회 시뮬레이션 결과:

- 평균: 약 3.03조 원
- 하위 5% 시나리오: 약 1.93조 원
- 보수적 가정 시: 약 1.23조 원

---

## 🏗 시스템 아키텍처

본 연구는 **Hyperledger Besu 기반 허가형 블록체인** 구조를 제안한다.

구성:

- 참여자 노드 (은행, 증권사, 보험사 등)
- KSD 중앙 노드
- BOK (KOFR Oracle)
- FSS 감독 노드
- Solidity 스마트 컨트랙트 3종:
  - AtomicRepoContract
  - CollateralManager
  - SettlementFinality

---

## 🔬 방법론

- KOFR 실데이터 (1,044건)
- CIR 금리 모형 파라미터 OLS 추정
- Basel III CRE22 기준 헤어컷 적용
- RiskMetrics 기반 √Δt 리스크 축소 모형
- 로그정규·감마·정규 분포 기반 확률 시뮬레이션

---

## 🌍 글로벌 대비 차별점

| 항목 | 글로벌 플랫폼 | 본 연구 |
|------|---------------|----------|
| 헤어컷 | 고정 | 동적 일중 헤어컷 |
| 규제 노드 | 없음 | FSS 감독 노드 |
| 금리 모델 | SOFR 연동 | KOFR + CIR |
| 편익 정량화 | 미제시 | TEB + MC 분석 |

---

## 📈 정책적 시사점

- 자본시장법 제294조 개정 필요
- 스마트 컨트랙트 법적 효력 명확화
- KSD 중심 단일 온체인 CSD 모델 제안
- 유동성 파편화 방지 구조 설계

---

## 🚀 결론

본 연구는 블록체인이 단순 기술 혁신을 넘어  
금융 시스템 효율성 혁명으로 작동할 수 있음을  
정량적으로 입증하였다.

온체인 레포는:

- 금융 안정성 강화
- 자본 효율성 증대
- 한국형 디지털 금융 인프라 구축

의 핵심 인프라가 될 수 있다.

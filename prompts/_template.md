---
id:                # 고유 식별자 (예: recon-2026-001)
version:            # 날짜 기반(YYYY-MM-DD) 또는 semver
author:             # 작성자
approver:           # 승인자 (승인 전까지 공란)
risk_level:         # Low | Medium | High
last_reviewed:      # YYYY-MM-DD
status: draft       # draft | in_review | approved | deprecated
target_tag:         # 예: payment-api, admin-console (실제 식별정보 금지)
---

# [프롬프트 이름]

## 1. 목적 / 역할

<!-- 이 프롬프트가 에이전트에게 맡기는 역할과 목적을 한 문단으로 -->

## 2. 전제조건 (인가 범위)

- 대상 범위:
- 사전 승인 근거(승인 티켓/문서 링크 등):
- 이 범위를 벗어난 대상에는 사용 금지

## 3. 입력 변수

<!-- 하드코딩 금지. 실행 시 채워 넣을 변수만 나열 -->
| 변수명 | 설명 | 예시(더미 값) |
|---|---|---|
| {{target_url}} | 점검 대상 URL | https://example.internal |
| {{credential_ref}} | 자격증명 참조 키(실제 값 아님) | vault://path/to/secret |

## 4. 기대 출력

<!-- 에이전트가 반환해야 할 결과의 형식/내용 -->

## 5. 실패·중단 조건

- 다음 상황에서는 즉시 실행을 중단한다:
  -
  -
- 중단 시 롤백/복구 방법:

## 6. 위험도 및 특이사항

- 위험도 산정 근거:
- 실행 전 재승인이 필요한 조건(해당 시):

---

**작성 시 체크리스트**
- [ ] 실제 고객/거래 데이터, 운영 도메인·IP, 자격증명 등 식별정보가 포함되지 않았는가
- [ ] 모든 대상 값이 변수로 파라미터화되어 있는가
- [ ] 위험도가 Medium/High인 경우 실패·중단 조건을 구체적으로 기술했는가

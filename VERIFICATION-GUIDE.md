# T04 검증안내서

기준: `spec/public-contract.json`, `spec/criterion-registry.json`

## 제출물

- 결과물 URL: `https://gamedh823-cmd.github.io/T04/`
- 소스 저장소 URL: `https://github.com/gamedh823-cmd/T04/commit/<commit 해시>`

## 재현·통과 확인

1. 어디로 가나요: 공개 결과물 URL 접속 → 상단 "현재 날씨" 탭
2. 무엇을 하나요(3단계 이내):
   1) 시·도/시·군·구/읍·면·동 선택
   2) "선택 지역 날씨 보기" 클릭
   3) "조회 정보" 카드 확인
3. 무엇이 보이면 통과:
   - 값·단위·출처(Open-Meteo)·출처 시각·조회 시각·기준 시간대(Asia/Seoul)가 모두 표시됨
   - 상태 배지가 "정상 · fresh/none"
4. 안 될 때 무엇이 보이나요:
   - 상태 배지가 "실패 · stale/{timeout|auth|rate_limit|offline|schema_error}" 중 하나로 표시
   - 마지막 정상값은 지워지지 않고 그대로 남아 있음
   - "↻ 다시 시도" 버튼 노출

## AI와 내 판단

1. AI에게 맡긴 일: normalized-reading 스키마 반영, 실패 상태 분기, 9개 fixture 재생 어댑터 구현
2. 내가 직접 판단한 일: (직접 채워주세요)
3. AI 말을 안 들은 일 (없으면 이유): (직접 채워주세요)

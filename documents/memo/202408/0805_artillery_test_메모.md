# Artillery 메모
부하 테스트 툴 중 하나인 Artillery 에 대한 메모입니다.

기존에 Artillery 에서 report 기능을 제공했습니다.  
CLI 모드에서 테스트 결과를 JSON 포맷으로 요약해주고 HTML 로 테스트 결과를 시각화해서 보여주던 report 기능이 deprecated 되고,  
시각화 및 분석 기능을 Artillery Dashboard 로 제공되도록 변경 예정입니다.

## Artillery Dashboard
- https://app.artillery.io/
- Artillery Cloud 서비스로 테스트에 대한 시각화 및 분석 기능을 제공
- 서비스가 더 발전하기 위해서 유료 모델을 도입한 것으로 보이며, 월 단위 구독 모델로 developer plan 은 제한적이지만 무료임
- 사용법
  - `artillery run test.yml --record --key YOUR_API_KEY`
  - API KEY 는 서비스에 가입하면 확인할 수 있다

## 출처
https://www.artillery.io/docs/reference/cli/report
> This command will be deprecated in the next major release of Artillery. We recommend using Artillery Dashboard for visualizing and analyzing Artillery reports.

# CartPole Environment 소개
## Reward
- 막대를 가능한 한 오랫동안 세워 두는 것이 목표
- 종료 단계를 포함하여 걸음마다 +1의 보상이 주어짐
- 보상의 threshold는 v1의 경우 500이고, v0의 경우 200임

## Starting State
- 모든 observations은 (-0.05, 0.05) 범위에서 균일하게 무작위 값을 할당받음

## Episode End
- 다음 중 하나라도 발생하면 에피소드가 종료
- 1.종료: 막대 각도가 ±12°를 초과할 경우
- 2.종료: 카트 위치가 ±2.4를 초과할 경우 (카트의 중심이 디스플레이 가장자리에 도달함)
- 3.단절: 에피소드 길이가 500을 초과할 경우 (v0의 경우 200)

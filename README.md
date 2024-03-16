# RL-Tutorial-Study
강화학습 튜토리얼 공부

<hr>

# CartPole


* γ: discount(0~1)
  * sum converges(합 수렴)

불확실한 먼 미래의 보상이 아닌 가까운 미래의 보상이 에이전트에게 더 중요하게 된다.

에이전트에게 먼 미래에 있는 보상보다 가까운 시일의 보상을 수집하기를 권한다.

주어진 상태에서 동작을 선택할 때 rewards를 최대화하는 방향으로 정책을 구성할 수 있다.

우리가 세상 물정을 다 알지 못하기 때문에 Q*에 대해 설정할 권한이 없다. 하지만 신경망 기법으로 대략적으로 접근할 수 있다. 임의의 상태로부터 학습된 Q*를

학습을 시킬 때 하나의 사실을 사용할 것이다. 벨맨 방정식을 따르는 몇몇의 정책을 위한 모든 Q함수는 다음과 같다.


# Huber Loss
* Q가 아주 noisy할 경우 outliers들을 대빟
  
### Definition
* 평균 제곱 오차(MSE)와 평균 절대 오차(MAE)의 장점을 결합한 것
* 오차가 작은 경우에는 MSE, 오차가 큰 경우에는 MAE를 사용
* 오차는 다음과 같이 정의
<img src="https://cdn.mathpix.com/snip/images/SAyRVC69H9yesBQ_DyXZQOfd1g0VclhQufkgWYKRQ4E.original.fullsize.png"/>

### expression
<img src="https://cdn.mathpix.com/snip/images/YMzNo150xygxUillJqFfuuLvDfUm5_0HeaUdXoZLGcI.original.fullsize.png"/>

# Dueling DQN Experiment Repository

Google DeepMind 팀이 발표한 Dueling DQN을 실습해봅시다.

1. Corridor Environment에서의 Policy Evaluation 실습(논문의 <code>Figure 3</code>)
2. <code>Atari Enduro-v0</code> 환경에서 vanilla DQN과 Dueling DQN이 찾은 final policy의 퍼포먼스 비교 실습

## 1. Corridor Experiment Plot Result

- 5 Actions

<p align="center"><img src="https://user-images.githubusercontent.com/79636473/159108872-62a681c9-abdd-4fe2-90bc-e0f114f0d046.png"></p>

- 10 Actions

<p align="center"><img src="https://user-images.githubusercontent.com/79636473/159108885-6cad46fa-b5da-4b3f-aa75-8c30032f6c54.png"></p>

- 20 Actions

<p align="center"><img src="https://user-images.githubusercontent.com/79636473/159108892-bd823b99-ac37-4191-9550-ed84d2f8a935.png"></p>

- Conclusion
  - 수렴 속도 측면에서 Dueling stream의 위력을 관찰할 수 있음.
  - 본 실험에서의 Single stream는 논문의 Single stream 보다 퍼포먼스가 안 좋음.
  - 반대로, 본 실험에서의 Dueling stream은 논문의 Dueling stream보다 더 좋은 퍼포먼스를 보임.
- Note
  - epsilon값을 논문과 달리 <code>0.01</code>로 설정하였음.

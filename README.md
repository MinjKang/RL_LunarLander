# 2022 Fall Semester 강화학습기초및응용

## 기본 실험 환경
Open AI GYM, Lunar Lander (https://www.gymlibrary.dev/environments/box2d/)

## Deep RL 기법들 </br>
- Deep Q-Network[^1]</br>
- Actor-Critic[^2] </br>
- Proximal policy optimization algorithms[^3]</br>

## 실험 결과 
episode 별 reward의 값을 나타낸 그래프로 4개의 모델 모두 동일하게 종료 조건 없이 훈련함, 실험 결과, PPO 알고리즘이 다른 모델 대비 200 이상의 reward 값에 가장 먼저 도달하지는 않지만 도달 이후에는 가장 안정적으로 수렴되며 훈련되는 것을 확인할 수 있음.

### Reward plot
![loss](https://github.com/MinjKang/Reinforcement_learning_LunarLander/blob/020ae3890c3b4f7662e7878982a1be67fb69f545/experiments_result.JPG)


## References
- Deep Q-Network (https://github.com/yuchen071/DQN-for-LunarLander-v2) </br>
- Actor-Critic, Proximal policy optimization algorithms  (https://github.com/bentrevett/pytorch-rl)

## Notes
아래 코드를 통해 `requirements.txt` 설치  

```
pip install -r requirements.txt
```


[^1]: Schulman, J., Wolski, F., Dhariwal, P., Radford, A., & Klimov, O. (2017). Proximal policy optimization algorithms. arXiv preprint arXiv:1707.06347
[^2]: Mnih, V., Badia, A. P., Mirza, M., Graves, A., Lillicrap, T., Harley, T., ... & Kavukcuoglu, K. (2016, June). Asynchronous methods for deep reinforcement learning. In International conference on machine learning (pp. 1928-1937). PMLR
[^3]: Mnih, V., Kavukcuoglu, K., Silver, D., Rusu, A. A., Veness, J., Bellemare, M. G., ... & Hassabis, D. (2015). Human-level control through deep reinforcement learning. nature, 518(7540), 529-533.

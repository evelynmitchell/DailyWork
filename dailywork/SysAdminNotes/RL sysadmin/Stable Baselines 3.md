## code 
https://github.com/DLR-RM/stable-baselines3

## docs 
https://stable-baselines3.readthedocs.io/en/master/
## docker
https://stable-baselines3.readthedocs.io/en/master/guide/install.html#using-docker-images
GPU image (requires [nvidia-docker](https://github.com/NVIDIA/nvidia-docker)):

docker pull stablebaselines/stable-baselines3

CPU only:

docker pull stablebaselines/stable-baselines3-cpu

---
docker run -it --runtime=nvidia --rm --network host --ipc=host --name test --mount src="$(pwd)",target=/home/mamba/stable-baselines3,type=bind stablebaselines/stable-baselines3 bash -c 'cd /home/mamba/stable-baselines3/ && pytest tests/'

Or, with the shell file:

./scripts/run_docker_gpu.sh pytest tests/

Run the docker CPU image

docker run -it --rm --network host --ipc=host --name test --mount src="$(pwd)",target=/home/mamba/stable-baselines3,type=bind stablebaselines/stable-baselines3-cpu bash -c 'cd /home/mamba/stable-baselines3/ && pytest tests/'

Or, with the shell file:

./scripts/run_docker_cpu.sh pytest tests/

## jax
https://github.com/araffin/sbxm SBX: Stable Baselines Jax (SB3 + Jax) RL algorithms 

## Contrib
https://github.com/Stable-Baselines-Team/stable-baselines3-contrib
**RL Algorithms**:

- [Augmented Random Search (ARS)](https://arxiv.org/abs/1803.07055)
- [Quantile Regression DQN (QR-DQN)](https://arxiv.org/abs/1710.10044)
- [PPO with invalid action masking (MaskablePPO)](https://arxiv.org/abs/2006.14171)
- [PPO with recurrent policy (RecurrentPPO aka PPO LSTM)](https://ppo-details.cleanrl.dev//2021/11/05/ppo-implementation-details/)
- [Truncated Quantile Critics (TQC)](https://arxiv.org/abs/2005.04269)
- [Trust Region Policy Optimization (TRPO)](https://arxiv.org/abs/1502.05477)
- [Batch Normalization in Deep Reinforcement Learning (CrossQ)](https://openreview.net/forum?id=PczQtTsTIX)

**Gym Wrappers**:

- [Time Feature Wrapper](https://arxiv.org/abs/1712.00378) https://arxiv.org/abs/1712.00378 "Time Limits in Reinforcement Learning

[Fabio Pardo](https://arxiv.org/search/cs?searchtype=author&query=Pardo,+F), [Arash Tavakoli](https://arxiv.org/search/cs?searchtype=author&query=Tavakoli,+A), [Vitaly Levdik](https://arxiv.org/search/cs?searchtype=author&query=Levdik,+V), [Petar Kormushev](https://arxiv.org/search/cs?searchtype=author&query=Kormushev,+P)

> In reinforcement learning, it is common to let an agent interact for a fixed amount of time with its environment before resetting it and repeating the process in a series of episodes. The task that the agent has to learn can either be to maximize its performance over (i) that fixed period, or (ii) an indefinite period where time limits are only used during training to diversify experience. In this paper, we provide a formal account for how time limits could effectively be handled in each of the two cases and explain why not doing so can cause state aliasing and invalidation of experience replay, leading to suboptimal policies and training instability. In case (i), we argue that the terminations due to time limits are in fact part of the environment, and thus a notion of the remaining time should be included as part of the agent's input to avoid violation of the Markov property. In case (ii), the time limits are not part of the environment and are only used to facilitate learning. We argue that this insight should be incorporated by bootstrapping from the value of the state at the end of each partial episode. For both cases, we illustrate empirically the significance of our considerations in improving the performance and stability of existing reinforcement learning algorithms, showing state-of-the-art results on several control tasks."

![[Screenshot from 2025-04-28 08-17-18.png]]

## hf
https://huggingface.co/sb3


## zoo
https://github.com/DLR-RM/rl-baselines3-zoo
https://rl-baselines3-zoo.readthedocs.io/en/master/

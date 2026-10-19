# Tiny World Models — AI Builders Lab

Hands-on Google Colab experiments for understanding **world models, reinforcement learning, and physical AI**.

## Open the notebooks

| Project | Goal | Technology | Open |
|---|---|---|---|
| **Mini World Model** | Learn 2D ball dynamics and imagine future trajectories | TensorFlow, NumPy | [Open in Colab](https://colab.research.google.com/github/dujing82-blip/tiny-world-models/blob/main/Mini_World_Model_Colab.ipynb) |
| **CartPole Control** | Balance one inverted pole by moving a cart left/right | Gymnasium CartPole-v1, PPO (Stable-Baselines3 / PyTorch) | [Open in Colab](https://colab.research.google.com/github/dujing82-blip/tiny-world-models/blob/main/CartPole_Control_Colab.ipynb) |
| **Double Pendulum Control** | Balance two linked inverted poles using continuous cart force | Gymnasium MuJoCo InvertedDoublePendulum-v5, PPO (Stable-Baselines3 / PyTorch) | [Open in Colab](https://colab.research.google.com/github/dujing82-blip/tiny-world-models/blob/main/Double_Pendulum_Control_Colab.ipynb) |

## How to run

Open a notebook in Google Colab and select **Runtime → Run all**.

- **Mini World Model:** CPU; no downloads required.
- **CartPole:** CPU; installs Gymnasium and Stable-Baselines3; moderate training time.
- **Double Pendulum:** CPU; installs MuJoCo and Stable-Baselines3; training can take several to tens of minutes. Default training is a starting point, **not a guarantee** of reliable balancing. If MuJoCo fails to import immediately after installation, restart the runtime and run all cells again.

## What students learn

1. **World model:** predicts the next state given the current state and an action.
2. **RL policy:** selects actions based on observations and rewards.
3. **Control:** applies actions repeatedly to keep a dynamic system stable.
4. **Model-based vs model-free:** the Mini World Model learns dynamics; the two PPO controllers learn policies and do **not** explicitly learn world models.

**Note:** The double pendulum starts near upright and focuses on balancing, not swing-up from a downward hanging configuration.

All notebooks are designed as educational examples. Results and training time vary by Colab runtime and random seed.

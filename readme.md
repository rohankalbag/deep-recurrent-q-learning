# Deep Recurrent Q-Learning for Partially Observable Markov Decision Processes

## EE782 : Advanced Topics in Machine Learning 

### Abstract 

This project presents our unique implementation of
**Deep Recurrent Q-Learning (DRQL)** that incorporates Transfer
Learning for feature extraction, a customized LSTM for temporal recurrence, and a domain-informed reward function. This
tailored approach aims to expedite convergence compared to the
vanilla implementation outlined in the [original paper](https://arxiv.org/abs/1507.06527). The performance evaluation focuses on two adaptive [Atari 2600](https://en.wikipedia.org/wiki/Atari_2600) games:
[Assault-v5](https://gymnasium.farama.org/environments/atari/assault/) and [Bowling](https://gymnasium.farama.org/environments/atari/bowling/), where game difficulty scales with player
proficiency. Comparative analysis between the convergence of our
optimized reward function and the vanilla version is conducted
using [StepLR](https://pytorch.org/docs/stable/generated/torch.optim.lr_scheduler.StepLR.html) and [CosineAnnealingLR](https://pytorch.org/docs/stable/generated/torch.optim.lr_scheduler.CosineAnnealingWarmRestarts.html) learning rate schedulers,
complemented by theoretical explanations. Additionally, an efficient windowed episodic memory implementation employing
bootstrapped sequential updates is proposed to optimize GPU
memory utilization


### Watch our agent play in action


Assault-v5           |  Bowling 
:-------------------------:|:-------------------------:
<img src="https://github.com/rohankalbag/deep-recurrent-q-learning/assets/46604893/11845492-2464-419e-b14a-26c98a813fd3" width=425></img> | <img src="https://github.com/rohankalbag/deep-recurrent-q-learning/assets/46604893/4607b58c-9502-4a6b-9e15-5bfe1f9cf93a" width=425></img> 


### Environment Setup 

```bash
python3 -m venv mlproj
source mlproj/bin/activate
pip install -r requirements.txt
```

> Link to [Jupyter Notebook](https://github.com/rohankalbag/deep-recurrent-q-learning-for-pomdps/blob/main/EE782.ipynb)
> Detailed [Report](https://github.com/rohankalbag/deep-recurrent-q-learning-for-pomdps/blob/main/Report.pdf) with Code, Experimentation and Results

### Collaborators:

- Rohan Kalbag
- Vansh Kapoor
- Sankalp Bhamare

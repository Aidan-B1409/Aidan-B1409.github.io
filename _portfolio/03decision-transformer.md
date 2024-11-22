---
title: "Decision Transformer for Robotic Arm Manipulation"
excerpt: "Transformers for offline reinforcement learning from synthetic data for robotics<br/><img 
src='/images/fetch_slide.gif'>"
collection: portfolio
---
Traditional methods in reinforcement learning iteratively update a policy function to optimize over non-continuous reward spaces. Recent work has demonstrated the possibility of reformulating these reward-based sequential decision problems as sequence learning problems. Simultaneously, the recent dominance of transformer models for sequence learning tasks has spurred research efforts to evaluate what domains can benefit from the powerful long-distance relationship learning possible with this architecture. The Decision Transformer seeks to unify these two principles with a generative trajectory modeling approach and a framework for large, interdependent sequence inputs. We extend the use of decision transformers to robotics control and demonstrate feasibility for this architecture to learn to control a 7-DoF robotic manipulator used to manipulate a simulated object.

![Push](/images/push.gif){:width="40%"} ![Reach](/images/reach.gif){:width="40%"}
![pick_and_place](/images/pick_and_place.gif){:width="40%"} ![slides](/images/fetch_slide.gif){:width="40%"}

To formulate this reinforcement learning problem as a sequence understanding problem, we represent each step of the
simulation as a state-action-reward tuple. Each input to our model then is a sequence of state-action-reward tuples,
representing each timestep in the trajectory.
We use the [GoFAR](https://jasonma2016.github.io/GoFAR/) dataset, which provides 40,000 action trajectories generated
from a random control policy, and 4,000 trajectories generated from an expert policy.
These policies control a 7-DoF robotic manipulator arm simulated in MuJoCo, from the [Gymnasium-Robotics](https://robotics.farama.org/envs/fetch/) library of reinforcement
learning environments.

![table](/images/decision_transformer_table.png)

We find that our decision transformer model, trained only on randomly synthesized control trajectories, is able to successfully complete the Reach task in 100% of trials. Using a combination of expert and randomly synthesized trajectories enables our model to learn more complex controls tasks. We find that Decision Transformers are able to effectively clone expert policies in an offline RL environment.

You can find the source code for our model and experiments [here](https://github.com/Aidan-B1409/AI535_DecisionTransformer), and a more in-depth writeup [here](/files/ai535_report.pdf)


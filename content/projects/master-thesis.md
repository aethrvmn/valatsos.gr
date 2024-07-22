---
type: "page"
showTableOfContents: true
---
# Reinforcement Learning: Theory and Implementation in a Custom Environment

You can find the thesis [here](/pdfs/mthesis.pdf) and the code [here](https://github.com/aethrvmn/GodotPneumaRL)

## Abstract

Reinforcement Learning (RL) is a subcategory of Machine Learning that consistently surpasses human performance and demonstrates superhuman understanding in various environments and datasets. Its applications span from mastering games like Go and Chess to optimizing real-world operations in robotics, finance, and healthcare. The adaptability and efficiency of RL algorithms in dynamic and complex scenarios highlight their transformative potential across multiple domains.

In this thesis, we present some core concepts of Reinforcement Learning.

First, we introduce the mathematical foundation of Reinforcement Learning (RL) through the Multi-Armed Bandit (MAB) problem, which serves as a simplified model for decision-making problems without state transitions, focusing solely on the trade-off between exploration and exploitation. We then extend the discussion to the more complex Markov Decision Processes (MDPs), which provide a formal framework for modeling decision-making problems where outcomes are partly random and partly under the control of a decision-maker, involving state transitions influenced by actions. Finally, we give an overview of the two main branches of Reinforcement Learning: value-based methods, which focus on estimating the value of states or state-action pairs, and policy-based methods, which directly optimize the policy that dictates the agent's actions.

We focus on Proximal Policy Optimization (PPO), which is the *de facto* baseline algorithm in modern RL literature due to its robustness and ease of implementation. We discuss its potential advantages, such as improved sample efficiency and stability, as well as its disadvantages, including sensitivity to hyper-parameters and computational overhead. We emphasize the importance of fine-tuning PPO to achieve optimal performance.

We demonstrate the application of these concepts within *Pneuma*, a custom-made environment specifically designed for this thesis. *Pneuma* aims to become a research base for independent Multi-Agent Reinforcement Learning (MARL), where multiple agents learn and interact within the same environment. We outline the requirements for such environments to support MARL effectively and detail the modifications we made to the baseline PPO method, as presented by OpenAI, to facilitate agent convergence for a single-agent level.

Finally, we discuss the potential for future enhancements to the *Pneuma* environment to increase its complexity and realism, aiming to create a more RPG-like setting, optimal for training agents in complex, multi-objective, and multi-step tasks.

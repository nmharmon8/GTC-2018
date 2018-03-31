# GTC 2018 Knowledge Dump
[GH-Pages](https://nmharmon8.github.io/GTC-2018/)
# Papers of interest in no particular order
- [Embodied Question Answering (Towards AI Agents that can see talk and act)](https://github.com/nmharmon8/GTC-2018/raw/master/papers/123987.928374.pdf)
- [Semi-supervised Learning with Deep Generative Models](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1406.5298.pdf)
- [Unrolled Generative Adversarial Networks](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1611.02163.pdf)
- [Unsupervised Image-to-Image Translation Networks](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1703.00848.pdf)
- [Model-Agnostic Meta-Learning for Fast Adaptation of Deep Networks](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1703.03400.pdf)
- [Towards End-To-End Speach Synthesis](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1703.10135.pdf)
- [Learning Important Features Through Propagating Activation Differences](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1704.02685.pdf)
- [Hindsight Experience Replay](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1707.01495.pdf)
- [Learning how to Active Learn: A Deep Reinforcement Learning Approach](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1708.02383.pdf)
- [Improving Landmark Localization with Semi-Supervised Learning](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1709.01591.pdf)
- [Learning with Opponent-Learning Awareness](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1709.04326.pdf)
- [Continuous Adaptation via Meta-Learning in Nonstationary and Competitive Environments](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1710.03641.pdf)
- [High-Resolution Image Synthesis and Semantic Manipulation with Conditional Gans](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1711.11585.pdf)
- [The Mechanics of n-Player Differentiable Games](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1802.05642.pdf)
- [Investigating Human Priors for Playing Video Games](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1802.10217.pdf)
- [IamNN: Iterative and Adaptive Mobile Neural Network for efficient image Classification](https://github.com/nmharmon8/GTC-2018/raw/master/papers/6eed1ee749e3b54fa92881d54a1a3dffb5716933.pdf)

# Talks of interest in no particular order -- Need to attach slides when released
> Learning with Oppent-Learning Awareness (LOLA)
- Notes: Learns with respect to opponents by differentiating with respect to the opponent's function (network parameters). Allows it to learn what its own action will cause the other learners to take.  
- Paper [Learning with Opponent-Learning Awareness](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1709.04326.pdf)
- Slides

> Towards AI Agents That Con See, Talk, and Act
- Notes: Agents learn through a form of curriculum training. Showing the human interactions helps the RL get started so it has a signal to train with. The curriculum training also initializes the network into the correct feature space, preventing it from learning an arbitrary character encoding.  
- Paper [Embodied Question Answering (Towards AI Agents that can see talk and act)](https://github.com/nmharmon8/GTC-2018/raw/master/papers/123987.928374.pdf)
- Slides

> Model Architectures and Training Techniques for High-Precision Landmark Localization
- Notes: Similar concept to "Towards AI Agents That Con See, Talk, and Act". A small amount of labeled data is used to initialize the network into the correct space, but then an alternative learning task is used to fully train the network.
- Paper [Improving Landmark Localization with Semi-Supervised Learning](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1709.01591.pdf)
- Slides

> Deep Active Learning
- Notes: May have applicability to SpecNet. At a minimum the confident scores would be useful. Train on a smaller set of data. Stop before overfitting to the data. Determine model uncertainty on samples of unlabeled data. Uncertainty is assigned based on the variance in class prediction using different dropout masks (has connections to bayesian stuff). Take samples that the model was most uncertain about and go through labeling process. Continue model training with the newly added samples. Repeat until the model is sufficiently accurate. Even if all data is labeled this method obtained higher accuracy then training on all the data. It might be interesting as a better way to sample data for batches. The presenter showed that this sampling typically changes the distributions of classes. Not sure if that is a good thing.  
- Paper - Could not find a paper
- Slides

> Learning to Learn, Deep Learning for Robotics, Deep Reinforcement Learning, AI for Manufacturing and Logistics
- Notes: I did not find an OpenAI baseline for this method. I think this is very appreciable to SC2. It allows few-shot adaptation to new environments and opponents. The biggest challenge I foresee is that we would still need the heartbeat to propagate rewards back to the agent which is very slow. Meaning that the few-shot adaptation will still take to much time. 
- Paper [Model-Agnostic Meta-Learning for Fast Adaptation of Deep Networks](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1703.03400.pdf) and [Continuous Adaptation via Meta-Learning in Nonstationary and Competitive Environments](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1710.03641.pdf)
- Slides

> Towards Lifelong Reinforcement Learning
- Notes: I think the previous approach is more applicable, but this is still interesting. 
- Paper [Investigating Human Priors for Playing Video Games](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1802.10217.pdf)
- Slides 

> IamNN: Iterative and Adaptive Mobile Neural Network for Efficient Image Classification
- Notes: Interesting analysis of ResNet. Would be interesting to explore adaptive computation on DeepSigint. Can scale computation based on available hardware and workload, which would be useful in a production environment. 
- Paper [IamNN: Iterative and Adaptive Mobile Neural Network for efficient image Classification](https://github.com/nmharmon8/GTC-2018/raw/master/papers/6eed1ee749e3b54fa92881d54a1a3dffb5716933.pdf)
- Slides 

> Not Just a Black Box: Interpretable Deep Learning for Genomics and Beyond. 
- Notes: This paper provides a way to determine which inputs were most important to the task. I missed the first part of the talk where this algorithm was explained, so I don't know how good it is. The speaker impressed me in the rest of the talk so I expect that it is interesting. 
- Paper [Learning Important Features Through Propagating Activation Differences](https://github.com/nmharmon8/GTC-2018/raw/master/papers/1704.02685.pdf)
- Slides

# Interests
- Sentinel 1&2 satellite -- Free satellite data
- Unified memory on TX2 -- managed_malloc
- Speech commands dataset Google
- Persistent kernels Cuda
- GPU direct RDMA
- Domain Generation Algorithms
- TensorRT
- Object classification using unordered point clouds


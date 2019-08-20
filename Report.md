# Report

## Description of the learning algorithm

The algorithm implemented to train the agent is [MADDPG](https://papers.nips.cc/paper/7217-multi-agent-actor-critic-for-mixed-cooperative-competitive-environments.pdf).

#### Hyperparameters chosen

- minibatch size: 128
- replay memory size: 1000000
- discount factor gamma: 0.99
- min squared gradient tau: 0.008
- learning rate actor: 0.0015
- learning rate critic: 0.0035
- weight decay: 0

#### Model Architecture
Each agent trains a model composed as follows:

1. The input to the neural network consists of a 24 x 1 vector representing the state observation

2. The first hidden layer is fully-connected and consists of 400 rectifier units.

3. The second hidden layer is fully-connected and consists of 300 rectifier units.

4. The output layer is a fully-connected linear layer with a single output for each of the 2 valid actions. The output layer uses tanh as output function.

## Performance of the trained agent
The environment is considered solved when the average of the maximum score between the two agents over 100 consecutive episodes is greater than *+0.5*.
The agents solved the environment in a total of **1902** episodes.

**Trained agent**

![trained_agent](https://user-images.githubusercontent.com/36470989/63344602-18f53080-c351-11e9-99bb-630245001acc.gif)



**Plot of the rewards obtained by the agent during the training**

![reward_plot](https://user-images.githubusercontent.com/36470989/63345132-56a68900-c352-11e9-96fd-eb7c5ea2e5ab.png)

## Future improvements

To improve the performance of the agent some of the suggestions for future work are:
- implementation of [Twin Delayed DDPG](https://spinningup.openai.com/en/latest/algorithms/td3.html)
- implementation of [Prioritized Experience Replay](https://arxiv.org/abs/1511.05952)

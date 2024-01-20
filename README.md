The goals of this project, carried out with the sales team of a Technology company in the Education industry, are to understand the underlying patterns in CRM data, and to optimize the user acquisition pipeline to improve the company’s sales funnel with the ultimate goal to create the best user experience for customers worldwide.
- Designed a Reinforcement Learning agent that optimizes the user acquisition pipeline to evenutally discover the optimal attributes and actions to increase overall sales.
- Data pre-processing and extensive Exploratory Data Analysis, focused on the distributions of categorical features and the chronological order of datetime features
- Modeled the state space as the union of the different encodings (mainly one-hot, but also boolean and integer) of the features
- Defined the action space and identified their transition probabilities
- Assigned the rewards to the target states and to intermediate secondary targets
- Implemented a Q-learning algorithm with state-based Q function modeled with a multi-layer Neural Network (Deep Q-Learning)
- Created the training loop with epsilon greedy action selection and fixed Q-target
- Implemented a Prioritized Replay Buffer with priority inversely proportional to the experience transition probability to solve the issue of low probabilities of the target state paths
- With the optimal policy obtained in the training, simulated 50'000 episodes to infer the best attributes and onboarding pipeline
- The optimal onboarding pipeline alone increased the probability of success of the first contact by 236% and of the subscription by 316%
- The optimal onboarding pipeline combined with the identified best candidates selection, increased the probability of success of the first contact by 571% and of the subscription by 864%

Curious for more? Check out the Notebook in the repo

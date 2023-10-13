# Q-learning_with_SMA_implementation

![image](https://github.com/EmoNasr/Q-learning_with_SMA_implementation/assets/87880384/36a57974-fea6-4ae0-8cc3-64e4053d5c73)


**What is Q-learning?**
Q-learning is a machine learning approach that enables a model to iteratively learn and improve over time by taking the correct action. Q-learning is a type of reinforcement learning.

With reinforcement learning, a machine learning model is trained to mimic the way animals or children learn. Good actions are rewarded or reinforced, while bad actions are discouraged and penalized.

With the state-action-reward-state-action form of reinforcement learning, the training regimen follows a model to take the right actions. Q-learning provides a model-free approach to reinforcement learning. There is no model of the environment to guide the reinforcement learning process. The agent -- which is the AI component that acts in the environment -- iteratively learns and makes predictions about the environment on its own.

Q-learning also takes an off-policy approach to reinforcement learning. A Q-learning approach aims to determine the optimal action based on its current state. The Q-learning approach can accomplish this by either developing its own set of rules or deviating from the prescribed policy. Because Q-learning may deviate from the given policy, a defined policy is not needed.

Off-policy approach in Q-learning is achieved using Q-values -- also known as action values. The Q-values are the expected future values for action and are stored in the Q-table.

Chris Watkins first discussed the foundations of Q-learning in a 1989 thesis for Cambridge University and further elaborated in a 1992 publication titled Q-learning.

**How does Q-learning work?**
Q-learning models operate in an iterative process that involves multiple components working together to help train a model. The iterative process involves the agent learning by exploring the environment and updating the model as the exploration continues. The multiple components of Q-learning include the following:

*Agents*. The agent is the entity that acts and operates within an environment.

*States*. The state is a variable that identifies the current position in an environment of an agent.

*Actions*. The action is the agent's operation when it is in a specific state.

*Rewards*. A foundational concept within reinforcement learning is the concept of providing either a positive or a negative response for the agent's actions.

*Episodes*. An episode is when an agent can no longer take a new action and ends up terminating.

*Q-values*. The Q-value is the metric used to measure an action at a particular state.

Here are the two methods to determine the Q-value:

Temporal difference. The temporal difference formula calculates the Q-value by incorporating the value of the current state and action by comparing the differences with the previous state and action.
Bellman's equation.
Mathematician Richard Bellman invented this equation in 1957 as a recursive formula for optimal decision-making. In the q-learning context, Bellman's equation is used to help calculate the value of a given state and assess its relative position. The state with the highest value is considered the optimal state.
Q-learning models work through trial-and-error experiences to learn the optimal behavior for a task. The Q-learning process involves modeling optimal behavior by learning an optimal action value function or q-function. This function represents the optimal long-term value of action a in state s and subsequently follows optimal behavior in every subsequent state.
![image](https://github.com/EmoNasr/Q-learning_with_SMA_implementation/assets/87880384/333f3b48-daaf-4f5a-9f92-be61b7c0d868)


**Result with SMA**
  **Best path**
  
Hello! Agent  agent0@192.168.1.106:1099/JADE is ready.
Hello! Agent  agent1@192.168.1.106:1099/JADE is ready.
Hello! Agent  agent2@192.168.1.106:1099/JADE is ready.
Hello! Agent  agent3@192.168.1.106:1099/JADE is ready.
Hello! Agent  agent4@192.168.1.106:1099/JADE is ready.

Agent agent0@192.168.1.106:1099/JADE is starting from (0,0)
(0,0) -> 3
(0,1) -> 3
(0,2) -> 3
(0,3) -> 3
(0,4) -> 3
(0,5) -> 1
(1,5) -> 1
(2,5) -> 1
(3,5) -> 1
(4,5) -> 1
Goal reached : (5 5)

Agent agent2@192.168.1.106:1099/JADE is starting from (0,0)
(0,0) -> 3
(0,1) -> 3
(0,2) -> 3
(0,3) -> 3
(0,4) -> 3
(0,5) -> 1
(1,5) -> 1
(2,5) -> 1
(3,5) -> 1
(4,5) -> 1
Goal reached : (5 5)

Agent agent4@192.168.1.106:1099/JADE is starting from (0,0)
(0,0) -> 3
(0,1) -> 3
(0,2) -> 3
(0,3) -> 3
(0,4) -> 3
(0,5) -> 1
(1,5) -> 1
(2,5) -> 1
(3,5) -> 1
(4,5) -> 1
Goal reached : (5 5)

Agent agent1@192.168.1.106:1099/JADE is starting from (0,0)
(0,0) -> 3
(0,1) -> 3
(0,2) -> 3
(0,3) -> 3
(0,4) -> 3
(0,5) -> 1
(1,5) -> 1
(2,5) -> 1
(3,5) -> 1
(4,5) -> 1
Goal reached : (5 5)

Agent agent3@192.168.1.106:1099/JADE is starting from (0,0)
(0,0) -> 3
(0,1) -> 3
(0,2) -> 3
(0,3) -> 3
(0,4) -> 3
(0,5) -> 1
(1,5) -> 1
(2,5) -> 1
(3,5) -> 1
(4,5) -> 1
Goal reached : (5 5)

  **Q-Table**
  
  agent0@192.168.1.106:1099/JADE
  
0.34867843889971595 0.31381054966767624 0.3486784396046058 0.3874204889999975
0.38742048721412586 0.3486784386231792 0.34867843947839783 0.43046720999999744
0.430467209996667 0.3874204888288516 0.38742048899148046 0.47829689999999736
0.4782968995056102 0.43046720891817997 0.43046720934463373 0.5314409999999974
0.5314409987022358 -0.4095100002700213 0.47829689701078015 0.5904899999999977
0.5904899998883641 0.6560999999999979 0.5314409997044255 0.5904899999292189
0.3486784351883672 0.06083691964856201 0.2605815136541366 0.3066876611162774
0.33508563437305194 0.27147685334461386 0.25680099086128444 0.3874204889920947
0.43046720999999744 0.29252041658598155 0.3372469116259736 0.41588299154744657
0.4782968999993957 0.30678093305252835 0.3010393687833931 -0.4319300914915779
0.5233208064330241 0.5968416058565136 0.40827931754979796 0.6560999999999979
0.5904899999910276 0.7289999999999983 -0.409510001031372 0.6560999987132051
0.08558317908955124 0.0 0.005177063476485465 0.1765797982502184
0.3439019576615444 0.01575675197273164 0.0185742995394071 0.13841542687907485
0.378475374865711 -0.6123284843769604 0.17951382321610887 0.11020004608068153
0.4294618845865539 -0.65645650725531 0.14166332886142005 -0.05501847257428161
-0.4743343458269878 0.5230591321924289 0.3249327803220652 0.7289999996961523
0.6560999972889424 0.8099999999999987 0.656099995989458 0.7289999996989549
0.006744899215688673 0.0 0.0 0.0
0.12311257434572027 0.0 0.0 0.0
0.18835672866224193 -0.08658684398576233 0.007186054618730992 -0.1
0.358962014370852 -0.0864758135970244 -0.2442155924551125 0.2506317533954262
0.4912579997523056 0.6697586928129108 -0.6875404600952434 0.8099999996612931
0.7289999998821717 0.899999999999999 0.7289999972354505 0.8099999999570295
0.0 0.0 0.0 0.0
0.0 0.0 0.0 0.0
-0.4253282697693178 0.0 0.0 -0.030295408174815186
-0.5884825220121364 -0.03781823817375533 0.0 0.27855614205382584
0.5715176106650337 0.4127471975017857 -0.18266132713234645 0.8999998980138889
0.8099999924208249 0.9999999999999996 0.8099990446476806 0.8999999971326178
0.0 0.0 0.0 0.0
0.0 0.0 0.0 0.0
-0.0323974794257201 0.0 0.0 0.0
-0.11436621197470764 0.0 -0.002268000000000001 0.0
0.12503326882122698 0.0 -0.00563646363854688 0.7712320754503901
0.0 0.0 0.0 0.0
agent2@192.168.1.106:1099/JADE
0.3486784399275654 0.31381058989300314 0.3486784397029839 0.3874204889999975
0.38742048839289217 0.34867842151227035 0.348678439939877 0.43046720999999744
0.43046720998613



**Result without SMA**

***********Q-Table***********

|0.3874204889999975|	0.3138105115754162|	0.3486784399576183|	0.34867844003996645|	|
|0.43046720999999744|	0.34867843087323913|	0.3486784381274481|	0.3874204889117825|	|
|0.47829689999999736|	0.3874204875944293|	0.38742048792582745|	0.4304672099819629|	|
|0.5314409999999974|	0.5115976102318408|	0.4304672098389642|	0.4782968999063541|	|
|0.5904899999999977|	-0.40951000603574417|	0.4782968998154497|	0.531440999466755|	|
|0.5904899947631348|	0.6560999999999979|	0.5314409992693973|	0.5904899986682535|	|
|0.2808133918291538|	0.14990706917472965|	0.2810990464264521|	0.3486784333374303|	|
|0.30642021052007684|	0.35607706169159936|	0.26555605025845386|	0.38742048653299993|	|
|0.2823053337721353|	0.3739082457489844|	0.24934448193184056|	0.43046720994927723|	|
|-0.4350109901165987|	0.583695230674976|	0.31972301742170983|	0.4782968789420375|	|
|0.6560999999999971|	0.6198329633037004|	0.4422097559016798|	0.5091917910807698|	|
|0.6560999995687546|	0.7289999999999983|	-0.40951000907275714|	0.5904899992500762|	|
|0.31822883220854126|	-0.3487563453204602|	0.02728951729648066|	0.05961158539211689|	|
|0.5147473309434254|	-0.5179787258523889|	0.04842923617303001|	0.06607126307006347|	|
|0.5898048875759778|	-0.5340173424462108|	0.22815855782692956|	0.17825948016815427|	|
|0.6560994751663093|	-0.47308017290578247|	0.423281370751235|	0.2913492365150411|	|
|0.728999999999984|	-0.2699808619361709|	0.5618306040392167|	-0.40186086421301787|	|
|0.7289999998877487|	0.8099999999999987|	0.6560999997247641|	0.6560999999017046|	|
|-0.10830171244237607|	0.0|	0.0|	0.054113178426053815|	|
|-0.4531856074131294|	0.0|	0.0|	0.0|	|
|-0.09912446467530495|	7.121476807117887E-4|	-0.2355974494142353|	0.3746762511194779|	|
|-0.08611533853743761|	0.013320896508383504|	-0.23218742935704575|	0.5392485705489392|	|
|0.8099999997150678|	0.6509072119784871|	-0.5387999449837512|	0.5670789949891158|	|
|0.8099999996354552|	0.899999999999999|	-0.2710000083161886|	0.7289999998928508|	|
|0.0|	0.0|	0.0|	0.0|	|
|0.0|	0.0|	0.0|	0.0|	|
|0.007912752007908763|	0.0|	0.0|	-0.08722601215564166|	|
|0.08088357964598904|	0.15638392205955348|	0.0|	-0.1665544334633728|	|
|0.89999994763184|	0.5913591151277563|	0.024569292696690538|	-0.24963530746694848|	|
|0.899999998956678|	0.9999999999999996|	0.8099995106352835|	0.8099999994326685|	|
|0.0|	0.0|	0.0|	0.0|	|
|0.0|	0.0|	0.0|	0.0|	|
|0.002785590000000001|	0.0|	0.0|	0.0|	|
|0.45451943310534826|	0.008080389900000002|	0.0|	0.007912752007908763|	|
|0.9282102012308148|	0.12524641509007803|	0.05035674756903301|	0.19759864395535265|	|
|0.0|	0.0|	0.0|	0.0|	|

State: (0) | Best action: 0
New state: (1)

State: (1) | Best action: 0
New state: (2)

State: (2) | Best action: 0
New state: (3)

State: (3) | Best action: 0
New state: (4)

State: (4) | Best action: 0
New state: (5)

State: (5) | Best action: 1
New state: (11)

State: (11) | Best action: 1
New state: (17)

State: (17) | Best action: 1
New state: (23)

State: (23) | Best action: 1
New state: (29)

State: (29) | Best action: 1
New state: (35)


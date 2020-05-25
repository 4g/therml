
## Using data to cool data centers
Data centers consume 2–3% of worlds power¹. 30–50% of this power goes into keeping it cool². A system of different mechanisms works together to bring heat out from a datacenter and discard it into the atmosphere. These mechanims are controlled by their own local control systems. In this post, we detail how to control a system of systems more efficiently.

### 
**Why are they inefficient ?**
 - Local controls
 - Tacit knowledge
 - Complex interaction
 - Difficult to model

**Can we design a better control system ?** 
 - Data based modelling
 - Fixed point optimisation 
 - Reinforcement learning on data model
 - Reinforcement learning directly on system
 - Continuous control

**Let us try it on a simple simulator ?** 
 - Environment
	 - Red balls are hot, blue balls are cold
	 - Physics engine simulates motion of balls
	 - Reward is given when all servers have cooled down
	 - Time penalty for taking too long
	 - Pymunk engine
 - Trpo agent
 - Results

**Modelling a real data center**
 - Sensory data from a real DC. Glance into data, simple EDA. 
 - Part based models
	 - Time delay in action
	 - LSTMs to simulate individual parts
	 - Each part connected to another
	 - Part connection graph
	 - State Machine composed of these parts is our simulator
	 - Accuracy of simulation
	 - Model sanity check
 - By product, predictive maintenance 

**Simple optimisation on data model**
 - Better setpoints according to weather
 - Reacting with a chiller instead of PAHUs

 **RL policies**
 - Agent
 - Rewards
 - Results

**System design**

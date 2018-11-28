# Artificial Neural Networks

- Inspired by biology.
- We have different neural network architechtures proposed for variety of analytics tasks. such as :
  - Regression.
  - Classification. (For now we will concentrate on classification only)
  - Clustering.
  - Feature extraction etc.
- There architechtures are netwrok of simple computing entities.
- Resurgance (increase) in interest recently.

# Biological Neural Network

- Looking into biological neural network, we will basically only focus on input and the output.
- Neuron receives input from dendrite or dendrite branches.
- and when input signal is above a certain threshold its going to produce an output that is going to be transmitted via tha synapsis to neurons that are further down the line.
- These connections through the dendrites and lapses are going to result in a complex network, even though the computing done by each element is very simple, summation and thresholding the sum,  total of this taken across on the network can give raise to very complex computations.

# A simple computing unit
  
![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Supervised%20Learning(Regression%20and%20Classification%20Techniques)/Artificial%20Neural%20Networks/simple_computing_unit.PNG)

# McCulloch Pitts Unit (1943)
- Initial model was proposed by McCulloch pitts (1943), known as McCulloch pitts unit or MP units.
- Uses only binary signals. i.e 0's and 1's.
- Nodes also produce only binary results (outputs are only 0's or 1's).
- Edges between these nodes are : 
  - Directed, Unweighted.
  - Are of two types : Excitatory or Inhibitory.
  - Transmits only binary signals.

![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Supervised%20Learning(Regression%20and%20Classification%20Techniques)/Artificial%20Neural%20Networks/McCullochPittsNeuronModel.png)

# Rules for evaluating the input

- Assume that a MP unit gets input X1, X2, .....Xn through n excitatory (+ve) edges and inputs Y1, Y1 .....Ym through the inhibitory edges.
- If m>=1 and atleast on of the Yi is 1, the unit is inhibited and the result of computation is 0.
- Otherwise, computed X= X1 + X2 + ....Xn if X>= 0(theta) the result is 1, else the result is 0(Zero).
- So the inhibitory in some sense here act as a gating signal. So if it is 1 the output is always 0 and if it is 0 then the output is result of computation.

**Step function with threshold**

![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Supervised%20Learning(Regression%20and%20Classification%20Techniques)/Artificial%20Neural%20Networks/step_function.gif)

- If input is below threshold 0(theta), output is 0(zero).
- If input is above threshold 0(theta), it makes the output 1

# What type of computations can we do with MP model

- Almost all of our familiar boolean operations with the MP neuron

![alt text](https://raw.githubusercontent.com/AbhishekKumar4/Data-Analytics/master/Supervised%20Learning(Regression%20and%20Classification%20Techniques)/Artificial%20Neural%20Networks/ComputationsbyMP.jpg)

**AND**
- If only both X1 and X2 are 1 so it will be >= threshold therefore output will be 1.

**OR**
- Either X1 or X2=1 , therefore output=1

**NOT**
- X1 acts as a inhibitory unit.
- if X1=1, inhibited o/p=0
- if X1=0, inhibited o/p=1 (or result of computation).

**Connect all together and solve any boolean function**

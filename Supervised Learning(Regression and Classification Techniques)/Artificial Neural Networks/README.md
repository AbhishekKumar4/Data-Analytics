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

![alt text]()

# Rules for evaluating the input

- Assume that a MP unit gets input X1, X2, .....Xn through n excitatory (+ve) edges and inputs Y1, Y1 .....Ym through the inhibitory edges.
- If m>=1 and atleast on of the Yi is 1, the unit is inhibited and the result of computation is 0.
- Otherwise, computed X= X1 + X2 + ....Xn if X>= 0(theta) the result is 1, else the result is 0(Zero).
- So the inhibitory in some sense here act as a gating signal. So if it is 1 the output is always 0 and if it is 0 then the output is result of computation.

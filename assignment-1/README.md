# Assignment 1: Background & Very Basics

------

Submitted by: Shivam Sharma 

### Questions 

1. **What is a neural network neuron?**

   **Answer**: An artificial neuron or simply called unit is the building block of an artificial neural network. Working of artificial neuron is based on how a biological neuron works. A biological neuron accepts input signals via its dendrites, which pass the electrical signal down to the cell body.

<p align="center">
  <img src="https://github.com/shivams619/end3.0_assignments/blob/2cab01ad2118625c78265b53ed2953097555d298/assignment-1/img/1_9DRHyzHBQs2DTYA5Wd_leQ.png" />
</p>

​		An artificial neuron works similarly. In an artificial neuron there are three main components.

<p align="center">
  <img src="https://github.com/shivams619/end3.0_assignments/blob/3d1014c793e9d8652594105796fc27ae294f867d/assignment-1/img/1_EuHPHlcyI1jCXopnP1QbYg.png" />
</p>

- **Input Signal**

  When input data comes in, it get multiplied by the weights assigned to that input value.

- **Sum**

  The weighted input is then summed up. Here a bias value or bias unit is also added to the sum as an offset . 

- **Activation**

  Now, the calculated signal is fed into a transfer function also called as a activation function.

  

2. **What is the use of the learning rate?**

     **Answer**: Learning rate parameter controls how much the coefficients can change on each update. 

<p align="center">
  <img src="https://github.com/shivams619/end3.0_assignments/blob/3d1014c793e9d8652594105796fc27ae294f867d/assignment-1/img/0_QwE8M4MupSdqA3M4.png" />
</p>

  ​		If the learning rate is very small then it will take the algorithm more time to converge on the global minima, However if the 		learning rate is big then it may miss the       global minima.



3. **How are weights initialized?**

   **Answer:** Deterministic algorithms execute same steps on the same input data every time they run. While using the deterministic approach best, worst and average running time can be determined, however deterministic algorithms are not suitable for complex problems or they may take computationally impractical time while solving them.

   An alternate is to use nondeterministic algorithms. These algorithms use elements of randomness when making decisions during the execution of the algorithm. This means that different order of steps will be executed every time they run on the same data. Randomness breaks symmetry and remove the bias giving a better likelihood of finding optimal solution. Hence the weights are randomly initialized. 

   

4. **What is "loss" in a neural network?**

   **Answer:** Loss indicate how far an estimated value is from its true value. A loss function maps decisions to their associated costs. Loss functions are not fixed, they can be changed depending on the task in hand and the goal to be met.

   

5. **What is the "chain rule" in gradient flow?**

   **Answer:** The chain rule is a formula for calculating the derivatives of composite functions. Composite functions are functions composed of functions inside other function(s).
   <p align="center">
  <img src="https://github.com/shivams619/end3.0_assignments/blob/3b342f009866299380466d1cd61ef279c7c3dad1/assignment-1/img/chainrule.PNG" />
</p>
<p>Backpropagation algorithm is used to effectively train a neural network using chain rule. In simple terms, after each forward pass through a network, backpropagation performs a backward pass while adjusting the model’s parameters (weights and biases). Backpropagation aims to minimize the cost function by adjusting network’s weights and biases.</p>

<p>The derivative of a function C measures the sensitivity to change of the function value (output value) with respect to a change in its argument x (input value). The derivative tells us the direction C is going. The gradient shows how much the parameter x needs to change (in positive or negative direction) to minimize C.
Compute these gradients happen using chain rule. 
 

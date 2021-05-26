# BackPropagation_Scratch

1) Implementing backpropagation and Gradient checking  

## Algorithm for Forward Propagation 


    X: input data point, note that in this assignment you are having 5-d data points
    y: output varible
    W: weight array, its of length 9, W[0] corresponds to w1 in graph, W[1] corresponds to w2 in graph, 
         ..., W[8] corresponds to w9 in graph.  
    you have to return the following variables
    exp= part1 (compute the forward propagation until exp and then store the values in exp)
    tanh =part2(compute the forward propagation until tanh and then store the values in tanh)
    sig = part3(compute the forward propagation until sigmoid and then store the values in sig)
    now compute remaining values from computional graph and get y'
    write code to compute the value of L=(y-y')^2
    compute derivative of L  w.r.to Y' and store it in dl
    Create a dictionary to store all the intermediate values
    store L, exp,tanh,sig,dl variables
 
## Algorithm for Backpropagation 

     L: the loss we calculated for the current point
     dictionary: the outputs of the forward_propagation() function
     write code to compute the gradients of each weight [w1,w2,w3,...,w9]
     Hint: you can use dict type to store the required variables 
     return dW, dW is a dictionary with gradients of all the weights
  
 ## Algorithm for gradient checking 
 
     compute the L value using forward_propagation()
     compute the gradients of W using backword_propagation()
    approx_gradients = []
    for each wi weight value in W:
        add a small value to weight wi, and then find the values of L with the updated weights
        subtract a small value to weight wi, and then find the values of L with the updated weights
        compute the approximation gradients of weight wi
        approx_gradients.append(approximation gradients of weight wi)
    compare the gradient of weights W from backword_propagation() with the aproximation gradients of weights with gradient_check formula
    
   
2) Optimizers 
 
 Implemented three types of Optimizers: 
 
 a) Vanilla Update //
 b) Momentum Update  //
 c) Adam Update  //
 
 

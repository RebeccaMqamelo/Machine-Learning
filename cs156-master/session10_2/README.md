## 10.2 Recurrent Neural Networks

## Study Guide

After completing the readings, you should be able to answer the following questions:

- Why is a Hopfield network a recurrent network?
- Give an example where the synchronous Hopfield network fails to converge to a solution. Explain in your own words why this happens, and how we might modify the network to guarantee convergence.
- Explain in your own words why the inverse of a stable state is also a stable state.

## Pre-class work

Implement a Hopfield Network, and perform the basic analysis below:

1. **Store**
   Implement a Python function which is able to store a memory in a Hopfield network.
2. **Recall**
   Implement a Python function which runs the recall algorithm for an initial (corrupted) memory. Make sure to include a stopping criteria.
3. **Capacity**
   Write a function to determine the capacity for a Hopfield network of a given size. This function should have a size parameter, and then initialize an empty Hopfield network. It must then store a random memory and test whether the network is able to recall the correct memory if given a pattern corrupted by a single bit. The function must then return the largest number of memories that were stored and successfully recalled.
4. **Scaling Behavior**
   Produce a plot showing capacity as a function of network size. What is the scaling behavior?
5. **(_optional_) Asynchronous Updates**
   Change your implementation so that the state is updated asynchronously. Find a state that didn't converge in your original implementation, and show that it does converge in your new implementation.
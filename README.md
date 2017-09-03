# CarND-Controls-MPC
Self-Driving Car Engineer Nanodegree Program

---


This is my (Anton Varfolomeev) solution of MPC project

---

## Reflections on the solution

It seems that one of the difficult and time-consuming part (for me at least) of this
project was integration with Ipopt and CppAD libraries. It took some time to
set environment (I use Ubuntu shell in Windows 10) - and it certainly required a 
lot of attention to pack all variables and constraints right way.

It was a little bit frustrating at first, but then I accepted it as just another practice of 
understanding a may-be-good library (package, framework) that one will use - or not.

After correction of inevitable errors (angle sign, index offset etc.), I received MPC
that at least tried to run. 

The next stage was objective function weights adjustment. Once again: objective function designs 
plays rather important part in the life of ML engineer. As a result, I received a smoothly
running car that achieved speeds up to 80 MPH (without delay).

Delay incorporation seemed a little bit tricky until I found that angle and acceleration 
values I can receive from the simulator. Then it became just the same state update function 
we used many times.





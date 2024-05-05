### Monte Carlo Techniques

We generally give up on truly random numbers, and use “Pseudo-Random” sequences of numbers instead.

One example of a pseudo-random number generator is the linear congruential generator:

x<sub>n + 1</sub> = (ax<sub>n</sub> + b) % c

This pseudo-random number generator takes a “seed” x0 and generates a
series of numbers which, depending on the choices of a, b, and c, can meet
the necessary criteria for Monte Carlo techniques.

It’s necessary that our random numbers meet the criteria :

- They must be uniformly distributed.
- They must be uncorrelated.
- We need a lot of points. Our percent error by this method is going to
  scale roughly as 1 / sqrt(N) so for a mere three significant figures in the answer,
  we need a million data pairs.
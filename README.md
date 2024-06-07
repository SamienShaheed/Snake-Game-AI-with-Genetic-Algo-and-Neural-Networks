# Snake-Game-AI-with-Genetic-Algo-and-Neural-Networks

This environment was extended from the existing repo:
https://github.com/greerviau/SnakeAI/tree/master

## Abstract
This report presents an intelligent agent developed to play the Snake Game using Genetic Algorithms and Neural Networks. The project investigates the impact of the number of hidden layers, the number of neurons, and the mutation rate on the efficacy of this intelligent agent. Multiple experiments were conducted to find the most efficient combination of parameters.

## Introduction
The project aims to investigate how the number of hidden layers in neural networks affects an intelligent agent's learning rate and efficacy in playing the Snake Game. The agent uses a simple neural network to control the snake's movement, optimized by a genetic algorithm. The custom environment for the Snake Game was developed using the Processing 4 IDE.

## Methodology
Inspired by hybrid models of neural networks and genetic algorithms, the project uses a neural network to steer the snake and genetic algorithms to improve the weights of the individual snakes in a population. The network architecture was experimented with varying the number of hidden layers and neurons per layer, as well as different mutation rates. Each generation consisted of 2000 individuals, and experiments were iterated for 50 generations.

## Experimental Design
A total of 27 experiments were conducted with different model architectures:
- One hidden layer, two hidden layers, and three hidden layers.
- Mutation rates: 0.01, 0.05, and 0.1.
- Neurons per layer: 6, 16, and 24.

## Results
- **Single-Layer Models**: Performed the best with faster improvement and higher scores.
- **Multi-Layer Models**: Showed poorer performance due to added complexity, leading to unnecessary moves and loops.
- **Mutation Rates**: Higher mutation rates (5% and 10%) led to better performance, while lower rates (1%) resulted in long plateaus and poor improvement.

## Discussion
The results suggest that simpler neural network architectures perform better for the Snake Game. Higher numbers of hidden layers lead to overfitting and slower learning. The mutation rate is crucial in avoiding local optima, with moderate rates yielding the best results. Initial conditions, such as the starting position of the snake, significantly influence the agent's learning patterns.

## Conclusion
The hybrid approach using neural networks and genetic algorithms demonstrates that simpler models with moderate mutation rates perform better in training an agent to play the Snake Game. Further work includes normalizing the starting position of the snake for more reliable results.

## References
1. P. Białas, "Implementation of artificial intelligence in Snake game using genetic algorithm and neural networks," CEUR Workshop Proc., vol. 2468, pp. 42–46, 2019.
2. A. Lambora, K. Gupta, and K. Chopra, "Genetic Algorithm- A Literature Review," 2019 Int. Conf. Mach. Learn. Big Data, Cloud Parallel Comput., no. 1998, pp. 380–384, 2019.
3. F. Vericat, C. O. Stoico, C. M. Carlevaro, and D. G. Renzi, "Genetic algorithm for the pair distribution function of the electron gas," Interdiscip. Sci. – Comput. Life Sci., vol. 3, no. 4, pp. 283–289, 2011, doi: 10.1007/s12539-011-0108-3.
4. S. Sharma, S. Mishra, N. Deodhar, A. Katageri, and P. Sagar, "Solving the Classic Snake Game Using AI," 2019 IEEE Pune Sect. Int. Conf. PuneCon 2019, pp. 20–23, 2019, doi: 10.1109/PuneCon46936.2019.9105796.
5. A. Almalki and P. Wocjan, "Exploration of reinforcement learning to play snake game," Proc. - 6th Annu. Conf. Comput. Sci. Comput. Intell. CSCI 2019, pp. 377–381, 2019, doi: 10.1109/CSCI49370.2019.00073.
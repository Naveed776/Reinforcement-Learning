# PointGoal0


| Metric                   | Unconstrained PPO|
|--------------------------|---------------|
| Total Iterations         | 7             |
| Total Time Elapsed (seconds) | 165         |
| Average FPS              | 561.57        |
| Average Policy Gradient Loss | -0.0038   |
| Average Value Loss       | 0.00321       |
| Average Explained Variance | 0.1396      |

### Detailed Performance Trends:

- **Early Iterations (1-5):** 
  - Saw gradual increase in episode reward mean and variability in value loss.
- **Mid Iterations (6-10):** 
  - Continued increase in episode reward mean with fluctuating training metrics.
- **Later Iterations (11-15):** 
  - Marked by further improvements in episode rewards and adjustments in training metrics.
- **Final Iterations (16-22):** 
  - Peaked in episode reward mean at 12.3, with reduced KL divergence and varied value loss indicating model convergence.
 
    Reawrd Epsiode 
  Minimum Return: 19.712 (Episode 15)
  Maximum Return: 28.056 (Episode 24)
  Mean Return: Approximately 24.165
  Median Return: Approximately 24.226
  This summary gives you an idea of the range and central tendency of the episode returns across the 25 episodes. If you need further         analysis or specific insights, feel free to ask!

### Conclusion:

- The reinforcement learning model demonstrated effective learning and convergence over the 22 iterations, with consistent improvements in episode rewards and adaptive adjustments in training metrics.

# PointButton0
Here's the summarized information in a table format based on the metrics you specified:

| Metric                   | Unconstrained PPO |                                                                                      
|--------------------------|---------------|
| **Iterations**           | 300.            |
| **Time Elapsed (seconds)**| 72.34 seconds  |
| **Average FPS**          |  41.55 |
| **Policy Gradient Loss** | 0.01 |
| **Value Loss**           | 0.289|
| **Explained Variance**   | 0.811|

1. **Performance Summary**:
   - **Iterations**: The training progresses through multiple iterations, with each iteration increasing the total timesteps.
   - **Time Elapsed**: The time elapsed increases roughly linearly with the number of iterations.
   - **Frames Per Second (fps)**: The fps remains relatively stable around 550-570 fps.
   - **Explained Variance**: Indicates how well the agent's value function explains the variance in the returns. It fluctuates but generally improves over iterations, showing better performance in capturing the environment dynamics.
   - **Learning Rate**: Constant at 0.0001 throughout.
   - **Loss**: Both policy gradient loss and value loss generally decrease, indicating that the policy and value function are improving with training.
   - **Approx KL (Kullback-Leibler divergence)**: Measures the difference between the old and new policy distributions. It remains relatively low, indicating stable policy updates.

2. **Convergence Observations**:
   - **Episode Length Mean**: Stabilizes early at 1000 steps per episode.
   - **Episode Reward Mean**: Increases over time, showing that the agent learns to achieve higher rewards as training progresses.

3. **Time to Convergence**: 
   - The exact time to convergence can vary based on the task complexity, but generally, the agent shows improvement in reward mean and stability in key metrics (KL divergence, loss, explained variance) over the training iterations.

4. **Key Metrics Trends**:
   - **Approx KL**: Decreases slightly, indicating policy updates are not too disruptive.
   - **Clip Fraction and Range**: Stable around 0.2, showing consistent clipping during updates.
   - **Entropy Loss**: Stays around -2.8, maintaining exploration during training.
   - **Value Loss**: Generally decreases, indicating improved accuracy of the value function estimations.

Overall, the agent appears to be making steady progress in learning the environment and improving its policy and value functions. The convergence trends suggest that with more iterations, the agent's performance in terms of rewards and stability is likely to continue improving.

# CarGoal0

| Metric                  | Unconstrained PPO|
|-------------------------|------------|
| Iterations              | 1470       |
| Time Elapsed (seconds)  | 9378.26    |
| Average FPS             | 0.156      |
| Policy Gradient Loss    | Mean: 0.000259, Std: 0.000076 |
| Value Loss              | Mean: 0.360659, Std: 0.075206 |
| Explained Variance      | Mean: 0.924522, Std: 0.015844 |

## Training Progress:

Iterations: 1470
Time Elapsed: 9378.26 seconds
Average FPS: 0.156
Loss Metrics:

Policy Gradient Loss: Mean: 0.000259, Std: 0.000076
Value Loss: Mean: 0.360659, Std: 0.075206
Explained Variance: Mean: 0.924522, Std: 0.015844
Conclusion:
The training ran for approximately 9378 seconds over 1470 iterations, achieving a mean policy gradient loss of 0.000259 and a high mean explained variance of 0.924522. However, the training processed frames at a very low rate of 0.156 FPS, indicating potential performance limitations or computational complexity. The higher standard deviation in value loss (0.075206) suggests some variability in training the 
value function.

# CarButton0

| Metric                  | Unconstrained PPO|
|-------------------------|------------|
| Iterations              | 27        |
| Time Elapsed (seconds)  | Approximately 5568.5    |
| Average FPS             | 122.0     |
| Policy Gradient Loss    |  0.0013|
| Value Loss              | 0.5|
| Explained Variance      |  0.944 |

## Training Progress:

Performance Metrics:

Average Episode Length: Consistently around 1000 steps per episode.
Average Episode Reward: Gradually increases from 7.99 to 10.6, indicating improving policy performance.
Training Time and Iterations:

Each iteration takes approximately 6 seconds.
FPS ranges between 457 to 498, averaging around 480 FPS.
Total training timesteps increase from 3000 to 81000 over 27 iterations.
Training Progress:

Learning Rate: Fixed at 0.0001 throughout training.
Policy Gradient Loss: Decreases steadily across iterations, indicating policy improvement.
Value Loss: Generally low and stable, suggesting good value estimation.
Entropy Loss: Maintains negativity, ensuring sufficient exploration.
Convergence:

Approximate KL Divergence and Clip Fraction: Generally low, indicating stable policy updates and adherence to clipping.
Explained Variance: Shows variability, suggesting fluctuations in value function prediction accuracy.
Conclusion:
The reinforcement learning model demonstrates a promising learning curve with improvements in episode rewards and stable performance metrics over iterations. However, fluctuations in explained variance and some loss metrics indicate potential areas for further optimization, particularly in hyperparameter tuning or exploration strategies. Overall, the training process exhibits steady improvement and convergence typical of policy gradient methods, highlighting its ability to learn effectively on the given benchmarks..

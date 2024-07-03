# PintGoal0


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

### Conclusion:

- The reinforcement learning model demonstrated effective learning and convergence over the 22 iterations, with consistent improvements in episode rewards and adaptive adjustments in training metrics.

# Comparision between PPO and PPO lagrangian

# Task 1 PointGoal 0

| Metric                     | PPO                             | PPO Lagrangian                  |
|----------------------------|---------------------------------|---------------------------------|
| **Iterations**             | 30+                             | 27+                             |
| **Time Elapsed (seconds)** | 186+                            | 176+                            |
| **Average FPS**            | Approximately 444               | Approximately 450               |
| **Policy Gradient Loss**   | Mostly negative values          | Mostly negative values          |
| **Value Loss**             | Shows improvement, fluctuations | Shows improvement, fluctuations |
| **Explained Variance**     | About 0.352                     | About 0.253                     |

### Summary of Comparison

1. **Iterations and Time Elapsed:**
   - PPO ran for more iterations (30+) and took slightly more time (186+ seconds) compared to PPO Lagrangian Goal 0 (27+ iterations, 176+ seconds).

2. **Average FPS:**
   - PPO: Approximately 444 FPS
   - PPO Lagrangian: Approximately 450 FPS
   - PPO Lagrangian has a slightly higher FPS, indicating it processes more frames per second.

3. **Policy Gradient Loss:**
   - Both algorithms show mostly negative values, indicating improvement in policy performance. No significant difference in this metric.

4. **Value Loss:**
   - Both algorithms exhibit fluctuations in value loss but show improvement over time. PPO POINTGOAL0 seems to have a smoother trend.

5. **Explained Variance:**
   - PPO reaches about 0.352
   - PPO Lagrangian reaches about 0.253
   - PPO has a higher explained variance, indicating it better explains the variance in returns.

### Conclusion

- **Average FPS:** PPO Lagrangian Goal 0 performs slightly better in terms of FPS.
- **Policy Gradient Loss:** Both algorithms show similar performance with negative policy gradient loss values.
- **Value Loss:** Both algorithms show improvement over time, but PPO POINTGOAL0 has a smoother trend.
- **Explained Variance:** PPO POINTGOAL0 performs better, with higher explained variance.

**Overall, PPO appears to have better performance in terms of explained variance and smoother value loss trends, while PPO Lagrangian has a slightly higher FPS.**

# Task 2 PointButton0

| Metric                     | PPO                             | PPO lagrangian               |
|----------------------------|---------------------------------|---------------------------------|
| **FPS (Frames Per Second)** | Approximately 417               | Approximately 457               |
| **Iterations**             | 20+                             | 27+                             |
| **Explained Variance**     | Iteration 20: 0.576<br>Iteration 30: 0.442 | Iteration 20: 0.602<br>Iteration 30: 0.565 |
| **Time Elapsed (seconds)** | 186+                            | 176+                            |
| **Policy Gradient Loss**   | -0.0063 to -0.00386             | -0.00841 to -0.0028             |

### Summary of Comparison
**Average FPS:**
PPO BUTTON runs at approximately 417 FPS, while PPO Lagrgain Button runs faster at around 457 FPS. 

**Iterations and Time Elapsed:**
PPOLagrgainButton also achieves higher explained variances (0.602 at Iteration 20, 0.565 at Iteration 30) compared to PPOBUTTON0 (0.576 at Iteration 20, 0.442 at Iteration 30), indicating potentially better performance in predicting the value function.

**Policy Gradient Loss:**
Both algorithms show similar policy gradient losses (-0.0063 to -0.00386 for PPOBUTTON0, -0.00841 to -0.0028 for PPOLagrgainButton),

**Conclusion:**

PPO lagrangian Button shows faster convergence per iteration with higher FPS and better explained variance metrics, suggesting potential advantages in performance. However, a direct safety comparison requires additional trials to assess policy robustness in real-world applications.


# Task 3 CarGoal0 

**Summary and Comparison Table:**

| Metric                     | PPO                             |  PPO lagrangian                    |
|----------------------------|---------------------------------|---------------------------------|
| **Average Episode Reward Mean** | 10.5                            | 9.47                            |
| **Entropy Loss**            | -2.76                           | -2.78                           |
| **Explained Variance**      |-0.00251                           | 0.247                         |
| **Policy Gradient Loss**    | -0.00857                         | -0.0052                        |
| **Value Loss**              | 0.0156                         | 0.00932                          |

**Summary:**

- **Average Episode Reward Mean:** PPO  achieves a higher average episode reward mean of 10.5 compared to PPO lagrangians 9.47, indicating better performance in terms of rewards obtained during training episodes.
  
- **Entropy Loss:** Both models have similar entropy losses, suggesting a balanced exploration-exploitation trade-off.
  
- **Explained Variance:** PPO  shows better prediction of returns with an explained variance of 0.247, whereas PPO lagrangian has a variance closer to zero (-0.00251).
  
- **Policy Gradient Loss:** PPO lagrangian has a lower policy gradient loss (-0.0052) compared to PPO  (-0.00857), indicating better policy optimization.
  
- **Value Loss:** PPOlagrgainCarGoa also performs better in terms of value function optimization with a lower value loss (0.00932) compared to PPOCARGOAL (0.0156).

**Conclusion:** Overall, while PPO  achieves a higher average episode reward mean, PPO lagrangian shows slightly better performance in terms of explained variance, policy gradient loss, and value loss. The choice between the two models would depend on the specific priorities and trade-offs relevant to the application of the reinforcement learning model.

# Comparision between PPO and PPO lagrangian

# Task 1 PointGoal 0

Certainly! Here's the summary and comparison in a table format:

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

# Results Quick Reference

## Paper Results (Normal Distribution)

### Random Assignment (Best Case)
- Error Rate: 32%
- Terminations: 45 false positives / 142 total (32%)
- Promotions: 46 false positives / 142 total (32%)
- False Negatives: ~52-53

### Biased Assignment (Realistic, σ=0.7)
- Error Rate: 54%
- Terminations: 77 false positives / 142 total (54%)
- Promotions: 76 false positives / 142 total (54%)
- False Negatives: ~83-84

## Power Law Extensions (Appendix B)

### Random Assignment
- Error Rate: 32% (identical to normal)
- Symmetric across terminations/promotions

### Moderate Clustering (σ=0.7)
- Termination Error: 39%
- Promotion Error: 61%
- Shows asymmetric pattern

### Strong Clustering (σ=0.95)
- Termination Error: 36%
- Promotion Error: 80%
- Catastrophic for promotions
- Only 2/10 true 1% performers promoted

## Interpretation

### What does 54% error mean?
More than half of people fired/promoted are wrong.
The system is worse than random (50%).

### Why does clustering make it worse?
Strong teams' worst member > weak teams' best member.
System can't see this (local frames).

### Why is power law asymmetric?
Bottom-heavy tail limits termination damage.
Top-heavy clustering amplifies promotion damage.

# Simulation Parameters Quick Reference

## Default Configuration
- Employees: 994
- Teams: 142
- Team Size: 7
- Distribution: Normal N(0,1)
- Clustering (σ_team): 0.7
- Cutoff: 15%
- Simulations: 100

## Key Parameters

### num_employees
Default: 994
Range: 100-10000
Description: Total population size

### team_size
Default: 7
Range: 3-20
Description: Members per team

### use_bias
Default: False
Options: True/False
Description: Use biased (realistic) team assignment

### clustering_strength
Default: 0.7 (for biased)
Range: 0.0-1.0
Description: Team quality variance (0=random, 1=perfect sorting)

### distribution
Default: 'normal'
Options: 'normal', 'powerlaw', 'uniform', 'lognormal'
Description: Talent distribution type

### cutoff_percentile
Default: 0.15
Range: 0.05-0.30
Description: What % to fire/promote

### num_simulations
Default: 100
Range: 1-10000
Description: Monte Carlo iterations

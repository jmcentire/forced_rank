# Usage Examples

## Basic Usage
```python
from forced_rank import run_simulation

# Run random assignment scenario
results = run_simulation(use_bias=False, num_simulations=100)
print(f"Error rate: {results['mean_error_rate']:.1%}")
```

## Compare Scenarios
```python
from forced_rank import compare_scenarios

results = compare_scenarios(num_simulations=100)
print(results['comparison_table'])
```

## Custom Parameters
```python
from forced_rank import Simulation

sim = Simulation(
    num_employees=1000,
    team_size=10,
    clustering_strength=0.5,
    distribution='powerlaw'
)

results = sim.run(num_simulations=100)
sim.plot_results()
```

## Sensitivity Analysis
```python
from forced_rank import sensitivity_analysis

results = sensitivity_analysis(
    param='clustering_strength',
    values=[0.0, 0.3, 0.5, 0.7, 0.9],
    num_simulations=100
)
```

## Power Law Analysis
```python
from forced_rank.powerlaw import run_powerlaw_analysis

results = run_powerlaw_analysis(
    clustering_levels=[0.0, 0.7, 0.95],
    analyze_asymmetry=True
)
```

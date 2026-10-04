# Findings Documentation + Visualization — Assumption Transparency

**Core Responsibility Demonstrated:** Creating visualizations and findings documentation with explicit assumptions and honest discussion of confidence levels.

## What This Does

1. **Assumptions Document**: Lists every assumption the analysis depends on (upfront, in JSON)
2. **Visualizations**: 4-panel figure showing data, trend, residuals, and confidence by finding type
3. **Limitations List**: Caveats (extrapolation risk, unknown causation, small sample, outliers)
4. **Confidence Breakdown**: Not all findings equally believable—trend direction HIGH, point forecasts LOW

## Run It

```bash
pip install -r requirements.txt
python main.py
```

**Output:**
- Console: Full findings report
- `findings.png`: 4-panel visualization
- `assumptions.json`: All model assumptions
- `limitations.json`: Honest caveats
- `report.txt`: Complete analysis write-up

## Key Insight

The visualization distinguishes confidence levels. Trend direction is clear (95% confidence). Point predictions are risky (55% confidence). Report explicitly states what we don't know (causation) and what could break our conclusions (nonlinear behavior, longer time window).

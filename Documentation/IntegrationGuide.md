# Integration Guide

## Integration model

Assessment subscribes to training lifecycle events and evaluates outcomes without controlling training flow.

Incoming events:

- `xr.training.step.started`
- `xr.training.step.completed`
- `xr.training.step.failed`
- `xr.training.scenario.completed`
- `xr.training.validation.failed`

Outgoing events:

- `xr.assessment.score.updated`
- `xr.assessment.failed`
- `xr.assessment.passed`
- `xr.assessment.completed`
- `xr.assessment.report.generated`

## Recommended production flow

1. Build and validate scenario in Training Toolkit.
2. Attach assessment profile per scenario.
3. Tune score/penalties/limits per competency target.
4. Run success and fail-case QA passes.
5. Ship with report export enabled.


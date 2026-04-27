# Event Contract

## Contract Version

- `1.0.0`

## Incoming (Training -> Assessment)

- `xr.training.step.started` (`ScenarioId`, `StepId`)
- `xr.training.step.completed` (`ScenarioId`, `StepId`)
- `xr.training.step.failed` (`StepId` or resolvable target)
- `xr.training.scenario.completed` (`ScenarioId`)
- `xr.training.validation.failed` (`StepId` or resolvable target)

## Outgoing (Assessment -> Consumers)

- `xr.assessment.score.updated` (`SessionId`, `CurrentScore`, `MaxScore`)
- `xr.assessment.failed` (`SessionId`, `Reason`)
- `xr.assessment.passed` (`SessionId`, `FinalScore`)
- `xr.assessment.completed` (`SessionId`, `Passed`, `FinalScore`)
- `xr.assessment.report.generated` (`SessionId`, `Report`)

## Report Schema Notes

Report payload supports:

- schema and package identifiers
- score and result
- time and step statistics
- mistakes and failure-limit metadata
- session/scenario/profile/build identifiers


# XRCore Training Assessment

![Unity](https://img.shields.io/badge/Unity-2022%2B%20%7C%20Unity%206-black)
![Category](https://img.shields.io/badge/Category-AI%20%2F%20XR%20Training-1f6feb)
![Package](https://img.shields.io/badge/Package-com.xrcore.training.assessment-7a3cff)
![Architecture](https://img.shields.io/badge/Architecture-Event--Driven-0ea5e9)
![License](https://img.shields.io/badge/License-MIT-84cc16)

Validate, score, and certify XR training performance with measurable outcomes.

XRCore Training Assessment is the evaluation and scoring layer for Unity XR training workflows built on top of XRCore SDK and XRCore Training Toolkit.

Where XRCore provides event-driven XR intelligence and Training Toolkit provides guided scenario execution, Assessment adds measurable performance validation: score, pass/fail decisions, critical-failure detection, and exportable reports.

## Demo

- Recommended demo flow:
  1. Look at target.
  2. Grab object.
  3. Place object.
  4. View final pass/fail summary and exported report.

## Why XRCore Training Assessment

Most XR training demos can show that the flow ended, but they cannot prove that the trainee performed correctly.

This package solves that gap by converting guided execution into measurable outcomes:

- weighted scoring per step,
- configurable penalties,
- mandatory-step enforcement,
- critical-failure rules,
- report generation for audit and QA.

## Relationship with XRCore Ecosystem

This package is intentionally distributed as an extension layer:

- **XRCore SDK** provides:
  - event bus and modular runtime systems,
  - XR interaction and perception architecture,
  - reusable agent/task foundation.
- **XRCore Training Toolkit** provides:
  - scenario and step orchestration,
  - validator-driven progression,
  - guided training UX.
- **XRCore Training Assessment** adds:
  - scoring and evaluation logic,
  - competency/pass-fail decisions,
  - assessment diagnostics,
  - exportable final reports (JSON/CSV).

## XRCore Ecosystem Links

- Built on top of XRCore SDK: [xrcore-sdk](https://github.com/splibiplay/xrcore-sdk)
- Works with XRCore Training Toolkit: [xrcore-training-toolkit](https://github.com/splibiplay/xrcore-training-toolkit)
- Assessment package repository: [xrcore-assessment](https://github.com/splibiplay/xrcore-assessment)
- Unity Asset Store publisher page: [SPL Publisher](https://assetstore.unity.com/publishers)

## Video Demos

- SDK demo: _coming soon_
- Toolkit demo: _coming soon_
- Assessment demo: [XRCore Training Assessment Demo](https://youtu.be/MpAfoV2tRJY)

## Key Features

- Event-driven assessment runner (`XRTrainingAssessmentRunner`)
- Designer-friendly profile system (`XRAssessmentProfile`)
- Weighted step rules and penalties
- Maximum mistakes / consecutive-failure auto-fail thresholds
- Critical failure handling
- Runtime guard and diagnostics overlay
- Setup Wizard with validate/fix workflow
- Report export:
  - JSON
  - CSV

## Architecture Overview

```
XRCore + Training Events
          ↓
XRTrainingAssessmentRunner
          ↓
Score / Rule Evaluation
          ↓
Pass-Fail + Report Generation
          ↓
JSON / CSV Export
```

## Main Components

- `XRTrainingAssessmentRunner`
- `XRAssessmentProfile`
- `XRStepAssessmentRule`
- `XRStepScoreEvaluator`
- `XRTrainingReport`
- `XRTrainingAssessmentRuntimeGuard`
- `XRTrainingAssessmentHealthOverlay`
- `XRTrainingAssessmentSetupWindow`

## Setup Wizard

Unity menu:

`Tools -> XRCore Training Assessment -> Setup Wizard`

Core actions:

- Validate
- Auto-Fix Scene
- Generate Profile From Selected XRTrainingScenario
- Export Diagnostics Snapshot

## Report Contract (v1)

`XRTrainingReport` includes:

- schema version
- final score / max score
- completion time
- mistakes and failure counters
- critical failures
- pass/fail result
- timestamps and identifiers

## Requirements

- Unity 2022+ or Unity 6
- XRCore SDK
- XRCore Training Toolkit

## Documentation

- `Documentation/QuickStart.md`
- `Documentation/IntegrationGuide.md`
- `Documentation/EventContract.md`

## License

XRCore Training Assessment is distributed under the MIT License. See `LICENSE`.


# QuickStart

## 1) Install dependencies

- Install/import XRCore SDK.
- Install/import XRCore Training Toolkit.
- Install/import XRCore Training Assessment.

## 2) Create assessment profile

- Create `XRAssessmentProfile`.
- Configure pass score, weighted rules, and mistake limits.

## 3) Add runtime components

- Add `XRTrainingAssessmentRunner` to scene.
- Assign assessment profile.

## 4) Validate setup

Open:

`Tools -> XRCore Training Assessment -> Setup Wizard`

Run:

- Validate
- Auto-Fix Scene (if needed)

## 5) Run demo and export

- Play your training scenario.
- Complete/fail steps to verify pass/fail logic.
- Check exported reports under:
  - `Application.persistentDataPath/XRTrainingAssessmentReports`


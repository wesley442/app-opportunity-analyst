# Validate App Idea

Use the `app-opportunity-analyst` skill to validate one existing app idea before building.

## Input

```text
Validate idea: <one-sentence app idea>
Target user: <optional>
Platform: <optional>
Constraints: <optional>
```

## Instructions

1. Restate the idea and the assumptions that must be true.
2. Search for direct and adjacent competitors.
3. Gather evidence for demand, willingness to pay, competition, and distribution.
4. Identify reasons the idea might fail.
5. Score the idea using `references/scoring-rubric.md`.
6. Recommend the smallest validation test before development.

## Output

Use `templates/validation-report.md`.

## Example

```text
Validate idea: a calendar app that uses AI to turn messy voice notes into scheduled tasks.
Target user: busy freelancers
Platform: iOS
Constraints: solo developer, 10-day MVP
```

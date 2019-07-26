# rush-issue-add-project
Example Microsoft Rush project that exhibits an issue while adding a new project.

# Repro steps
1. Clone repo
2. `rush install`
3. Uncomment the "project-b" project in `rush.json`
4. `rush update`

## Expected
Rush updates the shrink wrap with the new project.

## Actual
Rush produces this error:
```
ERROR: Cannot get dependency key for temp project: @rush-temp/project-b
```

<!--- These lines are template instructions, you do NOT need to delete them. -->
<!--- Go over all the following sections and checklists (put an `x` in all the boxes that apply. -->

<!--- Provide a general summary of your changes in the Title above -->

## Description, Motivation and Context (link issue)
<!--- Provide a clear summary of what this PR does and why. -->
<!--- Why is this change required? What problem does it solve? -->
<!--- If it fixes an open issue, please link to the issue here. -->

## Types of changes
<!--- What types of changes does your code introduce? Put an `x` in all the boxes that apply: -->
- [ ] Bug fix (non-breaking change which fixes an issue)
- [ ] New feature (non-breaking change which adds functionality)
- [ ] Refactoring (no functional changes)
- [ ] Documentation update
- [ ] Infrastructure / CI/CD
- [ ] Performance improvement

## Contributing Checklist
- [ ] My code follows the code style of this project
- [ ] I have read the **CONTRIBUTING** document.

## Documentation Checklist

### General:
- [ ] Updated `README`

### R software package:
- [ ] Ran `devtools::document()` to update `docs/`
- [ ] Ran `attachment::att_amend_desc()` to auto-sync function imports and DESCRIPTION
- [ ] Updated `CHANGELOG.md` (include this PR number) 

## Testing Checklist
<!--- Please describe in detail how you tested your changes. -->
<!--- Include details of your testing environment, and the tests you ran to -->
<!--- see how your change affects other areas of the code, etc. -->

### General:
- [ ] Self-reviewed the code for obvious errors
- [ ] Added or updated tests/data checks/assumption warnings where applicable
- [ ] No new warnings or console errors introduced

### R software package:
- [ ] Ran `devtools::test()` and passed all tests
- [ ] Ran `devtools::check()` with 0 ERRORS | 0 WARNINGS
<!---Describe in detail any remaining `check()` WARNINGS -->

### Regression Risk
<!-- Could this fix break anything else? -->

## PR Review & Prep Merge Checklist (GitFlow rebasing workflow)

- [ ] All branches up-to-date (*e.g.* `main`, `develop`, `develop-<feature-name>`)
```
git checkout develop
git pull develop
```
- [ ] Switch back to `feature-branch`
```
git checkout <feature-branch>
```
- [ ] Rebase `feature-branch` onto `develop` branch
```
git rebase develop
```
- [ ] Resolved all merge conflicts
- [ ] Run `devtools::check()` again - 0 ERRORS | 0 WARNINGS
- [ ] Fixed any ERROR or WARNINGS - committed - rebase again onto target branch
```
git add .
git commit -m "fixed <...> from rerunning devtools::check()"
git rebase develop
```
- [ ] Push rebased branch to origin - requires a force push after rebase
```
git push origin <feature-branch> --force
```
- [ ] All automated checks pass (scroll down below PR to see results if this is configured)
- [ ] Tagged PR Reviewer to the left & message them directly about the PR review

## Screenshots (if appropriate):
<!-- If applicable, add screenshots or screen recordings. -->

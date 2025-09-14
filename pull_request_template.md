## Pull Request Template for Salesforce Development

### Description
Please include a summary of the change and the related issue.  
- What feature/bug does this PR address?  
- Why is this change required?  
- Any background context?

---

### Checklist (Pre-Submission by Developer)

#### Code Quality
- [ ] Code follows project style guidelines (naming conventions, indentation, comments).
- [ ] No hardcoded IDs, credentials, or org-specific logic.
- [ ] Apex classes, triggers, and LWC components are bulkified and governor-limit safe.
- [ ] No `System.debug()` statements left in code unless required for logging.

#### Testing
- [ ] Apex unit tests are written with meaningful assertions.
- [ ] Minimum **75% coverage** achieved on new/modified Apex classes.
- [ ] Tests cover bulk scenarios and error-handling cases.
- [ ] LWC Jest tests updated/added for new components (if applicable).
- [ ] All tests pass locally before raising the PR.

#### Deployment Integrity
- [ ] Validated sfdx deployment (or package build) completed without errors.
- [ ] Code deploys cleanly to a scratch org / sandbox environment.
- [ ] No missing metadata (all referenced fields, objects, permissions included).
- [ ] Profiles/Permission Sets are minimized to least privilege necessary.

#### Documentation
- [ ] Added/updated inline code comments for complex logic.
- [ ] Updated README / technical design doc (if necessary).
- [ ] User-facing changes documented (labels, flows, config notes).

#### Reviews / Approvals
- [ ] Linked related Issue ticket(s).
- [ ] Requested review from at least one team member. @mention user to review PR.
- [ ] Added screenshots/GIFs for UI-related changes (LWCs/Visualforce updates).

---

### Additional Notes
Provide any additional information reviewers should know (e.g., special data setup, dependencies, sequence of deployment, rollback plan).

<!--
Authors: Please fill out this form carefully and completely. If you're new to deploying `github/github` please read the https://thehub.github.com/engineering/development-and-ops/deployment/deploying-dotcom/
-->

_**Reviewers:** Please read this description carefully. By approving this pull request you are approving its deployment and mitigation plans as well as the code change. If you feel there is anything unclear or missing, please ask for updates._

### Issues affected by this change

<!--
Every code change must address _at least 1_ issue. Fixes a bug, completes a task, every change should have a corresponding issue listed here. If one does not already exist, create one.

If this work is related to a feature release, add a link to the `github/releases` issue. ALL feature releases, even small features, should have a release issue. For more info, see the README: https://github.com/github/releases#readme

Format the issue(s) listed here with a markdown list so that each title unfurls automatically e.g.

- Closes [Link to issue here].
-->

### What are you trying to accomplish?

<!--
Provide a description of the changes, including any screenshots, videos, or graphs if applicable.
-->

### What approach did you choose and why?

<!--
This section is a place for you to describe your thought process in making these changes:

  - List any tradeoffs you made to take on or pay down tech debt.
  - Identify any work you did to mitigate risk.
  - Describe any alternative approaches you considered and why you discarded them.
-->

### Anything you want to highlight for special attention from reviewers?

<!--
This is your chance to identify remaining risks and confess any uncertainties you may have about the correctness of the changes:

  - Highlight anything on which you would like a second (or third) opinion.
  - Keep in mind how much traffic will be affected by your changes when assessing risk.
-->

### Which environments does this change target?

<!--
Which environments does this change impact? Select or unselect all that apply.

If it is a Production change and you have unselected any combination of dotcom, proxima or GHES

Please leave a brief explanation of why and how this change does not apply to those environments.
-->

- [x] Production
  - [x] dotcom
  - [x] proxima
  - [x] GHES
  - [ ] GHAE
- [ ] Non-production
  - [ ] dev/test
  - [ ] docs

### Risk Assessment

<!--
Please select from one of the following and detail why this level was chosen.

For more details on risk assessment, check out:

https://thehub.github.com/engineering/products-and-services/dotcom/pr-risk-and-rollout-review/#evaluate-the-pr-for-the-level-of-risk-it-presents
-->

- [ ] **Low risk** the change is fully under one or more Feature Flags OR the modifications are small, highly observable, and easily rolled back.
- [ ] **Medium risk** changes that are isolated, reduced in scope or could impact few users and not bring the site down.
- [ ] **High risk** changes are those that could impact our customers and SLOs, low or no test coverage, low observability, or slow to rollback.

### Feature Flags

<!--

Most production changes should be protected by one or more Feature Flags.

Please link the Feature Flag Rollout issues for each Feature Flag below.

If you need to create a Feature Flag Rollout issue, follow this link: https://github.com/github/github/issues/new?template=feature_flag_rollout.md&title=%5BFF%5D+.

If this is a production change and it _does not_ have a Feature Flag, briefly explain why here.

If this is a non-production changes simply enter N/A.
-->

### If something goes wrong, what are the mitigation and rollback strategies?

<!--
Common deployment risk mitigation strategies are listed below.

Delete all those that don't apply.

Describe your plans if they don't fit into any of these buckets.

For details on the expectations for rollout/rollback contingency planning, please see:

https://thehub.github.com/engineering/products-and-services/dotcom/pr-risk-and-rollout-review/#evaluate-the-pr-for-the-level-of-risk-it-presents
-->

* ### **Unknown** - **I forgot to update this section and don't have a mitigation strategy.**
* **Experiment** - Change will be tested with an experiment, but will need to be rolled back if the experiment does not work. Please link to the relevant experiment below.
* **Solo Deploy** - This change will be deployed solo, making it easier to monitor impact and revert if necessary. Solo deploys should be used sparingly since they prevent others from shipping with you.
* **Feature Flag** - Change can be disabled by feature flag, but will need to be rolled back if the feature flag does not work. Please link to the relevant feature flags below.
* **Review Lab Deploy** - This change will be tested on review-lab before being queued to deploy.
* **Rollback** - Change can only be disabled by [rolling back](https://ops.githubapp.com/docs/playbooks/github_deployments.md) the merge group, or by deploying a revert commit.

### Accessibility

<!--
You may remove this section and the "Accessibility" heading above _only_ if the changes in this pull request do not impact UI. Delete all those that don't apply.

If there are any accessibility-related updates, please describe them here. Questions? Ping us in the #accessibility" channel.
-->

* **Fixes axe scan violation** - This change fixes an existing [axe scan](https://thehub.github.com/epd/engineering/dev-practicals/frontend/accessibility/readiness-routine/development/#axe-scans) violation.
* **No new axe scan violation** - This change does not introduce any new [axe scan](https://thehub.github.com/epd/engineering/dev-practicals/frontend/accessibility/readiness-routine/development/#axe-scans) violations.
* **New axe violation** - This change introduces a new [axe scan](https://thehub.github.com/epd/engineering/dev-practicals/frontend/accessibility/readiness-routine/development/#axe-scans) violation. Please describe why the violation cannot be resolved below.

### Observability

<!--
If you have observability resources for this change other than the deployment dashboard and sentry, please link them here. Otherwise delete this comment and the "Observability" header above.

Examples might include custom graphs, dashboards, or EXPLAIN statements.
-->

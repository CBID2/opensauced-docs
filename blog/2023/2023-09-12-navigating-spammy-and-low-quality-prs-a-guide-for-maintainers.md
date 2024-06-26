---
title: "Navigating Spammy and Low-Quality PRs: A Guide for Maintainers"
tags: []
authors: BekahHW
slug: navigating-spammy-and-low-quality-prs-a-guide-for-maintainers
description: "Maintainers time is a valuable and finite asset. This guide defines spammy and low-quality PRs and gives maintainers tips on how to defend against them."
---


Open source maintainers are the ultimate utility players, reviewing code, managing community dynamics, defining strategy, writing code, and more. One of the most time-consuming tasks is reviewing Pull Requests (PRs), especially those that are spammy or of poor quality. And although contributors might not realize it, poor-quality contributions can be incredibly costly. So how can maintainers reduce spam and improve the quality of PRs?

<!-- truncate -->

## The Cost of Poor-Quality & Spammy PRs
### Poor-Quality PRs
> Poor-quality PRs may have good intentions but lack the necessary quality, completeness, or adherence to project guidelines. These PRs often require substantial revisions and are not immediately mergeable.

**Examples of poor-quality PRs include:**
- Incomplete: The PR may contain code that isn’t fully implemented or is broken, leading to failed tests. It also may not follow the contributing guidelines, leading to necessary steps being skipped.
- Lack of Documentation: The PR lacks comments, README updates, or inline documentation to explain the changes.
- Code Style Violations: The submitted code doesn’t adhere to the project's coding standards or style guide.
- No Issue Reference: The PR does not reference any existing issue or explain why the change is necessary, making it hard to understand the context.
- Blank PR template: Assuming there are PR templates, the contributor ignores all or part of the template, leaving the maintainer without the information they need to review the PR.
- Large and Unfocused: The PR tries to address multiple issues at once, making it difficult to review and test.

### Spammy PRs
> Spammy PRs appear to be made with little to no genuine intent to contribute to the project meaningfully. These are often created to take advantage of programs like Hacktoberfest or to simply gain contributor credits.

**Examples of Spammy PRs include:**
- "Hello, World!" Contributions: The PR adds a "Hello, World!" print statement or comment that has no relevance to the project.
- Whitespace Changes: The PR consists only of whitespace changes like adding/removing blank lines or spaces, without any meaningful code changes.
- Duplicate PRs: The same PR is submitted multiple times without any new changes.
- Irrelevant File Additions: The PR includes files that are irrelevant to the project.
- Automated Submissions: The PR appears to be generated by a bot and contains generic or templated changes that are not project-specific.

Each PR requires time and effort to review, and when they aren’t up to standard, they drain maintainer resources that could be better spent elsewhere. I find it helpful to have an overview of what types of PRs are included in my projects to help me best manage my time and filter out low-quality PRs.

[![OpenSauced Insights page](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/tuaahg2yptfdvblybto0.png)](https://insights.opensauced.pizza/pages/BekahHW/230/dashboard)

## Best Practices for Maintainers
1. Set Clear Guidelines
One of the first lines of defense against poor-quality PRs is to set clear contribution guidelines. Make sure to outline what you expect in a PR, including coding standards, commit messages, and documentation. Think of this as a filter, discouraging those who are not willing to meet basic requirements. Along with this, having a clear Code of Conduct can help to prevent repeat or malicious PRs and communication.

2. Use Automated Checks
Leverage technology to automate the initial review process. Tools like GitHub Actions can automatically run tests, check for code style violations, and even flag potential security issues. This can help you weed out problematic PRs before you even look at them.

3. Implement a PR Template
A PR template can guide contributors to provide all the necessary information you need for a review. This can include a checklist for the contributor to mark off before submission, ensuring that they have followed all the guidelines and completed any required tests. You can check out [OpenSauced’s PR template here](https://github.com/open-sauced/.github/blob/main/.github/PULL_REQUEST_TEMPLATE.md).

4. Limit Access
For projects that are prone to spam, consider adding [branch protections](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/managing-a-branch-protection-rule). GitHub allows you to create branch restrictions and even restrict access to only those who have been explicitly given permission, reducing the likelihood of spammy or malicious PRs.

    ![setting up branch protections](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/75x49gmpdwxidcipfg4n.png)

5. Peer Reviews
Encourage peer reviews among contributors before the PR reaches you. This can act as another layer of quality control and encourage collaboration.

6. Be Open to Communication
Maintain an open line of communication with your contributors. If you find that a particular contributor is consistently submitting poor-quality PRs, a direct conversation may be more effective than repeated written feedback.

By setting clear guidelines, leveraging automation, and fostering a culture of quality, you can reduce the time and effort spent on poor-quality PRs. Remember, the goal is not just to reduce spam but to elevate the quality of contributions to your project and to encourage repeat contributions from valued community members.









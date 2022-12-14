## Contributing to Casper - Guideline Document

Welcome! If you are on this page, you are probably interested in contributing to Casper's development, and we are excited to have you here.

Casper truly believes in the strength of community participation and welcomes help in many forms.

We'll always need help improving documentation, creating tutorials, and writing tests. You can help Casper by participating in development, code review, and documentation improvements.

## Code of Conduct
The Casper [Code of Conduct](https://github.com/casper-ecosystem/.github/blob/main/profile/CODE_OF_CONDUCT.md) governs this project and those participating in it.  By participating, you are expected to uphold this code.

## How can I contribute?

### 1. Reporting Bugs

The Casper Ecosystem and Network consist of repositories specific to the Casper Node, SDKs, Contracts and Documentation.

If you notice any bugs, please open an issue in the respective repository. You can choose the appropriate template when opening an issue and fill in the requested details.

When you are creating a bug report, please include as many details as possible. Fill out the required template, the information it asks for helps us resolve issues faster.

**Before Submitting A Bug Report**
- Check the documentation/FAQs for the list of common questions and problems.
- Determine which repository the problem should be reported in.
- Perform a cursory search to see if the problem has already been reported in the respective repo. If it has and the issue is still open, add a comment to the existing issue instead of opening a new one.

> Note: 
> If you find a closed issue that seems like it is the same thing that you're experiencing, open a new issue and include a link to the original issue in the body of your new one.

**How Do I Submit A (Good) Bug Report?**

Bugs are tracked as GitHub issues. After you've determined which repository your bug is related to, create an issue on that repository and provide the following information by filling in the template:

Explain the problem and include additional details to help maintainers reproduce the problem:
- **Use a clear and descriptive title** for the issue to identify the problem.
- **Describe the exact steps which reproduce the problem** in as much detail as possible
- **Provide specific examples to demonstrate the steps**. Include links to files or GitHub projects, or copy/paste-able snippets, which you use in those examples. If you're providing snippets in the issue, use Markdown code blocks.
- **Describe the behavior you observed after following the steps**, and point out what exactly is the problem with that behavior.
- **Explain which behavior you expected to see instead, and why**.


### 2. Code Contribution

There are several ways to identify an area where you can contribute to Casper.

You can take a look at existing issues in our various repositories to see what you can work on. 

If you're interested in working on an issue, we recommend you comment on it so that a maintainer can bring you up to speed, and that others know you are working on it.

If there's something you'd like to work on, but isn't captured by an existing issue, feel free to open an issue within the appropriate public repositories of the [Casper Ecosystem](https://github.com/casper-ecosystem/) to start the discussion.

If you're looking to collaborate and want to find easy tasks to start, look at the issues we marked as `good first issue`.

You can also start by looking through the `beginner` and `help-wanted` issues.

### 3. Casper Documentation

If you need to add or change anything in Casper Documentation, please raise a PR to the `dev` branch. 
>NOTE: Kindly check the sample PR/PR Process in the Pull Requests section.

The Casper [Writing and Editing Style Guide](https://docs.casperlabs.io/workflow/contribute/#overview) aims to establish a set of standards and guidelines for writing and editing Casper documents to provide uniformity and consistency throughout. 

The Writing and Editing Style Guide document briefly discusses the guidelines to be followed in developing the content for each deliverable.

Please follow the specific Writing Style Guides like [Guidelines](https://docs.casperlabs.io/workflow/contribute/#general-guidelines), [Grammar](https://docs.casperlabs.io/workflow/contribute/#grammar), [Verb Agreement](https://docs.casperlabs.io/workflow/contribute/#verb-agreement), [Headings](https://docs.casperlabs.io/workflow/contribute/#headings), [Lists](https://docs.casperlabs.io/workflow/contribute/#lists),  [Tables](https://docs.casperlabs.io/workflow/contribute/#tables), [Images](https://docs.casperlabs.io/workflow/contribute/#images), and [Formatting](https://docs.casperlabs.io/workflow/contribute/#formatting) used by Casper's documentation team to keep the updates consistent. 

Upon successfully submitting the PR, the Casper team will review the PR or reach out accordingly.

### 4. Creating Pull Requests

As a contributor, you are expected to `fork` a repository, work on your own `fork` and then submit a pull request. The pull request will be reviewed and eventually merged into the `main` repo.

**Prerequisites:**

**Step 1**: Create a fork of the `dev` , `feature` or `release-feature` branch to which you want to add your changes.

Please note that the naming convention followed for a Release/Feature branch releases;
- `release-1.4.6` in case of Major releases (e.g. Protocol release)
- `feat-1.5.0` in case of Feature releases

**Step 2:** Clone the forked repository and add code, commit and push

**Step 3:** Enable Automated Testing [Refer GitHub???s [Automating builds and tests - GitHub Docs](https://docs.github.com/en/actions/automating-builds-and-tests)  for more information]

**Step 4:** Verify the tests have been automatically run

- **Step 4.1:** Add a test which reveals a problem

  - **Step 4.1.2:** Open an issue on GitHub

  - **Step 4.1.3:** Fix the broken test and proceed to Step 4.2

**Step 4.2:** Open a Pull Request

**Step 5:** Casper Team will review the Pull Request and Accept if the changes are in line with Casper???s expected code quality, test coverage and security standards

- **Step 5.1:** Git Rules

    We use `gitchangelog` for all of our repos for change logs. For that, we need to adhere to the following convention when writing commit messages. Your pull request may not be merged if you are not following this convention.

- **Step 5.2:** Commit Message Convention

    The following suggestions might be useful to add in your commit messages. You might want to separate your commits into rough sections:
    - by purpose (for example: new, fix, change ...)
    - by the entity (for example: doc, sdk, code ...)
    - by the audience (for example: dev, tester, users ...)
  
    Additionally, you might want to tag some commits:
    - as `minor` commits that shouldn???t get output to your changelog (cosmetic changes, small typo in comments...)
    - as `refactor` if you don???t have any significant feature changes
        Thus, this should not also be part of the changelog displayed to a final user, but might be of some interest if you have a developer changelog.
    - you could also tag with `api` to mark API changes or if it's a new API   
      or similar

Try writing your commit message by targeting user functionality as often as you can. You can also select existing labels/tags available on the repos to categorize your commit message.

**Casper Pull Request Workflow:**

Please refer to the Casper Pull Request Workflow below;

![Casper PR Workflow](https://github.com/casper-ecosystem/.github/blob/main/profile/Casper_Pull%20Request_Flow.png)

- **Step 5.3:** Best Practices
  - Code in the Casper project should meet the style guidelines with sufficient test cases, descriptive commit messages, evidence that the contribution does not break any compatibility commitments or cause adverse feature interactions and evidence of high-quality peer review.
  - Casper recommends small, frequent PRs over large, infrequent ones.
  - When you notice those dependencies, put the fix into a commit of its own, then check out a new branch, and cherry-pick it.
  - Read the PR template prudently and make sure to follow all the instructions.
  - Please pay attention to the maintainer's feedback, since it is a necessary step to keep up with the standards Casper attains.
  - If the feature requires ongoing maintenance (e.g. support for a particular brand of database), we may ask you to accept responsibility for maintaining this feature.



### 5. Testing

If you are interested in testing our documentation, guides and developer tools, head over to the following pages:

- [Why Build on Casper](https://docs.casperlabs.io/dapp-dev-guide/build-on-casper/introduction/)
- [Getting Started with Rust](https://docs.casperlabs.io/dapp-dev-guide/writing-contracts/getting-started/)
- [Setting up a Local Network with NCTL](https://docs.casperlabs.io/dapp-dev-guide/building-dapps/setup-nctl/)
- [Testing Smart Contracts with NCTL](https://docs.casperlabs.io/dapp-dev-guide/building-dapps/nctl-test/)

We would love to know your insights/feedback from your testing. You can let us know by submitting issues in the respective repositories on GitHub.

### 6. Contributing New Projects to Casper Ecosystem

This section is specifically created to explain the mandatory requirements that the Community Developers/Teams are required to follow when contributing new projects to the Casper Ecosystem.

The contributing team is expected to follow the below Open-Source Software Compliance in accordance with the other Casper-specific contributions and standards outlined in the previous sections of this document.

**OSS Compliance Checklist:**

**Must have**
- An OSI-approved OSS license (the LICENSE file)
- README with intro, install, usage, and testing instructions (README.md)

**Recommended having**
- Repo description (on the top right of the repo, with a proper web link, and relevant topics for discoverability)
- Code of conduct (CODE_OF_CONDUCT.md)
- Contribution policy (CONTRIBUTING.md)
- Security policy (SECURITY.md)

**Nice to have**
- Issue templates
- PR template
- Repository admins accept content reports (enabled from the admin settings of the repo)

## Contributing Style Guide

Please follow the Writing Style Guide used by Casper's Documentation team to ensure consistency across Casper Ecosystem documentation.

[Contributing Documentation](https://docs.casperlabs.io/workflow/contribute/)

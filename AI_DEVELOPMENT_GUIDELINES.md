# AI Development Guidelines

These guidelines define the development rules that AI assistants and contributors must follow when working on this repository.

The primary objective is to maintain the existing website, preserve its functionality, and make only the changes explicitly requested by the repository owner.

## 1. Inspect the Repository Before Making Changes

- Inspect the repository structure and relevant files before starting any development task.
- Identify the existing technologies, implementation patterns, dependencies, and project configuration.
- Check the current Git branch and working-tree status.
- Review related files before deciding where or how to implement a change.
- Never assume the repository structure or implementation without verifying it.

## 2. Understand the Existing Implementation

- Read and understand the relevant existing code before modifying it.
- Identify dependencies between HTML pages, CSS, JavaScript, navigation, and other website components.
- Follow the existing coding style and implementation patterns wherever practical.
- Prefer small, targeted changes over unnecessary rewrites.
- Do not replace working implementations with new ones unless explicitly requested.
- If the requested change could affect other parts of the website, identify those risks before proceeding.

## 3. Preserve Existing Website Functionality

Unless explicitly instructed otherwise, preserve all existing:

- Website functionality and interactive features.
- SEO metadata, canonical URLs, structured data, and sitemap configuration.
- Google Analytics tracking and configuration.
- Google AdSense scripts, ad placements, and configuration.
- Internal navigation, external links, and page-to-page connections.
- Existing page content, layouts, styles, and responsive behavior.
- Domain configuration, CNAME files, and GitHub Pages settings.
- Existing URLs and search-engine indexing behavior.

Do not remove, replace, rename, or modify these elements as part of unrelated development work.

## 4. Use Feature Branches for Significant Updates

- Work on a separate feature branch for significant updates, bug fixes, and new features.
- Create the branch from the latest appropriate base branch, normally `main`.
- Use clear and descriptive branch names.
- Do not develop significant changes directly on `main`.
- Keep each branch focused on one task or related group of changes.
- Avoid including unrelated modifications in the same branch.

## 5. Review Proposed Changes Before Committing

- Explain the proposed implementation before making significant changes.
- Identify every file that will be added, modified, or deleted.
- Show the complete contents of newly created files.
- Show the complete Git diff for all proposed changes.
- Explain the purpose of each change and identify any potential impact on existing functionality.
- Wait for the repository owner's review and approval before committing when approval has been requested.
- Never hide, omit, or combine unrelated changes in a review.

## 6. Protect the Main Branch

- Never force-push to `main`.
- Never force-update, reset, or rewrite the `main` branch history.
- Never bypass the normal feature-branch and pull-request workflow for significant changes.
- Do not overwrite existing files or commits to avoid resolving a conflict properly.
- Use normal Git operations and preserve repository history.

## 7. Require Explicit Approval Before Merging or Deploying

- Never merge a pull request without the repository owner's explicit approval.
- Never deploy changes without the repository owner's explicit approval.
- Opening a pull request does not constitute permission to merge it.
- A successful review or passing automated checks does not independently authorize a merge.
- Wait for explicit approval before performing any merge or deployment action.
- After merging, report the merge commit ID and the exact files changed.

## 8. Test Changes Before Recommending a Merge

- Test the functionality affected by the proposed changes.
- Verify that new features work as intended.
- Check that existing related functionality remains operational.
- Validate links, redirects, navigation, and relevant page behavior when applicable.
- Check for broken references, console errors, and obvious layout or responsive issues when applicable.
- Verify that SEO, Google Analytics, AdSense, and other protected elements remain intact when affected.
- Report which tests were performed and their results.
- Clearly disclose anything that could not be tested.
- Recommend a merge only after reviewing the changes and available test results.

---

## General Development Principle

Make only the changes necessary to complete the explicitly requested task.

Preserve existing functionality, avoid unnecessary modifications, maintain a clear Git history, and keep the repository owner in control of all commits, merges, and deployments.

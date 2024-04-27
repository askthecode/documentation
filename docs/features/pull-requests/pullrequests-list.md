---
label: List Pull Requests
icon: list-unordered
order: 100
---

[!embed](/resources/usage/pull-requests/list-all.mp4)

# List Pull Requests

### Overview

The `List Pull Requests` feature allows users to view all open pull requests within a specific GitHub repository directly from the AskTheCode GPT. This functionality provides an overview of the repository's pull request activity, aiding in code review processes and project management.

### Why It's Useful

- **Pull Request Overview**: Quickly obtain a list of all open pull requests, offering insight into ongoing changes and code reviews.
- **Facilitates Code Review**: Streamlines the process of identifying pull requests that need attention, simplifying the workflow for contributors and reviewers.
- **Pull Request Analysis**: Provides a great entrypoint for further [Pull Requests Overview](/features/pull-requests/pullrequest-overview.md), [Pull Requests Comments](/features/pull-requests/pullrequest-comments.md) and [Pull Requests Changes](/features/pull-requests/pullrequest-changes.md) features.

### How to Use

1. **Provide the Repository URL**: Begin by providing the GitHub repository URL to the AskTheCode GPT.
2. **Request Pull Request List**: Request a list of all open pull requests in the repository using a simple command like "Please list all pull requests in [repository URL]."

### Sample

```prompt
Please list pull requests in https://github.com/huggingface/pytorch-image-models
Respond with the pull request name and URL
```

### Conclusion

The `List Pull Requests` feature is an essential tool for effective GitHub repository management, providing a straightforward way to view and engage with open pull requests. It enhances user interaction with the project by facilitating quick access to and discussions about pending changes.
---

### Pull Request Changes

The `Pull Request Changes` feature focuses on analyzing the changes made in pull requests, specifically useful for PRs with numerous changed files. This feature is particularly helpful when the pull request overview cannot display all changes due to the 100k characters limitation in GPT actions responses.

#### Why It's Useful

- **Detailed File Analysis**: Provides a granular view of the changes made in each file within a pull request, enabling better understanding and review of the changes.
- **Paging Capability**: Supports paging through file changes, crucial for pull requests with extensive modifications.

#### How to Use

1. **Provide the Pull Request URL**: Start by providing the GitHub pull request URL to the AskTheCode GPT.
2. **Request Pull Request File Changes**: Specify your interest in analyzing the file changes, especially for large PRs.
3. **Navigate Through File Changes**: Use the paging functionality to move through the changes efficiently.

#### Sample

```prompt
https://github.com/dotnet/efcore/pull/10264
Please provide detailed changes for each file affected in the pull request.
```

#### Conclusion

The `Pull Request Changes` feature enhances the ability to analyze and understand the changes made in large pull requests efficiently, making it easier to review and assess the impact of those changes.


---

### Pull Request Changes

The `Pull Request Changes` feature focuses on analyzing the changes made in pull requests, specifically useful for PRs with numerous changed files. This feature is particularly helpful when the pull request overview cannot display all changes due to the 100k characters limitation in GPT actions responses.

#### Why It's Useful

- **Detailed File Analysis**: Provides a granular view of the changes made in each file within a pull request, enabling better understanding and review of the changes.
- **Paging Capability**: Supports paging through file changes, crucial for pull requests with extensive modifications.

#### How to Use

1. **Provide the Pull Request URL**: Start by providing the GitHub pull request URL to the AskTheCode GPT.
2. **Request Pull Request File Changes**: Specify your interest in analyzing the file changes, especially for large PRs.
3. **Navigate Through File Changes**: Use the paging functionality to move through the changes efficiently.

#### Sample

```prompt
https://github.com/dotnet/efcore/pull/10264
Please provide detailed changes for each file affected in the pull request.
```

#### Conclusion

The `Pull Request Changes` feature enhances the ability to analyze and understand the changes made in large pull requests efficiently, making it easier to review and assess the impact of those changes.


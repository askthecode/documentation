---
label: Pull Requests Changes
icon: file-code
order: 70
---

[!embed](/resources/usage/pull-requests/changes.mp4)

### Overview

The `Pull Request Changes` feature focuses on analyzing the changes made in pull requests, specifically useful for PRs with numerous changed files. This feature is particularly helpful when the pull request overview cannot display all changes due to the 100k characters limitation in GPT actions responses.

### Why It's Useful

- **Detailed File Analysis**: Provides a granular view of the changes made in each file within a pull request, enabling better understanding and review of the changes.
- **Paging Capability**: Supports paging through file changes, crucial for pull requests with extensive modifications.

### How to Use

1. **Provide the Pull Request URL**: Start by providing the GitHub pull request URL to the AskTheCode GPT.
2. **Request Pull Request File Changes**: Specify your interest in analyzing the file changes, especially for large PRs.
3. **Navigate Through File Changes**: Use the paging functionality to move through the changes efficiently.

### Sample

```prompt
https://github.com/dotnet/efcore/pull/33302
Please iterate over all changes and respond in the format: <changed file name> - <brief description of change>
```

### Conclusion

The `Pull Request Changes` feature enhances the ability to analyze and understand the changes made in large pull requests efficiently, making it easier to review and assess the impact of those changes.

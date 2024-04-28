---
label: Pull Requests Comments
icon: comment-discussion
order: 80
---

# Pull Request Comments

### Overview

The `Pull Request Comments` feature focuses on analyzing and managing conversations in pull requests, particularly useful for PRs with extensive discussions that exceed the capability of the standard [Pull Request Overview](/features/pull-requests/pullrequest-overview.md) feature due to response size limitations.

### Why It's Useful

- **Detailed Conversation Analysis**: Provides an in-depth view of the conversations within pull requests, enabling better understanding and management of discussions.
- **Paging Capability**: Supports paging through conversations, which is essential for large pull requests with lengthy discussions.

### How to Use

1. **Provide the Pull Request URL**: Start by providing the GitHub pull request URL to the AskTheCode GPT.
2. **Request Pull Request Comments**: Specify your interest in analyzing the comments, particularly for large PRs.
3. **Navigate Through Conversations**: Use the paging functionality to move through extensive conversations efficiently.

### Sample

```prompt
https://github.com/dotnet/efcore/pull/10264
Please iterate over the conversation and provide me a summary of each comment and the discussion under it.
```

### Conclusion

The `Pull Request Comments` feature is designed to handle extensive conversations in pull requests efficiently, making it easier to analyze and summarize those discussions.
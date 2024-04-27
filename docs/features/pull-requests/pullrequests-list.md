---
label: List Pull Requests
icon: list-unordered
order: 100
---
---
label: List Pull Requests
icon: git-pull-request
order: 110

!!!warning
Currently, the feature is supported only by the [AskTheCode GPT](https://chat.openai.com/g/g-3s6SJ5V7S-askthecode).  
!!!

# List Pull Requests

### Overview

The **List Pull Requests** feature allows users to view all open pull requests within a specific GitHub repository directly from the AskTheCode GPT. This functionality provides an overview of the repository's pull request activity, aiding in code review processes and project management.

### Why It's Useful

- **Pull Request Overview**: Quickly obtain a list of all open pull requests, offering insight into ongoing changes and code reviews.
- **Facilitates Code Review**: Streamlines the process of identifying pull requests that need attention, simplifying the workflow for contributors and reviewers.
- **Supports Collaboration**: Enhances team collaboration by allowing users to select and discuss pull requests directly through the chat UI.

### How to Use

1. **Provide the Repository URL**: Begin by providing the GitHub repository URL to the AskTheCode plugin.
2. **Request Pull Request List**: Request a list of all open pull requests in the repository using a simple command like "Please list all pull requests in [repository URL]."

### Sample

```prompt
Please list all pull requests in https://github.com/huggingface/pytorch-image-models
```

![](/resources/usage/pull-requests/list-pull-requests-response.png)

### Conclusion

The "List Pull Requests" feature is an essential tool for effective GitHub repository management, providing a straightforward way to view and engage with open pull requests. It enhances user interaction with the project by facilitating quick access to and discussions about pending changes.


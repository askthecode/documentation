---
label: List Branches
icon: list-unordered
order: 100
---

!!!warning
Currently the feature is supported only by the [AskTheCode GPT](https://chat.openai.com/g/g-3s6SJ5V7S-askthecode).
!!!

# List Branches

### Overview

The **List Branches** feature enables users to view all branches within a specific GitHub repository directly from the AskTheCode GPT. This functionality provides an overview of the repository's branch structure, making it easier to navigate and manage different versions of the project.

### Why It's Useful

- **Branch Overview**: Quickly get an overview of all branches in a repository, helping users to navigate and understand the project's structure.

- **Branch Selection for Work Continuation**: Enables users to pick up and continue working on a specific branch directly from the chat UI.

- **Branch Naming Strategy Support**: Depending on the branch naming strategy, this feature can help ChatGPT to automatically pick the correct branch for any user interactions.

### How to Use

1. **Provide the Repository URL**: Start by providing the GitHub repository URL to the AskTheCode plugin.

2. **Request Branch List**: Ask for a list of all branches in the repository using a simple command like "Please list all branches in [repository URL]."

### Sample

```prompt
Please list all branches in https://github.com/huggingface/pytorch-image-models
```

![](/resources/usage/branches/list-branches-response.png)

### Conclusion
The "List Repository Branches" feature is a vital tool for efficient GitHub repository management, offering a straightforward method to view and select branches. It enhances user interaction with the project by facilitating branch selection and supporting strategic branch naming for optimized ChatGPT integration.

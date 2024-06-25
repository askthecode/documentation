---
label: Create Pull Request
icon: git-pull-request
order: 60
---

!!!warning Beta Feature
The functionality described in this document is **currently in beta**. Please be aware that there might be some unexpected behaviors.
!!!

!!!warning
This feature is only available when the [GitHub OAuth Authentication](/authentication/#authentication-methods) is used.
!!!

# Create Pull Request

[!embed](/resources/usage/pull-requests/create.mp4)

### Overview

The **Create Pull Request** feature allows users to create a new pull request within a GitHub repository directly from the AskTheCode GPT. This feature streamlines the process of initiating code reviews and merging changes, facilitating better collaboration and project management.

### Why It's Useful

- **Simplifies Code Review Process**: Makes it easy to create pull requests directly from the chat interface, promoting more frequent and efficient code reviews.
- **Enhances Collaboration**: Encourages collaborative development by making it simpler to propose changes and request feedback.
- **Integrates Seamlessly**: Works well in conjuction with [Create Branch](/features/branches/create-branch) and [Pull Request Overview](/features/pull-requests/pullrequest-overview) features.

### How to Use

1. **Provide the Repository URL**: Start by providing the GitHub repository URL to the AskTheCode plugin.
2. **Specify Branches**: Indicate the source branch (where your changes are) and the target branch (where you want to merge the changes). Make sure to follow your project's branching strategy.
3. **Title and Description**: Optionally provide a title and description for the pull request. If not explicitly provided, AskTheCode will generate them for you.

### Sample

**Full Sample URL**: [AskTheCode GPT Sample](https://chatgpt.com/share/7da32860-c8fb-41b1-940a-ac3374ecd821)

In this example, the user asks AskTheCode to merge changes from the `2048-game` into the `main` branch. AskTheCode verifies that there are no open pull requests between these branches and then proceeds to create a new pull request. The user can then review the pull request details and make any necessary modifications.

### Conclusion

The `Create Pull Request` feature is designed to enhance the collaborative development process by simplifying the creation of pull requests. This promotes efficient code reviews and project management, ensuring that changes are thoroughly reviewed and seamlessly integrated.

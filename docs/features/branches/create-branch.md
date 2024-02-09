---
label: Create Branch
icon: git-branch
order: 90
---

!!!warning
Currently the feature is supported only by the [AskTheCode GPT](https://chat.openai.com/g/g-3s6SJ5V7S-askthecode).
!!!

!!!warning
This feature is only avalable when the [GitHub OAuth Authentication](/authentication/#authentication-methods) is used.
!!!

# Create Branch

### Overview

The **Create Branch** feature allows users to create a new branch within a GitHub repository directly from the AskTheCode GPT. This feature streamlines the process of branching, enabling users to easily manage different development paths or features within the project.

### Why It's Useful

- **Streamlines Branch Creation**: Simplifies the process of creating a new branch, making it accessible directly from the chat interface.

- **Supports Multiple Development Paths**: Facilitates the management of different features or development directions by allowing easy branch creation.

- **Facilitates Safe File Management**: Aligns well with the file content management features, highly recommended to let AskTheCode manage files in a new branch to prevent corrupting working code.

### How to Use

1. **Provide the Repository URL**: Begin by providing the GitHub repository URL to the AskTheCode plugin.

2. **Specify the New Branch Name**: Indicate the desired name for the new branch. It's important to follow any naming conventions your project adheres to.

3. **Identify the Source Branch (Optional)**: If you want the new branch to be created from a specific branch other than the default, specify the source branch.

### Sample

```prompt
Please create a new branch named "feature-x" in https://github.com/username/repository from the "development" branch.
```

![](/resources/usage/branches/create-branch.png)

### Conclusion

The **Create Branch** feature is primarily designed to enhance the file editing experience by providing a safe environment for managing changes. Creating a new branch is highly recommended when working on modifications, ensuring that the main project's code remains intact and operational.

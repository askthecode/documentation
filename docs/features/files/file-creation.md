---
label: File Creation
order: 100
icon: diff-added
---

!!!warning Beta Feature
The functionality described in this document is **currently in beta**. Please be aware that there might be some unexpected behaviors.
!!!

!!!warning
Currently the feature is supported only by the [AskTheCode GPT](https://chat.openai.com/g/g-3s6SJ5V7S-askthecode).
!!!

!!!warning
This feature is only avalable when the [GitHub OAuth Authentication](/authentication/#authentication-methods) is used.
!!!

# File Creation

### Overview

The File Creation feature in AskTheCode enables users to add new files to a GitHub repository directly through the chat interface. This functionality simplifies the process of contributing new content to a project as a result of your interactions with the AskTheCode GPT, allowing for quick and seamless integration of new resources, documentation, or code.

### Why It's Useful

- **Facilitates Persistent GPT Interactions**: This enhancement enables users to directly save the outcomes of their interactions with AskTheCode GPT into the repository. Whether it's code snippets, configuration files, or documentation generated during a chat, this feature seamlessly integrates GPT's insights into your project's development workflow.

- **Enhances Collaboration Through GPT Insights**: By allowing the storage of GPT interaction results, team members can now contribute more effectively. This feature not only preserves the context of discussions but also enriches the project repository with valuable insights, making collaboration more dynamic and informed.

### How to Use

1. **Select the Repository and Branch**: Initiate by choosing the GitHub repository URL where the new file will be created. Consider creating a new branch for these changes to maintain the stability of the project's mainline.

!!!info Caution
Creating files directly in the default branch is not prohibited but can is highly discouraged. For a safer development process, it's **highly recommended** to perform changes in a new branch. Creating a new branch for your edits isolates changes, simplifies review, and reduces the risk of unintentionally affecting the project's stability. Please, consider using a dedicated branch for any updates or modifications.
!!!

2. **Provide File Details**: Specify the path and name for the new file, including the directory structure if it should be nested within specific folders.

3. **Incorporate GPT Interaction Results**: Ask AskTheCode GPT to generate a required content and store it to the file. This could be code, documentation, or any other project-relevant content.

4. **Finalize File Creation**: Optionally you can explicitly specify the commit message to eb used. If not, AskTheCode GPT will generate appropriate commit message on its own.

### Example

In this example, the process of creating an initial HTML markup for the 2048 game within a GitHub repository is outlined. 

The operation consists of two main steps:

1. **Creating a New Branch**: A new branch is created specifically for this development activity to ensure that the main codebase remains unaffected until the new features are ready to be merged.

2. **Creating the Initial HTML File**: With the new branch set up, the AskTheCode GPT is asked to generate the initial HTML markup file for the 2048 game.

3. **Storing it to the repository**: When the content is generated, it's saved to the newly created branch in the repository.

The prompt used for this operation is as follows:

```prompt
https://github.com/askthecode/test-repo

Please do the following:

1. Create new branch 2048-game
2. In this newly created branch create html file with simple board for the 2048 game
3. Save this html to the "2048-game" directory 
```

The full sample can be found by this [link](https://chat.openai.com/share/e90ff849-6c44-4646-b53d-44d0bbd664dd).

### Conclusion

The File Creation feature enhances the GitHub experience by enabling users to easily add new files to their repositories directly from the chat interface with AskTheCode, streamlining project development and collaboration.

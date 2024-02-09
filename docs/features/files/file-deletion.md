---
label: File Deletion
order: 80
icon: diff-removed
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

# File Deletion

### Overview

The File Deletion feature in AskTheCode allows users to remove files from a GitHub repository directly through the chat interface. This functionality enables a more dynamic and interactive experience, allowing for the seamless management of repository contents.

### Why It's Useful

- **Streamlines Repository Management**: Facilitates the quick and easy removal of unnecessary or outdated files from the repository, keeping the project clean and organized.

- **Enhances Collaborative Workflows**: By allowing the deletion of files through chat, users can efficiently manage project assets and maintain a streamlined development process.

- **Supports Dynamic Project Evolution**: As projects evolve, the ability to remove files becomes crucial in adapting to new requirements or changes in project direction.

### How to Use

1. **Select the Repository and Branch**: Begin by specifying the GitHub repository URL where the file will be deleted. Ensure you're working on the correct branch to avoid unintended deletions. 

!!!info Caution
Deleting files directly in the default branch is not prohibited but can is highly discouraged. For a safer development process, it's **highly recommended** to perform changes in a new branch. Creating a new branch for your edits isolates changes, simplifies review, and reduces the risk of unintentionally affecting the project's stability. Please, consider using a dedicated branch for any updates or modifications.
!!!

2. **Identify the File to Delete**: Provide the path and name of the file you wish to remove. Accuracy is crucial to prevent the deletion of the wrong file.

3. **Confirm File Deletion**: Before proceeding, AskTheCode GPT will confirm the file deletion request to ensure it is intentional and correct. This step is crucial for avoiding accidental loss of important files.

4. **Deletion Process**: Upon confirmation, AskTheCode GPT will proceed to delete the specified file from the repository and provide feedback on the successful removal.

### Example

```prompt
Please delete the file named "old_version.txt" in the branch "feature/update" of the repository https://github.com/username/repository.
```

### Conclusion

The File Deletion feature is designed to complement the file management capabilities within GitHub repositories, offering a direct and efficient method to remove files. By integrating this feature with the chat interface, AskTheCode enhances the user experience, providing a seamless workflow for managing project contents.
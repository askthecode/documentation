---
label: Delete Branch
icon: trash
order: 10
---

!!!warning
Currently, the feature is supported only by the [AskTheCode GPT](https://chat.openai.com/g/g-3s6SJ5V7S-askthecode).
!!!

!!!warning
This feature is only available when the [GitHub OAuth Authentication](/authentication/#authentication-methods) is used.
!!!

### Overview

The **Delete Branch** feature allows users to remove an existing branch from a GitHub repository directly through AskTheCode GPT. This feature facilitates efficient branch management by enabling users to declutter the repository by removing obsolete or merged branches.

### Why It's Useful

- **Simplifies Branch Management**: Allows for the easy removal of branches that are no longer needed, keeping the repository clean and manageable.

- **Prevents Clutter**: Helps in avoiding the accumulation of stale branches, making it easier to navigate and focus on active development branches.

- **Completes Branch Management Features**: Along with creating and listing branches, deleting a branch completes the suite of branch management capabilities, offering full control over the repository's branches directly from the chat interface.

### How to Use

1. **Provide the Repository URL**: Start by giving the GitHub repository URL to the AskTheCode plugin.

2. **Specify the Branch to Delete**: Clearly state the name of the branch you wish to delete. Ensure that the branch is not protected or currently in use.

3. **Confirm Deletion (Optional)**: For safety, you may be asked to confirm the deletion request. This prevents accidental removal of important branches.

### Sample

```prompt
Please delete the "feature-x" branch in https://github.com/username/repository.
```

![](/resources/usage/branches/delete-branch.png)

### Conclusion

The **Delete Branch** feature is crucial for maintaining a clean and efficient repository. It complements the file and branch management features by allowing users to easily remove branches, ensuring that the repository remains organized and focused on current development efforts.
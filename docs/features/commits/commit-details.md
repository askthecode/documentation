---
label: Commit Details
icon: git-commit
order: 100
---

### Overview

The Commit Details feature allows users to delve deeper into the changes in the particular Github commit. By providing a link to the desired Github commit, users can ask ChatGPT questions related to the changes in this commit or even request to load the full file content before or after the commit for a more detailed analysis. Dive into the heart of Github commits, understand the changes, and analyze them without leaving the ChatGPT environment.

### Why It's Useful

- **Detailed Analysis**: Understand the changes in a commit without having to manually sift through the code.
- **Quick Insights**: Get quick answers to specific questions about a commit's changes, saving time and effort.
- **Enhanced Understanding**: By understanding the changes in a commit, developers can make more informed decisions and contribute more effectively.
- **Iterative Analysis**: For large commits, paging is implemented, allowing ChatGPT to analyze changes iteratively.
- **Full File Content Loading**: Users can request ChatGPT to load the full file content before or after the commit for a more in-depth analysis.

### Sample

#### Small commit analysis

**Full Sample URL**: [ChatGPT Sample](https://chat.openai.com/share/997785f1-4b27-478b-92c3-4672ef9b0f60)

In this sample, we are analyzing a commit from the .NET Runtime github repository:
[.NET Runtime Commit](https://github.com/dotnet/runtime/commit/b09e18e8b6092e35611c2567bd55e8909ea78d7d)

We are prompting ChatGPT with the next prompt:

```
https://github.com/dotnet/runtime/commit/b09e18e8b6092e35611c2567bd55e8909ea78d7d

Act as a proficient C# .NET developer.

Please give me an overview of the commit and then iterate over the changes in this commit, analyze files one by one. For each file output:
1. How many lines were added, updated, and deleted (in one line)
2. Describe what have been changed. Do not use some general reviews like code cleanup etc but describe the actual change. If code is added, say what new code does. If updated, analyze what was before and how the new code improves the previous one. If deleted, say what has been deleted and try to elaborate why.
3. Map changes to the commit description and how it correlates.
4. Please make a review of the changes and say if some fixes are required. Pay attention both to coding style and the meaning of changes. Especially this goes to removal - highlight which code has been removed and why. Respond only with "passed the review" or "failed."
5. Highlight areas that should be reviewed by a human. Do that only when you spot some issues with the changes or when you cannot be sure that the change is needed and solves any issue. Otherwise, say that no review is needed.
```

#### Larger commit analysis

Some commits are large enough that they cannot be analyzed in one go. To maintain response quality, the plugin pages the commit changes in the case of large commits.

**Full Sample URL**: [ChatGPT Sample](https://chat.openai.com/share/438050fd-c059-4c1e-a2e4-7b3de2d134e8)

In this sample, we'll analyze a commit from the Semantic Kernel GitHub repository:
[Semantic Kernel Commit](https://github.com/microsoft/semantic-kernel/commit/18ffc4bf2f2b57d3c58381e8d961e3757ce0c991)

In this case, the commit contains changes in 13 files. These changes are quite extensive. So, when prompted with similar prompts as above, it analyzes only the first 5 files with the first request and then analyzes the remaining files with the second request.
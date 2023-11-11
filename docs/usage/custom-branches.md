---
label: Custom Branches
icon: "git-branch"
order: 90
---

# Using Custom Branches with AskTheCode Plugin

The AskTheCode plugin is not limited to querying repositories using just the default branch. It offers flexibility by allowing users to specify a particular branch or even use a commit SHA to view the repository files at a specific point in history.

---

## Custom Branch or Commit SHA

To query a specific branch, append the branch name to the repository URL after `/tree/`, the URL would look like `https://github.com/<owner>/<repo>/tree/<branch-name>`.

To query a specific commit, append the commit SHA to the repository URL after `/tree/`, the URL would look like `https://github.com/owner/repo/tree/<commit-sha>`.

## Sample Queries

Each of the following samples demonstrates how to structure your prompt for different types of queries.

+++ :icon-command-palette: Default Branch
```prompt
https://github.com/langchain-ai/langchainjs
please give me an example of how it can be used
```
+++ :icon-git-branch: Specific Branch
```prompt
https://github.com/langchain-ai/langchainjs/tree/gh-pages
please give me an example of how it can be used
```
+++ :icon-commit: Specific Commit
```prompt
https://github.com/langchain-ai/langchainjs/tree/98f0df29d75141fd5ff53b14f17f113314122d72
please give me an example of how it can be used
```
+++

## Troubleshooting

If you encounter issues accessing specific branches or commits, consider the following steps to diagnose and resolve the problem:

1. **Check the URL Format**: Ensure that the URL format is correct when specifying a branch or commit. For branches, the URL should look like `https://github.com/<owner>/<repo>/tree/<branch-name>`. For commits, it should be `https://github.com/<owner>/<repo>/tree/<commit-sha>`.

2. **Custom Instructions for ChatGPT**: The way ChatGPT interacts with the AskTheCode plugin can be influenced by previous conversations and prompts. If you have set custom instructions for how you want ChatGPT to respond to your inquiries, it might interfere with the plugin's functionality. Consider removing or modifying these instructions and try accessing the branch or commit again.

3. **Test in a New Chat Window**: Sometimes, starting a fresh conversation can help. Try accessing the branch or commit in a new chat window using a simple prompt.

4. **Feedback and Reporting**: If you continue to face issues, provide feedback or report the issue for further assistance. Detailed information, including screenshots or specific error messages, can be helpful in diagnosing the problem.
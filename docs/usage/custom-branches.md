---
label: Custom Branches
icon: "git-branch"
order: 90
---

# Using Custom Branches with AskTheCode Plugin

The AskTheCode plugin is not limited to querying repositories using just the default branch. It offers flexibility by allowing users to specify a particular branch or even use a commit SHA to view the repository files at a specific point in history.

---

## Steps for Using Custom Branches

The AskTheCode plugin enhances your experience by supporting queries not only on the default branch but also on specified branches or even specific commits.

### Custom Branch or Commit SHA

To query a specific branch, append the branch name to the repository URL after `/tree/`, the URL would look like `https://github.com/<owner>/<repo>/tree/<branch-name>`.

To query a specific commit, append the commit SHA to the repository URL after `/tree/`, the URL would look like `https://github.com/owner/repo/tree/<commit-sha>`.

### Sample Queries

Each of the following samples demonstrates how to structure your prompt for different types of queries.

**1. Default Branch**

``` Prompt
https://github.com/langchain-ai/langchainjs
please give me an example of how it can be used
```

**2. Specific Branch**

In this sample, we're querying the `gh-pages` branch:

``` Prompt
https://github.com/langchain-ai/langchainjs/tree/gh-pages
please give me an example of how it can be used
```

**3. Specific Commit**

This sample demonstrates how to query the repository at a specific point in its history using a commit SHA:

``` Prompt
https://github.com/langchain-ai/langchainjs/tree/98f0df29d75141fd5ff53b14f17f113314122d72
please give me an example of how it can be used
```

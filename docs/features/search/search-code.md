---
label: Search Code
icon: codescan
order: 90
---

# Search Code

!!!
Only the default branch is supported for this functionality.
!!!


---

### Overview

The Search Code functionality is a feature designed to enhance interactions with Github repositories. By leveraging the Github Search, it provides more precise results when users specify particular entities such as a class, method, file etc. Unlike the base version of the plugin, which returns the entire repository structure to ChatGPT, this feature narrows down the results based on user input, ensuring more relevant and accurate responses.

### Search Hits and Contextual Analysis

One of the powerful aspects of the Search functionality is its ability to return search hits. This means that when a user queries for a specific entity, such as a method or class, the plugin doesn't just identify its presence but also provides snippets or "hits" from the file where the entity is found. 

This capability is particularly useful in scenarios where users want to understand the context or usage of a specific method or entity without fetching the entire file content. For instance, if a user asks, "Is this method only declared or also used somewhere across the file/repository?", the search hits can provide enough context to answer without needing to analyze the whole file.


### Why It's Useful

- **Enhanced Precision**: By specifying entities like files, classes, or methods, users can get directly relevant results, bypassing unrelated content.
- **Overcome Base Limitations**: The Search feature addresses the [Repository Structure Limit constraint](/features/repository-content/#constraints) of the base functionality, offering a more refined search experience.
- **Quick Access**: Users can swiftly navigate to the exact sections of a repository they're interested in.
- **Optimized for Large Repositories**: Especially useful for extensive repositories where the base functionality might be overwhelmed.

### Samples 

#### .NET Runtime Repository Analysis

**Full Sample URL**: [Proposal for Skipping Visibility Checks](https://chat.openai.com/share/e94cbb96-9aee-4e99-9b71-60e7ab1b0dab)

In this sample, we use the plugin to analyze the proposal in the .NET runtime repository. This repository is enormously large and greatly exceeds the [repository size constraints](/features/repository-content/#constraints).

Steps in the sample:
1. First, we use the [Issues](/features/github-issues) feature to analyze the proposal description and comments.
2. We try to find the details about the attribute mentioned in the proposal.
3. The continuation of the conversation is omitted, but the user could use the plugin to continue the analysis.

![](/resources/usage/search/sample.png)

### Conclusion
The `Search Code` functionality enhances the capabilities of the plugin, offering users a more refined and targeted approach to navigating Github repositories. By addressing the repository size limitations of the base functionality and providing a solution tailored to user queries, it ensures a more efficient and user-centric experience.

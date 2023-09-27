---
label: Search (beta)
icon: codescan
order: 60
---

# Search

!!!warning Beta Feature
The **Search** functionality described in this document is **currently in beta**. Please be aware that there might be some unexpected behaviors.
!!!

---

### Overview
The Github Repository Search functionality is a feature designed to enhance interactions with Github repositories. By leveraging the Github Search feature, it provides more precise results when users specify particular entities such as a class, method, file etc. Unlike the base version of the plugin, which returns the entire repository structure to ChatGPT, this feature narrows down the results based on user input, ensuring more relevant and accurate responses.

### Why It's Useful
- **Enhanced Precision**: By specifying entities like files, classes, or methods, users can get directly relevant results, bypassing unrelated content.
- **Overcome Base Limitations**: The Search feature addresses the [Repository Structure Limit constraint](/usage/basic-usage/#constraints) of the base functionality, offering a more refined search experience.
- **Quick Access**: Users can swiftly navigate to the exact sections of a repository they're interested in.
- **Optimized for Large Repositories**: Especially useful for extensive repositories where the base functionality might be overwhelmed.

### Sample: .NET Runtime Repository Analysis

**Full Sample URL**: [Proposal for Skipping Visibility Checks](https://chat.openai.com/share/e94cbb96-9aee-4e99-9b71-60e7ab1b0dab)

In this sample, we use the plugin to analyze the proposal in the .NET runtime repository. This repository is enormously large and greatly exceeds the [repository size constraints](/usage/basic-usage/#constraints).

Steps in the sample:
1. First, we use the [Issues](/usage/issues) feature to analyze the proposal description and comments.
2. We try to find the details about the attribute mentioned in the proposal.
3. The continuation of the conversation is omitted, but the user could use the plugin to continue the analysis.

![](/resources/usage/search/sample.png)

### Conclusion
The `Repository Search` functionality enhances the capabilities of the plugin, offering users a more refined and targeted approach to navigating Github repositories. By addressing the repository size limitations of the base functionality and providing a solution tailored to user queries, it ensures a more efficient and user-centric experience.

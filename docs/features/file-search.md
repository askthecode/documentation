---
label: File Search (beta)
icon: file-code
order: 50
---

# File Search

!!!warning Beta Feature
The **File Search** functionality described in this document is **currently in beta**. Please be aware that there might be some unexpected behaviors.
!!!

### Overview

The File Search functionality is a feature designed to enhance interactions with large files within Github repositories. It enables ChatGPT to conduct keyword searches within a single file, focusing on specific classes, functions, or property declarations. This feature is particularly useful for querying large files that cannot be supported as raw content.

### Search Hits and Contextual Analysis

File Search returns "search hits", meaning that when a user queries for a specific entity within a file, the plugin provides relevant snippets from the file. This capability is crucial for understanding the context or usage of a specific method or entity without fetching the entire file content.

### Why It's Useful

- **Targeted Searches**: Allows users to search for specific classes, functions, or properties within a file.
- **Large File Handling**: Ideal for interacting with large files that are too extensive for the context window of the GPT model.
- **Customizable Results**: Users can specify the number of lines to extract for each search hit.
- **Pagination of Results**: Supports pagination for extensive search results, providing partial results in the first response and allowing for subsequent requests for remaining matches.

### Example

You can find the sample usage of this feature in the [Usage > Querying Large File](/usage/large-file) documentation

### Conclusion

The `File Search` functionality enhances the capabilities of the plugin, offering a more refined and targeted approach to navigating large files in Github repositories. It addresses the challenges of interacting with large files and provides a solution tailored to user queries, ensuring a more efficient and user-centric experience.

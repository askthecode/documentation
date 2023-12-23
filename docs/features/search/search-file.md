---
label: Search File
icon: file-code
order: 100
---

# Search File

### Overview

The Search File functionality is a feature designed to enhance interactions with large files within Github repositories. It enables ChatGPT to conduct keyword searches within a single file, focusing on specific classes, functions, or property declarations. This feature is particularly useful for querying large files that cannot be supported as raw content.

### Search Hits and Contextual Analysis

Search File returns "search hits", meaning that when a user queries for a specific entity within a file, the plugin provides relevant snippets from the file. This capability is crucial for understanding the context or usage of a specific method or entity without fetching the entire file content.

### Why It's Useful

- **Targeted Searches**: Allows users to search for specific classes, functions, or properties within a file.
- **Large File Handling**: Ideal for interacting with large files that are too extensive for the context window of the GPT model.
- **Customizable Results**: Users can specify the number of lines to extract for each search hit.
- **Pagination of Results**: Supports pagination for extensive search results, providing partial results in the first response and allowing for subsequent requests for remaining matches.

### Sample

You can find the sample usage of this feature in the [Usage > Querying Large Files](/usage/large-files) documentation

### Conclusion

The `Search File` functionality enhances the capabilities of the plugin, offering a more refined and targeted approach to navigating large files in Github repositories. It addresses the challenges of interacting with large files and provides a solution tailored to user queries, ensuring a more efficient and user-centric experience.

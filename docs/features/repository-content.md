---
label: Repository Content
icon: file
order: 90
---

# Repository Content

---

### Overview

The Repository Content feature is designed to empower ChatGPT with the ability to retrieve and analyze the content of files within a GitHub repository. By first [querying the structure of the repository](/features/repository-structure), ChatGPT gains knowledge of the files present and can then selectively request the content of files deemed relevant to answer the user's question.

### Why It's Useful

- **Comprehensive Analysis**: By accessing the actual content of repository files, ChatGPT can provide detailed insights, explanations, and code suggestions.
- **Optimized File Retrieval**: AskTheCode employs multiple strategies to reduce file sizes and ensure efficient content retrieval, especially for large files.
- **Private Repository Access**: this feature supports accessing private repositories if the user is [authenticated with their GitHub account](/authentication).
- **Paging Support**: For extensive files, AskTheCode enforces content paging to ensure that ChatGPT can analyze the file without hallucinations.

### Constraints

- **File Size Limit:** The maximum file size supported by AskTheCode is **50,000** characters long. This limit is due to the current restrictions of ChatGPT for the maximum plugin response size.  
- **Large Files:** Issues can occur with very large files due to the limits of the ChatGPT context size. It's recommended to be cautious when analyzing large files.
- **Repository Structure Limit:** Currently, the plugin can retrieve the structure of repositories that have less than **100,000 files** with a maximum size of **7 MB** for their structure. This limitation is derived from the [GitHub tree endpoint](https://docs.github.com/en/rest/git/trees?apiVersion=2022-11-28#get-a-tree).

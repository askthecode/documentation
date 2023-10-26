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

### Sample

#### Basic sample

The sample and guidelines can be found [here](/usage/basic-usage)

#### Retrieving Files by Pages

Sometimes you might prompt ChatGPT for something that will require it to query multiple files from the repository, and the total size of these files can be quite large. If the plugin were to simply return all contents to ChatGPT, it would significantly overflow the context of the GPT-4 model used under the hood, and resulted in a poor response quality. To prevent this, the plugin detects when the total size of the requested files is significant and pages them.

Let's assume that we want to query all functions defined in the [Langchain Utils directory](https://github.com/langchain-ai/langchain/tree/master/libs/langchain/langchain/utils).

Sample conversation: https://chat.openai.com/share/f349d959-d957-47f7-a7f7-0febe9197602

The total size of all files within this directory is large, which would result in ChatGPT compressing file contents, significantly impacting the response quality. Instead, the plugin paginates results, allowing ChatGPT to analyze the amount of data it can process at once.
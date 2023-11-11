---
label: Basic Usage
icon: "file"
order: 100
---

# Basic Usage

!!!warning Warning
The screenshots provided in this guide are based on an older version of the AskTheCode plugin. The actual response from the plugin might differ (and hopefully be better) in the latest versions.
!!!

The AskTheCode plugin is designed to assist developers in analyzing GitHub repositories. By integrating with ChatGPT, users can ask questions directly related to the content and structure of a given repository. This documentation will guide you through the basic usage of the plugin.

---

## Prerequisites

- A GitHub repository URL you wish to analyze.
- AskTheCode plugin installed

---

## Steps for Basic Usage

1. **Provide the Repository Link:**  
   Start by providing the GitHub repository URL to the AskTheCode plugin.

2. **Ask Questions:**  
   With the repository URL provided, you can now ask specific questions related to the repository. For instance, if you want to know about the purpose or details of a particular project, simply ask.

3. **Interact and Analyze:**  
   Based on the responses from the plugin, you can continue to interact with ChatGPT to get deeper insights, explanations, or even code suggestions related to the repository.

---

## Sample: LangChain

If you're curious about a particular GitHub repository and want to get general information or insights, the AskTheCode plugin can be invaluable. Let's take the "LangChain" repository as an example.

**Input the following prompt:**  

```prompt
https://github.com/langchain-ai/langchain  
What is LangChain?
```

In a barebone ChatGPT, without any plugins, it might not know anything about "LangChain".

![](/resources/usage/basic-usage/no-plugin-installed.png)

However, with the AskTheCode plugin, ChatGPT can directly fetch and analyze the information from the provided GitHub repository and answer the question.

![](/resources/usage/basic-usage/plugin-installed.png)

---

## Tips

- Ensure that the repository URL is correct and accessible.
- Be specific in your questions to get more accurate and relevant answers.
- Familiarize yourself with the repository's structure to ask more targeted questions.

---
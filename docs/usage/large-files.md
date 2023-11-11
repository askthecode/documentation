---
label: Querying Large Files
icon: file-code
order: 70
---

# Querying Large Files

!!!warning Warning
The screenshots provided in this guide are based on an older version of the AskTheCode plugin. The actual response from the plugin might differ (and hopefully be better) in the latest versions.
!!!

In this guide, we'll investigate how the [File Search](/features/file-search) feature can assist in analyzing large files. We'll conduct the analysis on the [Qdrant vector store](https://github.com/langchain-ai/langchain/blob/master/libs/langchain/langchain/vectorstores/qdrant.py) from the Langchain repository. This file is 91.5K characters long, so it won't fit into the GPT-4 context for analysis, which could result in model hallucinations.

Full demo can be found here:
[Qdrant Class and Function](https://chat.openai.com/share/64c1546a-9b0c-4cdf-a78e-34cab69d4eb9)

## Prerequisites

- Access to the Qdrant vectorstore in the Langchain repository: [https://github.com/langchain-ai/langchain/blob/master/libs/langchain/langchain/vectorstores/qdrant.py](https://github.com/langchain-ai/langchain/blob/master/libs/langchain/langchain/vectorstores/qdrant.py)
- AskTheCode plugin installed

## Step 1: Retrieving all defined classes and functions

The first step is to retrieve all defined classes and functions of the Qdrant vectorstore.

**Input the following prompt:**  

```prompt
https://github.com/langchain-ai/langchain/

Please find path to the file that defines the qdrant vectorstore. Once you know the file path, search for all defined classes and functions in this file.
```

## Step 2: Plugin Searching In The File

Upon receiving the prompt, AskTheCode will first iterate through the repository and search for the Qdrant vector store. Once found, it will perform the search for the class and function definitions within the file:

![](/resources/usage/large-files/step2.png)

It's worth noting how ChatGPT understood which keywords it should use when searching for classes and functions in the Python code:

![](/resources/usage/large-files/step2-plugin-request.png)

## Step 3: Retrieving Body Of The Specific Function

Now we want to ask the plugin to give us the body of the `_asearch_with_score_by_vector ` function, that we can use for our further analysis.

**Input the following prompt:**

```prompt
Please search for the definition of the _asearch_with_score_by_vector function. Grab first 300 lines. Respond with the body of this function.
```

In this prompt, we are explicitly specifying how many lines of code we want to extract to ensure that the whole function body will be contained in the plugin response.

## Step 4: Plugin Retrieves The Function

Upon receiving the prompt, AskTheCode will search the Qdrant vectorstore file once again, now for a specific function:

![](/resources/usage/large-files/step4.png)

## Conclusion

In this guide, we explored the powerful capabilities of the [File Search](/features/file-search) feature in the AskTheCode plugin, particularly in handling large files. Our case study involved the Qdrant vector store from the Langchain repository, a file too large for traditional analysis within the GPT-4 context.


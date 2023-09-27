---
label: Step-by-Step Prompting
icon: number
order: 80
---

# Step-by-Step Prompting

!!!warning Warning
The screenshots provided in this guide are based on an older version of the AskTheCode plugin. The actual response from the plugin might differ (and hopefully be better) in the latest versions.
!!!

In this guide, we'll showcase the power of specifying steps for the AskTheCode plugin. By providing a structured prompt, you can guide the plugin to analyze code in a more focused manner, ensuring you get the insights you need.

## Prerequisites

- Access to the eShopOnWeb repository: [https://github.com/dotnet-architecture/eShopOnWeb](https://github.com/dotnet-architecture/eShopOnWeb)
- AskTheCode plugin installed

## Step 1: Crafting the Prompt for AskTheCode Plugin

The first step is to provide a clear and structured prompt to the AskTheCode plugin. This prompt acts as a set of instructions, guiding the plugin on what to analyze and how.

**Input the following prompt:**  

```plaintext
You are a technical documentation writer for the eShopOnWeb repository. Your task is to provide a clear and detailed description of the full handling flow for the endpoint 'GET api/catalog-items' in the given GitHub repository: 
https://github.com/dotnet-architecture/eShopOnWeb

Follow these steps:

1. Locate the file that handles the specified route in the repository.
2. Analyze the code of the handler to understand its functionality.
3. Fetch the code of all dependencies related to the route handler and data retrieval logic.
4. Analyze the dependencies, including their code and further dependencies if needed.
5. Describe the main components involved in handling the 'GET api/catalog-items' endpoint and explain their interaction.

Ensure your description includes any abstract classes or interface implementations as well as explanations of any external library usage. 
Make sure to provide a structured and easy-to-understand response that demonstrates a deep understanding of the codebase.
```

## Step 2: Plugin's Search for the Route Handler

Upon receiving the prompt, AskTheCode will begin its search for the file handling the 'GET api/catalog-items' route.

![](/resources/usage/step-by-step/step2.png)

## Step 3: Plugin Identifying Dependencies

The plugin will then identify and fetch the dependencies related to the route handler. This is based on the instructions provided in the prompt.

![](/resources/usage/step-by-step/step3.png)

## Step 4: Plugin's Dependency Analysis

AskTheCode will analyze the dependencies, diving deep into their code, understanding their functionality, and identifying any further dependencies.

![](/resources/usage/step-by-step/step4.png)

## Step 5: Reviewing the Plugin's Response

Once the analysis is complete, AskTheCode will provide a comprehensive description of the main components, their interactions, and any other relevant details as instructed in the prompt.

## Visualizing the Analysis: Mermaid Flowchart

To further enhance our understanding of the 'GET api/catalog-items' endpoint and its dependencies, we can visualize the results using a Mermaid flowchart. This provides a graphical representation of the interactions and flow of the endpoint, making it easier to grasp the overall structure and logic.

By prompting ChatGPT with the following:

```
Please build a mermaid flowchart diagram based on this research
```

We can obtain a Mermaid diagram as follows:

```mermaid
flowchart TD

subgraph CatalogItemListPagedEndpoint
    A[GET api/catalog-items] --> B[HandleAsync]
    B --> C[Use CatalogFilterSpecification]
    B --> D[Use CatalogFilterPaginatedSpecification]
    B --> E[Fetch items from IRepository<CatalogItem>]
    B --> F[Map items using IMapper]
    B --> G[Compose picture URIs using IUriComposer]
end

subgraph Specifications
    C --> H[Filter by brandId & typeId]
    D --> I[Paginate results]
end

subgraph Dependencies
    E --> J[IRepository<CatalogItem>]
    F --> K[IMapper]
    G --> L[IUriComposer]
end

subgraph IRepository
    J --> M[CRUD operations]
    J --> N[Query methods]
end
```

## Conclusion

By providing a clear and structured prompt to the AskTheCode plugin, you can harness its power to get precise insights into specific parts of a codebase. This approach can be replicated for other endpoints or repositories, demonstrating the flexibility and capability of the plugin.



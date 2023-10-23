---
label: Repository Structure
icon: list-unordered
order: 100
---

# Github Repository Structure Retrieval

---

### Overview
The Github Repository Structure Retrieval feature is an integral part of the AskTheCode plugin, designed to empower users with the ability to seamlessly explore the structure of any given GitHub repository. By simply providing the link to a desired repository, users can gain a comprehensive understanding of its structure, including directories and files, without the need to navigate manually through GitHub's interface.

### Why It's Useful
- **Effortless Repository Exploration**: With this feature, a single link is all you need to get a detailed overview of any repository's structure.
  
- **Branch and Commit Flexibility**: Whether you're looking to explore the default branch, delve into a custom branch, or even analyze the repository at a specific commit, this feature has got you covered. This flexibility ensures that users can get insights into the repository's state at any point in its history. More details con be found in [Custom Branches documentation](/usage/custom-branches)
  
- **Tailored Directory Content Retrieval**: Interested in a specific directory or multiple directories within the repository? No problem! Specify your areas of interest, and the plugin will retrieve the contents just for you.

### Limitations
The retrieval of the entire structure for very large repositories can be challenging due to the constraints of the ChatGPT context size. To address this limitation and ensure efficient and user-friendly interactions, the feature is designed to initially present only the directories for large repositories. This approach allows ChatGPT to specify which directory or directories it wish to explore further, enabling a more targeted and manageable exploration. This design choice ensures that despite the inherent constraints, users can still gain meaningful insights into the structure of large repositories without overwhelming ChatGPT.

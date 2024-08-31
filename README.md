# Memory Operations Experimentation with Large Language Models (LLMs)

<image src="./notebooks/girl.png" width=100>
<image src="./notebooks/surprised-cat-with-huge-eyes-free-photo.jpg" width=100>

This repository hosts a series of experiments focused on memory operations using various Large Language Models (LLMs), including ChatGPT-4, ChatGPT-3.5, and Ollama/Llama3.1-8b. The experiments explore how these models handle memory addition, injection, and update/deletion across different data types.

## Table of Contents

- [Experiments Overview](#experiments-overview)
  - [Experiment 1: Memory Addition](#experiment-1-memory-addition)
  - [Experiment 2: Memory Injection](#experiment-2-memory-injection)
  - [Experiment 3: Memory Update and Deletion](#experiment-3-memory-update-and-deletion)
- [Development Guidelines](#development-guidelines)
- [Testing and Evaluation](#testing-and-evaluation)
- [End Goal](#end-goal)
- [Contributing](#contributing)
- [License](#license)
- [Authors and Acknowledgments](#authors-and-acknowledgments)

## Experiments Overview

### Experiment 1: Memory Addition

The first experiment focuses on adding memories with different data types (string, integer, datetime) across three LLMs:
- **ChatGPT-4**
- **ChatGPT-3.5**
- **Ollama/Llama3.1-8b**

For each model, three sub-experiments will be conducted:
1. Memory addition with strings.
2. Memory addition with integers.
3. Memory addition with datetime objects.

Each sub-experiment will evaluate the model’s ability to store and retrieve 10 distinct memory entries. The results will be visualized across 9 figures, each representing one LLM and one data type.

### Experiment 2: Memory Injection

The second experiment will explore how well the models can handle memory injection. Specifics of this experiment will build on the results from Experiment 1, focusing on injecting new memory entries into the models and evaluating their recall accuracy.

### Experiment 3: Memory Update and Deletion

The third experiment will test the models' capabilities to update and delete existing memories. This will include:
- Updating existing memory entries with new information.
- Deleting specific memory entries and ensuring they are not retrievable.

## Development Guidelines

To maintain a high standard of development, please adhere to the following guidelines:
1. **Do not include API keys in the code.** Use environment variables or secure methods to handle sensitive information.
2. **Follow a pull request review process.** All code changes should be peer-reviewed to ensure quality and consistency.
3. **Separate test data from test code.** Store test data in YAML or JSON files to keep the codebase clean and organized.

## Testing and Evaluation

### Test Classes

Memory operations will be tested across three types of data:
1. **String data:** Evaluate the model's ability to recall multiple strings, such as languages learned.
2. **Integer data:** Test the model's recall of numerical data, such as test scores or IDs.
3. **Datetime data:** Assess the model's handling of date-related information, like events over the past year.

### Evaluation Metrics

1. **Direct Memory Check:** Verify the memory entries directly in the database (e.g., mem0).
2. **General Queries:** Ask broad questions (e.g., "What languages have I learned?") to evaluate the model’s ability to search and combine multiple memories.
3. **Specific Queries:** Ask targeted questions (e.g., "Have I learned X language?") to test individual memory retrieval.

### Experiment Parameters

- **Temperature Setting:** Start with a low temperature (0) and observe the results. If time permits, experiment with higher temperatures to analyze changes in memory recall behavior.

## End Goal

The final goal is to generate a table comparing the success rate of memory operations across different LLMs and data types:

|           | Llama3.1-8b | ChatGPT-4 | ChatGPT-3.5 |
|-----------|-------------|-----------|-------------|
| **Int**   |             |           |             |
| **Str**   |             |           |             |
| **Date**  |             |           |             |

Each cell in the table will represent the number of successful tests for the respective model and data type.

## Contributing

We welcome contributions from the open-source community to improve the experiments, add new tests, or refine the existing methodology. Please ensure that you follow the development guidelines and submit changes via pull requests for review.

### Professional Notes for Community Members

We encourage all contributors to:
- Uphold high standards in code quality and documentation.
- Engage in constructive discussions during pull requests and code reviews.
- Adhere to security best practices, especially in handling sensitive data like API keys.

By contributing, you help advance the research in memory operations with LLMs and contribute to a shared knowledge base that benefits the entire AI community.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Authors and Acknowledgments

This project is developed and maintained by **Darren** and **Spark** at **Trend Micro AILAB**. We would like to thank all contributors and community members for their valuable input and support.

---

**Trend Micro AILAB** is committed to driving innovation in AI research and development. This project reflects our dedication to advancing the field of AI while maintaining the highest standards of quality and professionalism.
